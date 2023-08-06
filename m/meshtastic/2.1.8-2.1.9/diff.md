# Comparing `tmp/meshtastic-2.1.8.tar.gz` & `tmp/meshtastic-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.1.8.tar", last modified: Tue May 30 12:46:56 2023, max compression
+gzip compressed data, was "meshtastic-2.1.9.tar", last modified: Wed Jun 28 01:16:29 2023, max compression
```

## Comparing `meshtastic-2.1.8.tar` & `meshtastic-2.1.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:56.532436 meshtastic-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 12:46:44.000000 meshtastic-2.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 12:46:44.000000 meshtastic-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 12:46:56.532436 meshtastic-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-30 12:46:44.000000 meshtastic-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:56.532436 meshtastic-2.1.8/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/device_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    37626 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/xmodem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:56.532436 meshtastic-2.1.8/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:46:56.536436 meshtastic-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-30 12:46:44.000000 meshtastic-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:16:29.853455 meshtastic-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-28 01:16:17.000000 meshtastic-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-28 01:16:17.000000 meshtastic-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-28 01:16:29.853455 meshtastic-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-28 01:16:17.000000 meshtastic-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:16:29.853455 meshtastic-2.1.9/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/device_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37626 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21895 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-28 01:16:17.000000 meshtastic-2.1.9/meshtastic/xmodem_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:16:29.853455 meshtastic-2.1.9/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-28 01:16:29.000000 meshtastic-2.1.9/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-28 01:16:29.000000 meshtastic-2.1.9/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:16:29.000000 meshtastic-2.1.9/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-28 01:16:29.000000 meshtastic-2.1.9/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-28 01:16:29.000000 meshtastic-2.1.9/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 01:16:29.000000 meshtastic-2.1.9/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:16:29.853455 meshtastic-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-28 01:16:18.000000 meshtastic-2.1.9/setup.py
```

### Comparing `meshtastic-2.1.8/LICENSE.txt` & `meshtastic-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/PKG-INFO` & `meshtastic-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.8/README.md` & `meshtastic-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/__init__.py` & `meshtastic-2.1.9/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/__main__.py` & `meshtastic-2.1.9/meshtastic/__main__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/admin_pb2.py` & `meshtastic-2.1.9/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/apponly_pb2.py` & `meshtastic-2.1.9/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/ble_interface.py` & `meshtastic-2.1.9/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.1.9/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/channel_pb2.py` & `meshtastic-2.1.9/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/clientonly_pb2.py` & `meshtastic-2.1.9/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/config_pb2.py` & `meshtastic-2.1.9/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/connection_status_pb2.py` & `meshtastic-2.1.9/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/device_metadata_pb2.py` & `meshtastic-2.1.9/meshtastic/device_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/deviceonly_pb2.py` & `meshtastic-2.1.9/meshtastic/deviceonly_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,37 +12,54 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import channel_pb2 as meshtastic_dot_channel__pb2
 from meshtastic import localonly_pb2 as meshtastic_dot_localonly__pb2
 from meshtastic import mesh_pb2 as meshtastic_dot_mesh__pb2
