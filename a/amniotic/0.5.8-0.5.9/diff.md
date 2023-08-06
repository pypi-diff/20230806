# Comparing `tmp/amniotic-0.5.8.tar.gz` & `tmp/amniotic-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amniotic-0.5.8.tar", last modified: Sat Jun 24 14:35:41 2023, max compression
+gzip compressed data, was "amniotic-0.5.9.tar", last modified: Sat Aug  5 12:30:34 2023, max compression
```

## Comparing `amniotic-0.5.8.tar` & `amniotic-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.024410 amniotic-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-24 14:35:41.024410 amniotic-0.5.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.020410 amniotic-0.5.8/amniotic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.024410 amniotic-0.5.8/amniotic/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/mqtt/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 14:35:38.000000 amniotic-0.5.8/amniotic/version
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-24 14:35:33.000000 amniotic-0.5.8/amniotic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:35:41.020410 amniotic-0.5.8/amniotic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-24 14:35:41.000000 amniotic-0.5.8/amniotic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:35:40.000000 amniotic-0.5.8/amniotic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:35:41.024410 amniotic-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-24 14:35:33.000000 amniotic-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:30:34.445958 amniotic-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-05 12:30:34.445958 amniotic-0.5.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:30:34.445958 amniotic-0.5.9/amniotic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:30:34.445958 amniotic-0.5.9/amniotic/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/mqtt/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/mqtt/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/mqtt/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/mqtt/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/mqtt/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 12:30:31.000000 amniotic-0.5.9/amniotic/version
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:30:24.000000 amniotic-0.5.9/amniotic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:30:34.445958 amniotic-0.5.9/amniotic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-05 12:30:34.000000 amniotic-0.5.9/amniotic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-05 12:30:34.000000 amniotic-0.5.9/amniotic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:30:34.000000 amniotic-0.5.9/amniotic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-05 12:30:34.000000 amniotic-0.5.9/amniotic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 12:30:34.000000 amniotic-0.5.9/amniotic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:30:34.000000 amniotic-0.5.9/amniotic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:30:34.445958 amniotic-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-05 12:30:24.000000 amniotic-0.5.9/setup.py
```

### Comparing `amniotic-0.5.8/PKG-INFO` & `amniotic-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.8
+Version: 0.5.9
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `amniotic-0.5.8/amniotic/audio.py` & `amniotic-0.5.9/amniotic/audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,46 +44,53 @@
     When a player is not yet open, we need to open one temporarily to fetch the audio devices. Since this is somewhat
     expensive, here we cache the devices with a limited lifespan, so that this is only done so often.
 
     """
     logging.info(f'Loaded temporary player to get devices...')
     player = load_new_player()
     devices_raw = player.audio_output_device_enum()
-    unload_player(player)
     logging.info(f'Unloading temporary player.')
+    unload_player(player)
     return devices_raw
 
 def get_devices(player: Optional[vlc.MediaPlayer] = None, device_names: dict[str, str] = None) -> dict[str, str]:
     """
 
     Create a mapping from audio output device IDs to their friendly names from VLC's peculiar enum format.
 
     """
 
+    log_devices = False
     if player:
         devices_raw = player.audio_output_device_enum()
     else:
         devices_raw = get_devices_raw()
+        log_devices = True
 
-    devices = {}
-    device_names = device_names or {}
+    devices_pairs = []
     if devices_raw:
         device_raw = devices_raw
-        count = 0
         while device_raw:
-            count += 1
             device_raw = device_raw.contents
             description = device_raw.description.decode()
             device = device_raw.device.decode()
-            count = len([key for key in devices.keys() if key == description])
-            if count:
-                description = f'{description} ({count + 1})'
-            devices[device] = device_names.get(description, description)
+            devices_pairs.append((device, description))
             device_raw = device_raw.next
 
+    devices = {}
+    device_names = device_names or {}
+    for device_id, description in devices_pairs:
+        count = len([value for value in devices.values() if value == description])
+        if count:
+            description = f'{description} ({count + 1})'
+        devices[device_id] = device_names.get(description, description)
+
+    if log_devices:
+        logging.info(f'Found devices: {devices}')
+
     return devices
 
 
 def sanitize_volume(value: Number) -> int:
     """
 
     Ensure a volume is an `int` between 0 and 100
```

### Comparing `amniotic-0.5.8/amniotic/config.py` & `amniotic-0.5.9/amniotic/config.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.8/amniotic/mqtt/control.py` & `amniotic-0.5.9/amniotic/mqtt/control.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.8/amniotic/mqtt/device.py` & `amniotic-0.5.9/amniotic/mqtt/device.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.8/amniotic/mqtt/loop.py` & `amniotic-0.5.9/amniotic/mqtt/loop.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.8/amniotic/mqtt/sensor.py` & `amniotic-0.5.9/amniotic/mqtt/sensor.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.8/amniotic/mqtt/tools.py` & `amniotic-0.5.9/amniotic/mqtt/tools.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.8/amniotic.egg-info/PKG-INFO` & `amniotic-0.5.9/amniotic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.8
+Version: 0.5.9
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `amniotic-0.5.8/setup.py` & `amniotic-0.5.9/setup.py`

 * *Files identical despite different names*

