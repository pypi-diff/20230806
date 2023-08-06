# Comparing `tmp/greeneye_monitor-4.0-py3-none-any.whl.zip` & `tmp/greeneye_monitor-4.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12142 bytes, number of entries: 10
+Zip file size: 12178 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       30 b- defN 22-May-27 16:30 greeneye/__init__.py
--rw-r--r--  2.0 unx     9130 b- defN 23-May-20 00:16 greeneye/api.py
--rw-r--r--  2.0 unx    29242 b- defN 23-May-30 18:20 greeneye/monitor.py
--rw-r--r--  2.0 unx      325 b- defN 23-May-15 16:41 greeneye/protocol.py
+-rw-r--r--  2.0 unx     9130 b- defN 23-May-31 00:18 greeneye/api.py
+-rw-r--r--  2.0 unx    29306 b- defN 23-Aug-06 19:48 greeneye/monitor.py
+-rw-r--r--  2.0 unx      325 b- defN 23-May-31 00:18 greeneye/protocol.py
 -rw-r--r--  2.0 unx        0 b- defN 22-May-27 16:30 greeneye/py.typed
--rw-r--r--  2.0 unx     1296 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2851 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      791 b- defN 23-May-30 22:25 greeneye_monitor-4.0.dist-info/RECORD
-10 files, 43766 bytes uncompressed, 10790 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx     1296 b- defN 23-Aug-06 19:51 greeneye_monitor-4.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2853 b- defN 23-Aug-06 19:51 greeneye_monitor-4.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 19:51 greeneye_monitor-4.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-06 19:51 greeneye_monitor-4.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      801 b- defN 23-Aug-06 19:51 greeneye_monitor-4.0.1.dist-info/RECORD
+10 files, 43842 bytes uncompressed, 10806 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: greeneye/protocol.py
 Comment: 
 
 Filename: greeneye/py.typed
 Comment: 
 
-Filename: greeneye_monitor-4.0.dist-info/LICENSE
+Filename: greeneye_monitor-4.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: greeneye_monitor-4.0.dist-info/METADATA
+Filename: greeneye_monitor-4.0.1.dist-info/METADATA
 Comment: 
 
-Filename: greeneye_monitor-4.0.dist-info/WHEEL
+Filename: greeneye_monitor-4.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: greeneye_monitor-4.0.dist-info/top_level.txt
+Filename: greeneye_monitor-4.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: greeneye_monitor-4.0.dist-info/RECORD
+Filename: greeneye_monitor-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## greeneye/monitor.py

```diff
@@ -543,17 +543,17 @@
         if self.type == MonitorType.GEM:
             # Initialize temperature sensors if needed
             for num in range(len(self.temperature_sensors), NUM_TEMPERATURE_SENSORS):
                 self.temperature_sensors.append(
                     TemperatureSensor(self, num, settings.temperature_unit)
                 )
 
-            self.pulse_counters = [
-                PulseCounter(self, num) for num in range(0, NUM_PULSE_COUNTERS)
-            ]
+            # Initialize pulse counters if needed
+            for num in range(len(self.pulse_counters), NUM_PULSE_COUNTERS):
+                self.pulse_counters.append(PulseCounter(self, num))
 
         # Voltage sensor was created up front
 
         # Now update settings if needed and trigger listeners
         coroutines = []
         for temperature_sensor in self.temperature_sensors:
             coroutines.append(temperature_sensor.handle_settings(settings))
```

## Comparing `greeneye_monitor-4.0.dist-info/LICENSE` & `greeneye_monitor-4.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `greeneye_monitor-4.0.dist-info/METADATA` & `greeneye_monitor-4.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greeneye-monitor
-Version: 4.0
+Version: 4.0.1
 Summary: Receive data packets from GreenEye Monitor (http://www.brultech.com/greeneye/)
 Home-page: https://github.com/jkeljo/greeneye-monitor
 Author: Jonathan Keljo
 Keywords: greeneye
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