+from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/deviceonly.proto\x1a\x18meshtastic/channel.proto\x1a\x1ameshtastic/localonly.proto\x1a\x15meshtastic/mesh.proto\x1a\x1emeshtastic/module_config.proto\"\xbd\x02\n\x0b\x44\x65viceState\x12\x1c\n\x07my_node\x18\x02 \x01(\x0b\x32\x0b.MyNodeInfo\x12\x14\n\x05owner\x18\x03 \x01(\x0b\x32\x05.User\x12\x1a\n\x07node_db\x18\x04 \x03(\x0b\x32\t.NodeInfo\x12\"\n\rreceive_queue\x18\x05 \x03(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07version\x18\x08 \x01(\r\x12$\n\x0frx_text_message\x18\x07 \x01(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07no_save\x18\t \x01(\x08\x12\x15\n\rdid_gps_reset\x18\x0b \x01(\x08\x12 \n\x0brx_waypoint\x18\x0c \x01(\x0b\x32\x0b.MeshPacket\x12\x39\n\x19node_remote_hardware_pins\x18\r \x03(\x0b\x32\x16.NodeRemoteHardwarePin\":\n\x0b\x43hannelFile\x12\x1a\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x08.Channel\x12\x0f\n\x07version\x18\x02 \x01(\r\"\xf6\x01\n\x08OEMStore\x12\x16\n\x0eoem_icon_width\x18\x01 \x01(\r\x12\x17\n\x0foem_icon_height\x18\x02 \x01(\r\x12\x15\n\roem_icon_bits\x18\x03 \x01(\x0c\x12\x1e\n\x08oem_font\x18\x04 \x01(\x0e\x32\x0c.ScreenFonts\x12\x10\n\x08oem_text\x18\x05 \x01(\t\x12\x13\n\x0boem_aes_key\x18\x06 \x01(\x0c\x12&\n\x10oem_local_config\x18\x07 \x01(\x0b\x32\x0c.LocalConfig\x12\x33\n\x17oem_local_module_config\x18\x08 \x01(\x0b\x32\x12.LocalModuleConfig\"J\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12\x1f\n\x03pin\x18\x02 \x01(\x0b\x32\x12.RemoteHardwarePin*>\n\x0bScreenFonts\x12\x0e\n\nFONT_SMALL\x10\x00\x12\x0f\n\x0b\x46ONT_MEDIUM\x10\x01\x12\x0e\n\nFONT_LARGE\x10\x02\x42_\n\x13\x63om.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bmeshtastic/deviceonly.proto\x1a\x18meshtastic/channel.proto\x1a\x1ameshtastic/localonly.proto\x1a\x15meshtastic/mesh.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x1emeshtastic/module_config.proto\"\xe6\x02\n\x0b\x44\x65viceState\x12\x1c\n\x07my_node\x18\x02 \x01(\x0b\x32\x0b.MyNodeInfo\x12\x14\n\x05owner\x18\x03 \x01(\x0b\x32\x05.User\x12\x1e\n\x07node_db\x18\x04 \x03(\x0b\x32\t.NodeInfoB\x02\x18\x01\x12\"\n\rreceive_queue\x18\x05 \x03(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07version\x18\x08 \x01(\r\x12$\n\x0frx_text_message\x18\x07 \x01(\x0b\x32\x0b.MeshPacket\x12\x0f\n\x07no_save\x18\t \x01(\x08\x12\x15\n\rdid_gps_reset\x18\x0b \x01(\x08\x12 \n\x0brx_waypoint\x18\x0c \x01(\x0b\x32\x0b.MeshPacket\x12\x39\n\x19node_remote_hardware_pins\x18\r \x03(\x0b\x32\x16.NodeRemoteHardwarePin\x12#\n\x0cnode_db_lite\x18\x0e \x03(\x0b\x32\r.NodeInfoLite\"\xab\x01\n\x0cNodeInfoLite\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1f\n\x08position\x18\x03 \x01(\x0b\x32\r.PositionLite\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\x85\x01\n\x0cPositionLite\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\":\n\x0b\x43hannelFile\x12\x1a\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x08.Channel\x12\x0f\n\x07version\x18\x02 \x01(\r\"\xf6\x01\n\x08OEMStore\x12\x16\n\x0eoem_icon_width\x18\x01 \x01(\r\x12\x17\n\x0foem_icon_height\x18\x02 \x01(\r\x12\x15\n\roem_icon_bits\x18\x03 \x01(\x0c\x12\x1e\n\x08oem_font\x18\x04 \x01(\x0e\x32\x0c.ScreenFonts\x12\x10\n\x08oem_text\x18\x05 \x01(\t\x12\x13\n\x0boem_aes_key\x18\x06 \x01(\x0c\x12&\n\x10oem_local_config\x18\x07 \x01(\x0b\x32\x0c.LocalConfig\x12\x33\n\x17oem_local_module_config\x18\x08 \x01(\x0b\x32\x12.LocalModuleConfig\"J\n\x15NodeRemoteHardwarePin\x12\x10\n\x08node_num\x18\x01 \x01(\r\x12\x1f\n\x03pin\x18\x02 \x01(\x0b\x32\x12.RemoteHardwarePin*>\n\x0bScreenFonts\x12\x0e\n\nFONT_SMALL\x10\x00\x12\x0f\n\x0b\x46ONT_MEDIUM\x10\x01\x12\x0e\n\nFONT_LARGE\x10\x02\x42_\n\x13\x63om.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _SCREENFONTS = DESCRIPTOR.enum_types_by_name['ScreenFonts']
 ScreenFonts = enum_type_wrapper.EnumTypeWrapper(_SCREENFONTS)
 FONT_SMALL = 0
 FONT_MEDIUM = 1
 FONT_LARGE = 2
 
 
 _DEVICESTATE = DESCRIPTOR.message_types_by_name['DeviceState']
+_NODEINFOLITE = DESCRIPTOR.message_types_by_name['NodeInfoLite']
+_POSITIONLITE = DESCRIPTOR.message_types_by_name['PositionLite']
 _CHANNELFILE = DESCRIPTOR.message_types_by_name['ChannelFile']
 _OEMSTORE = DESCRIPTOR.message_types_by_name['OEMStore']
 _NODEREMOTEHARDWAREPIN = DESCRIPTOR.message_types_by_name['NodeRemoteHardwarePin']
 DeviceState = _reflection.GeneratedProtocolMessageType('DeviceState', (_message.Message,), {
   'DESCRIPTOR' : _DEVICESTATE,
   '__module__' : 'meshtastic.deviceonly_pb2'
   # @@protoc_insertion_point(class_scope:DeviceState)
   })
 _sym_db.RegisterMessage(DeviceState)
 
+NodeInfoLite = _reflection.GeneratedProtocolMessageType('NodeInfoLite', (_message.Message,), {
+  'DESCRIPTOR' : _NODEINFOLITE,
+  '__module__' : 'meshtastic.deviceonly_pb2'
+  # @@protoc_insertion_point(class_scope:NodeInfoLite)
+  })
+_sym_db.RegisterMessage(NodeInfoLite)
+
+PositionLite = _reflection.GeneratedProtocolMessageType('PositionLite', (_message.Message,), {
+  'DESCRIPTOR' : _POSITIONLITE,
+  '__module__' : 'meshtastic.deviceonly_pb2'
+  # @@protoc_insertion_point(class_scope:PositionLite)
+  })
+_sym_db.RegisterMessage(PositionLite)
+
 ChannelFile = _reflection.GeneratedProtocolMessageType('ChannelFile', (_message.Message,), {
   'DESCRIPTOR' : _CHANNELFILE,
   '__module__' : 'meshtastic.deviceonly_pb2'
   # @@protoc_insertion_point(class_scope:ChannelFile)
   })
 _sym_db.RegisterMessage(ChannelFile)
 
@@ -60,18 +77,24 @@
   })
 _sym_db.RegisterMessage(NodeRemoteHardwarePin)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nDeviceOnlyZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _SCREENFONTS._serialized_start=845
-  _SCREENFONTS._serialized_end=907
-  _DEVICESTATE._serialized_start=141
-  _DEVICESTATE._serialized_end=458
-  _CHANNELFILE._serialized_start=460
-  _CHANNELFILE._serialized_end=518
-  _OEMSTORE._serialized_start=521
-  _OEMSTORE._serialized_end=767
-  _NODEREMOTEHARDWAREPIN._serialized_start=769
-  _NODEREMOTEHARDWAREPIN._serialized_end=843
+  _DEVICESTATE.fields_by_name['node_db']._options = None
+  _DEVICESTATE.fields_by_name['node_db']._serialized_options = b'\030\001'
+  _SCREENFONTS._serialized_start=1224
+  _SCREENFONTS._serialized_end=1286
+  _DEVICESTATE._serialized_start=169
+  _DEVICESTATE._serialized_end=527
+  _NODEINFOLITE._serialized_start=530
+  _NODEINFOLITE._serialized_end=701
+  _POSITIONLITE._serialized_start=704
+  _POSITIONLITE._serialized_end=837
+  _CHANNELFILE._serialized_start=839
+  _CHANNELFILE._serialized_end=897
+  _OEMSTORE._serialized_start=900
+  _OEMSTORE._serialized_end=1146
+  _NODEREMOTEHARDWAREPIN._serialized_start=1148
+  _NODEREMOTEHARDWAREPIN._serialized_end=1222
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.8/meshtastic/globals.py` & `meshtastic-2.1.9/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/localonly_pb2.py` & `meshtastic-2.1.9/meshtastic/localonly_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/localonly.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\"\xb0\x02\n\x0bLocalConfig\x12$\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfig\x12(\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfig\x12\"\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfig\x12&\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfig\x12&\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfig\x12 \n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfig\x12*\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfig\x12\x0f\n\x07version\x18\x08 \x01(\r\"\x81\x04\n\x11LocalModuleConfig\x12&\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfig\x12*\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfig\x12G\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfig\x12\x37\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfig\x12\x31\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfig\x12\x30\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfig\x12\x39\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfig\x12(\n\x05\x61udio\x18\t \x01(\x0b\x32\x19.ModuleConfig.AudioConfig\x12;\n\x0fremote_hardware\x18\n \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfig\x12\x0f\n\x07version\x18\x08 \x01(\rBd\n\x13\x63om.geeksville.meshB\x0fLocalOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/localonly.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\"\xb0\x02\n\x0bLocalConfig\x12$\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfig\x12(\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfig\x12\"\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfig\x12&\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfig\x12&\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfig\x12 \n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfig\x12*\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfig\x12\x0f\n\x07version\x18\x08 \x01(\r\"\xba\x04\n\x11LocalModuleConfig\x12&\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfig\x12*\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfig\x12G\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfig\x12\x37\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfig\x12\x31\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfig\x12\x30\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfig\x12\x39\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfig\x12(\n\x05\x61udio\x18\t \x01(\x0b\x32\x19.ModuleConfig.AudioConfig\x12;\n\x0fremote_hardware\x18\n \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfig\x12\x37\n\rneighbor_info\x18\x0b \x01(\x0b\x32 .ModuleConfig.NeighborInfoConfig\x12\x0f\n\x07version\x18\x08 \x01(\rBd\n\x13\x63om.geeksville.meshB\x0fLocalOnlyProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 
 
 _LOCALCONFIG = DESCRIPTOR.message_types_by_name['LocalConfig']
 _LOCALMODULECONFIG = DESCRIPTOR.message_types_by_name['LocalModuleConfig']
 LocalConfig = _reflection.GeneratedProtocolMessageType('LocalConfig', (_message.Message,), {
   'DESCRIPTOR' : _LOCALCONFIG,
@@ -39,9 +39,9 @@
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\017LocalOnlyProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _LOCALCONFIG._serialized_start=88
   _LOCALCONFIG._serialized_end=392
   _LOCALMODULECONFIG._serialized_start=395
-  _LOCALMODULECONFIG._serialized_end=908
+  _LOCALMODULECONFIG._serialized_end=965
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.8/meshtastic/mesh_interface.py` & `meshtastic-2.1.9/meshtastic/mesh_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/mesh_pb2.py` & `meshtastic-2.1.9/meshtastic/mesh_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 from meshtastic import portnums_pb2 as meshtastic_dot_portnums__pb2
 from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import xmodem_pb2 as meshtastic_dot_xmodem__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xb7\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\x81\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x0f\n\x07macaddr\x18\x04 \x01(\x0c\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"\xcb\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12$\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.Delayed\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xa3\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\x86\x03\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x0f\n\x07has_gps\x18\x02 \x01(\x08\x12\x14\n\x0cmax_channels\x18\x03 \x01(\r\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12&\n\nerror_code\x18\x05 \x01(\x0e\x32\x12.CriticalErrorCode\x12\x15\n\rerror_address\x18\x06 \x01(\r\x12\x13\n\x0b\x65rror_count\x18\x07 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x0f\n\x07\x62itrate\x18\t \x01(\x02\x12\x1c\n\x14message_timeout_msec\x18\n \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\x12\x15\n\rair_period_tx\x18\x0c \x03(\r\x12\x15\n\rair_period_rx\x18\r \x03(\r\x12\x10\n\x08has_wifi\x18\x0e \x01(\x08\x12\x1b\n\x13\x63hannel_utilization\x18\x0f \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x10 \x01(\x02\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xa7\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x42\x11\n\x0fpayload_variant\"\x8c\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"V\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12\x1c\n\tneighbors\x18\x03 \x03(\x0b\x32\t.Neighbor\"(\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\"\x97\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08*\xea\x04\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xb7\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\x85\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x13\n\x07macaddr\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"\xcb\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12$\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.Delayed\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xa3\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\xba\x03\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x13\n\x07has_gps\x18\x02 \x01(\x08\x42\x02\x18\x01\x12\x18\n\x0cmax_channels\x18\x03 \x01(\rB\x02\x18\x01\x12\x1c\n\x10\x66irmware_version\x18\x04 \x01(\tB\x02\x18\x01\x12*\n\nerror_code\x18\x05 \x01(\x0e\x32\x12.CriticalErrorCodeB\x02\x18\x01\x12\x19\n\rerror_address\x18\x06 \x01(\rB\x02\x18\x01\x12\x17\n\x0b\x65rror_count\x18\x07 \x01(\rB\x02\x18\x01\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x13\n\x07\x62itrate\x18\t \x01(\x02\x42\x02\x18\x01\x12 \n\x14message_timeout_msec\x18\n \x01(\rB\x02\x18\x01\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\x12\x19\n\rair_period_tx\x18\x0c \x03(\rB\x02\x18\x01\x12\x19\n\rair_period_rx\x18\r \x03(\rB\x02\x18\x01\x12\x14\n\x08has_wifi\x18\x0e \x01(\x08\x42\x02\x18\x01\x12\x1f\n\x13\x63hannel_utilization\x18\x0f \x01(\x02\x42\x02\x18\x01\x12\x17\n\x0b\x61ir_util_tx\x18\x10 \x01(\x02\x42\x02\x18\x01\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xa7\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x42\x11\n\x0fpayload_variant\"\x8c\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"V\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12\x1c\n\tneighbors\x18\x03 \x03(\x0b\x32\t.Neighbor\"(\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\"\x97\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08*\xea\x04\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _HARDWAREMODEL = DESCRIPTOR.enum_types_by_name['HardwareModel']
 HardwareModel = enum_type_wrapper.EnumTypeWrapper(_HARDWAREMODEL)
 _CONSTANTS = DESCRIPTOR.enum_types_by_name['Constants']
 Constants = enum_type_wrapper.EnumTypeWrapper(_CONSTANTS)
 _CRITICALERRORCODE = DESCRIPTOR.enum_types_by_name['CriticalErrorCode']
 CriticalErrorCode = enum_type_wrapper.EnumTypeWrapper(_CRITICALERRORCODE)
@@ -224,60 +224,88 @@
   })
 _sym_db.RegisterMessage(DeviceMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _HARDWAREMODEL._serialized_start=4034
-  _HARDWAREMODEL._serialized_end=4652
-  _CONSTANTS._serialized_start=4654
-  _CONSTANTS._serialized_end=4698
-  _CRITICALERRORCODE._serialized_start=4701
-  _CRITICALERRORCODE._serialized_end=4939
+  _USER.fields_by_name['macaddr']._options = None
+  _USER.fields_by_name['macaddr']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['has_gps']._options = None
+  _MYNODEINFO.fields_by_name['has_gps']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['max_channels']._options = None
+  _MYNODEINFO.fields_by_name['max_channels']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['firmware_version']._options = None
+  _MYNODEINFO.fields_by_name['firmware_version']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['error_code']._options = None
+  _MYNODEINFO.fields_by_name['error_code']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['error_address']._options = None
+  _MYNODEINFO.fields_by_name['error_address']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['error_count']._options = None
+  _MYNODEINFO.fields_by_name['error_count']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['bitrate']._options = None
+  _MYNODEINFO.fields_by_name['bitrate']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['message_timeout_msec']._options = None
+  _MYNODEINFO.fields_by_name['message_timeout_msec']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['air_period_tx']._options = None
+  _MYNODEINFO.fields_by_name['air_period_tx']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['air_period_rx']._options = None
+  _MYNODEINFO.fields_by_name['air_period_rx']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['has_wifi']._options = None
+  _MYNODEINFO.fields_by_name['has_wifi']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['channel_utilization']._options = None
+  _MYNODEINFO.fields_by_name['channel_utilization']._serialized_options = b'\030\001'
+  _MYNODEINFO.fields_by_name['air_util_tx']._options = None
+  _MYNODEINFO.fields_by_name['air_util_tx']._serialized_options = b'\030\001'
+  _HARDWAREMODEL._serialized_start=4090
+  _HARDWAREMODEL._serialized_end=4708
+  _CONSTANTS._serialized_start=4710
+  _CONSTANTS._serialized_end=4754
+  _CRITICALERRORCODE._serialized_start=4757
+  _CRITICALERRORCODE._serialized_end=4995
   _POSITION._serialized_start=189
   _POSITION._serialized_end=884
   _POSITION_LOCSOURCE._serialized_start=706
   _POSITION_LOCSOURCE._serialized_end=784
   _POSITION_ALTSOURCE._serialized_start=786
   _POSITION_ALTSOURCE._serialized_end=884
   _USER._serialized_start=887
-  _USER._serialized_end=1016
-  _ROUTEDISCOVERY._serialized_start=1018
-  _ROUTEDISCOVERY._serialized_end=1049
-  _ROUTING._serialized_start=1052
-  _ROUTING._serialized_end=1399
-  _ROUTING_ERROR._serialized_start=1186
-  _ROUTING_ERROR._serialized_end=1388
-  _DATA._serialized_start=1402
-  _DATA._serialized_end=1558
-  _WAYPOINT._serialized_start=1561
-  _WAYPOINT._serialized_end=1708
-  _MESHPACKET._serialized_start=1711
-  _MESHPACKET._serialized_end=2170
-  _MESHPACKET_PRIORITY._serialized_start=1992
-  _MESHPACKET_PRIORITY._serialized_end=2083
-  _MESHPACKET_DELAYED._serialized_start=2085
-  _MESHPACKET_DELAYED._serialized_end=2151
-  _NODEINFO._serialized_start=2173
-  _NODEINFO._serialized_end=2336
-  _MYNODEINFO._serialized_start=2339
-  _MYNODEINFO._serialized_end=2729
-  _LOGRECORD._serialized_start=2732
-  _LOGRECORD._serialized_end=2913
-  _LOGRECORD_LEVEL._serialized_start=2825
-  _LOGRECORD_LEVEL._serialized_end=2913
-  _QUEUESTATUS._serialized_start=2915
-  _QUEUESTATUS._serialized_end=2995
-  _FROMRADIO._serialized_start=2998
-  _FROMRADIO._serialized_end=3421
-  _TORADIO._serialized_start=3424
-  _TORADIO._serialized_end=3564
-  _COMPRESSED._serialized_start=3566
-  _COMPRESSED._serialized_end=3619
-  _NEIGHBORINFO._serialized_start=3621
-  _NEIGHBORINFO._serialized_end=3707
-  _NEIGHBOR._serialized_start=3709
-  _NEIGHBOR._serialized_end=3749
-  _DEVICEMETADATA._serialized_start=3752
-  _DEVICEMETADATA._serialized_end=4031
+  _USER._serialized_end=1020
+  _ROUTEDISCOVERY._serialized_start=1022
+  _ROUTEDISCOVERY._serialized_end=1053
+  _ROUTING._serialized_start=1056
+  _ROUTING._serialized_end=1403
+  _ROUTING_ERROR._serialized_start=1190
+  _ROUTING_ERROR._serialized_end=1392
+  _DATA._serialized_start=1406
+  _DATA._serialized_end=1562
+  _WAYPOINT._serialized_start=1565
+  _WAYPOINT._serialized_end=1712
+  _MESHPACKET._serialized_start=1715
+  _MESHPACKET._serialized_end=2174
+  _MESHPACKET_PRIORITY._serialized_start=1996
+  _MESHPACKET_PRIORITY._serialized_end=2087
+  _MESHPACKET_DELAYED._serialized_start=2089
+  _MESHPACKET_DELAYED._serialized_end=2155
+  _NODEINFO._serialized_start=2177
+  _NODEINFO._serialized_end=2340
+  _MYNODEINFO._serialized_start=2343
+  _MYNODEINFO._serialized_end=2785
+  _LOGRECORD._serialized_start=2788
+  _LOGRECORD._serialized_end=2969
+  _LOGRECORD_LEVEL._serialized_start=2881
+  _LOGRECORD_LEVEL._serialized_end=2969
+  _QUEUESTATUS._serialized_start=2971
+  _QUEUESTATUS._serialized_end=3051
+  _FROMRADIO._serialized_start=3054
+  _FROMRADIO._serialized_end=3477
+  _TORADIO._serialized_start=3480
+  _TORADIO._serialized_end=3620
+  _COMPRESSED._serialized_start=3622
+  _COMPRESSED._serialized_end=3675
+  _NEIGHBORINFO._serialized_start=3677
+  _NEIGHBORINFO._serialized_end=3763
+  _NEIGHBOR._serialized_start=3765
+  _NEIGHBOR._serialized_end=3805
+  _DEVICEMETADATA._serialized_start=3808
+  _DEVICEMETADATA._serialized_end=4087
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.8/meshtastic/module_config_pb2.py` & `meshtastic-2.1.9/meshtastic/module_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xbb\x18\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1aw\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12*\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x12.RemoteHardwarePin\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\xce\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\x12$\n\x1coverride_console_serial_port\x18\x08 \x01(\x08\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"U\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x12\x0b\n\x07\x43\x41LTOPO\x10\x05\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variant\"Y\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xb6\x19\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x12\x39\n\rneighbor_info\x18\n \x01(\x0b\x32 .ModuleConfig.NeighborInfoConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1aw\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12*\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x12.RemoteHardwarePin\x1a>\n\x12NeighborInfoConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x17\n\x0fupdate_interval\x18\x02 \x01(\r\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\xce\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\x12$\n\x1coverride_console_serial_port\x18\x08 \x01(\x08\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"U\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x12\x0b\n\x07\x43\x41LTOPO\x10\x05\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variant\"Y\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _REMOTEHARDWAREPINTYPE = DESCRIPTOR.enum_types_by_name['RemoteHardwarePinType']
 RemoteHardwarePinType = enum_type_wrapper.EnumTypeWrapper(_REMOTEHARDWAREPINTYPE)
 UNKNOWN = 0
 DIGITAL_READ = 1
 DIGITAL_WRITE = 2
 
 
 _MODULECONFIG = DESCRIPTOR.message_types_by_name['ModuleConfig']
 _MODULECONFIG_MQTTCONFIG = _MODULECONFIG.nested_types_by_name['MQTTConfig']
 _MODULECONFIG_REMOTEHARDWARECONFIG = _MODULECONFIG.nested_types_by_name['RemoteHardwareConfig']
+_MODULECONFIG_NEIGHBORINFOCONFIG = _MODULECONFIG.nested_types_by_name['NeighborInfoConfig']
 _MODULECONFIG_AUDIOCONFIG = _MODULECONFIG.nested_types_by_name['AudioConfig']
 _MODULECONFIG_SERIALCONFIG = _MODULECONFIG.nested_types_by_name['SerialConfig']
 _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG = _MODULECONFIG.nested_types_by_name['ExternalNotificationConfig']
 _MODULECONFIG_STOREFORWARDCONFIG = _MODULECONFIG.nested_types_by_name['StoreForwardConfig']
 _MODULECONFIG_RANGETESTCONFIG = _MODULECONFIG.nested_types_by_name['RangeTestConfig']
 _MODULECONFIG_TELEMETRYCONFIG = _MODULECONFIG.nested_types_by_name['TelemetryConfig']
 _MODULECONFIG_CANNEDMESSAGECONFIG = _MODULECONFIG.nested_types_by_name['CannedMessageConfig']
@@ -51,14 +52,21 @@
   'RemoteHardwareConfig' : _reflection.GeneratedProtocolMessageType('RemoteHardwareConfig', (_message.Message,), {
     'DESCRIPTOR' : _MODULECONFIG_REMOTEHARDWARECONFIG,
     '__module__' : 'meshtastic.module_config_pb2'
     # @@protoc_insertion_point(class_scope:ModuleConfig.RemoteHardwareConfig)
     })
   ,
 
+  'NeighborInfoConfig' : _reflection.GeneratedProtocolMessageType('NeighborInfoConfig', (_message.Message,), {
+    'DESCRIPTOR' : _MODULECONFIG_NEIGHBORINFOCONFIG,
+    '__module__' : 'meshtastic.module_config_pb2'
+    # @@protoc_insertion_point(class_scope:ModuleConfig.NeighborInfoConfig)
+    })
+  ,
+
   'AudioConfig' : _reflection.GeneratedProtocolMessageType('AudioConfig', (_message.Message,), {
     'DESCRIPTOR' : _MODULECONFIG_AUDIOCONFIG,
     '__module__' : 'meshtastic.module_config_pb2'
     # @@protoc_insertion_point(class_scope:ModuleConfig.AudioConfig)
     })
   ,
 
@@ -106,14 +114,15 @@
   'DESCRIPTOR' : _MODULECONFIG,
   '__module__' : 'meshtastic.module_config_pb2'
   # @@protoc_insertion_point(class_scope:ModuleConfig)
   })
 _sym_db.RegisterMessage(ModuleConfig)
 _sym_db.RegisterMessage(ModuleConfig.MQTTConfig)
 _sym_db.RegisterMessage(ModuleConfig.RemoteHardwareConfig)
+_sym_db.RegisterMessage(ModuleConfig.NeighborInfoConfig)
 _sym_db.RegisterMessage(ModuleConfig.AudioConfig)
 _sym_db.RegisterMessage(ModuleConfig.SerialConfig)
 _sym_db.RegisterMessage(ModuleConfig.ExternalNotificationConfig)
 _sym_db.RegisterMessage(ModuleConfig.StoreForwardConfig)
 _sym_db.RegisterMessage(ModuleConfig.RangeTestConfig)
 _sym_db.RegisterMessage(ModuleConfig.TelemetryConfig)
 _sym_db.RegisterMessage(ModuleConfig.CannedMessageConfig)
@@ -125,40 +134,42 @@
   })
 _sym_db.RegisterMessage(RemoteHardwarePin)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\022ModuleConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _REMOTEHARDWAREPINTYPE._serialized_start=3259
-  _REMOTEHARDWAREPINTYPE._serialized_end=3332
+  _REMOTEHARDWAREPINTYPE._serialized_start=3382
+  _REMOTEHARDWAREPINTYPE._serialized_end=3455
   _MODULECONFIG._serialized_start=35
-  _MODULECONFIG._serialized_end=3166
-  _MODULECONFIG_MQTTCONFIG._serialized_start=547
-  _MODULECONFIG_MQTTCONFIG._serialized_end=714
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=716
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=835
-  _MODULECONFIG_AUDIOCONFIG._serialized_start=838
-  _MODULECONFIG_AUDIOCONFIG._serialized_end=1183
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=1016
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1183
-  _MODULECONFIG_SERIALCONFIG._serialized_start=1186
-  _MODULECONFIG_SERIALCONFIG._serialized_end=1776
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1423
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1689
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1691
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1776
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1779
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=2113
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=2116
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2248
-  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2250
-  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2314
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2317
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2579
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2582
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3147
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=3048
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3147
-  _REMOTEHARDWAREPIN._serialized_start=3168
-  _REMOTEHARDWAREPIN._serialized_end=3257
+  _MODULECONFIG._serialized_end=3289
+  _MODULECONFIG_MQTTCONFIG._serialized_start=606
+  _MODULECONFIG_MQTTCONFIG._serialized_end=773
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=775
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=894
+  _MODULECONFIG_NEIGHBORINFOCONFIG._serialized_start=896
+  _MODULECONFIG_NEIGHBORINFOCONFIG._serialized_end=958
+  _MODULECONFIG_AUDIOCONFIG._serialized_start=961
+  _MODULECONFIG_AUDIOCONFIG._serialized_end=1306
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=1139
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1306
+  _MODULECONFIG_SERIALCONFIG._serialized_start=1309
+  _MODULECONFIG_SERIALCONFIG._serialized_end=1899
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1546
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1812
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1814
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1899
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1902
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=2236
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=2239
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2371
+  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2373
+  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2437
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2440
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2702
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2705
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3270
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=3171
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3270
+  _REMOTEHARDWAREPIN._serialized_start=3291
+  _REMOTEHARDWAREPIN._serialized_end=3380
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.8/meshtastic/mqtt_pb2.py` & `meshtastic-2.1.9/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/node.py` & `meshtastic-2.1.9/meshtastic/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         """Show human readable description of our channels."""
         print("Channels:")
         if self.channels:
             logging.debug(f"self.channels:{self.channels}")
             for c in self.channels:
                 # print('c.settings.psk:', c.settings.psk)
                 cStr = stripnl(MessageToJson(c.settings))
-                # only show if there is no psk (meaning disabled channel)
-                if c.settings.psk:
+                # don't show disabled channels
+                if channel_pb2.Channel.Role.Name(c.role)!="DISABLED":
                     print(
                         f"  {channel_pb2.Channel.Role.Name(c.role)} psk={pskToString(c.settings.psk)} {cStr}"
                     )
         publicURL = self.getURL(includeAll=False)
         adminURL = self.getURL(includeAll=True)
         print(f"\nPrimary channel URL: {publicURL}")
         if adminURL != publicURL:
@@ -184,14 +184,18 @@
             )
         elif config_name == "audio":
             p.set_module_config.audio.CopyFrom(self.moduleConfig.audio)
         elif config_name == "remote_hardware":
             p.set_module_config.remote_hardware.CopyFrom(
                 self.moduleConfig.remote_hardware
             )
+        elif config_name == "neighbor_info":
+            p.set_module_config.neighbor_info.CopyFrom(
+                self.moduleConfig.neighbor_info
+            )
         else:
             our_exit(f"Error: No valid config with name {config_name}")
 
         logging.debug(f"Wrote: {config_name}")
         if self == self.iface.localNode:
             onResponse = None
         else:
```

### Comparing `meshtastic-2.1.8/meshtastic/portnums_pb2.py` & `meshtastic-2.1.9/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/remote_hardware.py` & `meshtastic-2.1.9/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.1.9/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/rtttl_pb2.py` & `meshtastic-2.1.9/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/serial_interface.py` & `meshtastic-2.1.9/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/storeforward_pb2.py` & `meshtastic-2.1.9/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/stream_interface.py` & `meshtastic-2.1.9/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/supported_device.py` & `meshtastic-2.1.9/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/tcp_interface.py` & `meshtastic-2.1.9/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/telemetry_pb2.py` & `meshtastic-2.1.9/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/test.py` & `meshtastic-2.1.9/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/tunnel.py` & `meshtastic-2.1.9/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/util.py` & `meshtastic-2.1.9/meshtastic/util.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic/xmodem_pb2.py` & `meshtastic-2.1.9/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.1.9/meshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.8/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.1.9/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.8/setup.py` & `meshtastic-2.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.1.8",
+    version="2.1.9",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

