# Comparing `tmp/bluezero-0.7.1.tar.gz` & `tmp/bluezero-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluezero-0.7.1.tar", last modified: Thu Jul 14 18:04:56 2022, max compression
+gzip compressed data, was "bluezero-0.8.0.tar", last modified: Sun Aug  6 16:22:26 2023, max compression
```

## Comparing `bluezero-0.7.1.tar` & `bluezero-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 18:04:56.084624 bluezero-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-07-14 18:04:48.000000 bluezero-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5007 2022-07-14 18:04:56.084624 bluezero-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-07-14 18:04:48.000000 bluezero-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 18:04:56.080624 bluezero-0.7.1/bluezero/
--rwxr-xr-x   0 runner    (1001) docker     (121)    15260 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/GATT.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11459 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    11695 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/advertisement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/async_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/broadcaster.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3605 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/central.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1801 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14410 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/dbus_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10491 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/eddystone_beacon.py
--rw-r--r--   0 runner    (1001) docker     (121)    19156 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/localGATT.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/media_player.py
--rw-r--r--   0 runner    (1001) docker     (121)    36504 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/microbit.py
--rw-r--r--   0 runner    (1001) docker     (121)    10052 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/observer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6857 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/peripheral.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5849 2022-07-14 18:04:48.000000 bluezero-0.7.1/bluezero/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 18:04:56.080624 bluezero-0.7.1/bluezero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5007 2022-07-14 18:04:56.000000 bluezero-0.7.1/bluezero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-07-14 18:04:56.000000 bluezero-0.7.1/bluezero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 18:04:56.000000 bluezero-0.7.1/bluezero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-14 18:04:56.000000 bluezero-0.7.1/bluezero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-14 18:04:56.000000 bluezero-0.7.1/bluezero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-14 18:04:56.084624 bluezero-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-07-14 18:04:48.000000 bluezero-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:26.870475 bluezero-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-06 16:22:16.000000 bluezero-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-06 16:22:26.870475 bluezero-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-08-06 16:22:16.000000 bluezero-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:26.866475 bluezero-0.8.0/bluezero/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15260 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/GATT.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11459 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/advertisement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/async_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/broadcaster.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3605 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/central.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14410 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/dbus_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10491 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/eddystone_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19355 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/localGATT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/media_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36504 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/microbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/observer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6857 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/peripheral.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5849 2023-08-06 16:22:16.000000 bluezero-0.8.0/bluezero/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:22:26.870475 bluezero-0.8.0/bluezero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 16:22:26.000000 bluezero-0.8.0/bluezero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-06 16:22:26.870475 bluezero-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-08-06 16:22:16.000000 bluezero-0.8.0/setup.py
```

### Comparing `bluezero-0.7.1/LICENSE` & `bluezero-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/PKG-INFO` & `bluezero-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: bluezero
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python library for Bluetooth Low Energy (BLE) on Linux
 Home-page: https://github.com/ukBaz/python-bluezero
 Author: Barry Byford
 Author-email: barry_byford@yahoo.co.uk
 Maintainer: Barry Byford
 Maintainer-email: barry_byford@yahoo.co.uk
 License: MIT
 Keywords: Bluetooth BLE development
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Education
@@ -138,9 +137,7 @@
 
 It is based on a proprietary UART service specification by Nordic Semiconductors.
 Data sent to and from this service can be viewed using the nRF UART apps from Nordic
 Semiconductors for Android and iOS.
 
 It uses the Bluezero peripheral file (level 10) so should be easier than the previous CPU
 Temperature example that was a level 100.
-
-
```

### Comparing `bluezero-0.7.1/README.rst` & `bluezero-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/GATT.py` & `bluezero-0.8.0/bluezero/GATT.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/adapter.py` & `bluezero-0.8.0/bluezero/adapter.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/advertisement.py` & `bluezero-0.8.0/bluezero/advertisement.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/async_tools.py` & `bluezero-0.8.0/bluezero/async_tools.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/broadcaster.py` & `bluezero-0.8.0/bluezero/broadcaster.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/central.py` & `bluezero-0.8.0/bluezero/central.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/constants.py` & `bluezero-0.8.0/bluezero/constants.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/dbus_tools.py` & `bluezero-0.8.0/bluezero/dbus_tools.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/device.py` & `bluezero-0.8.0/bluezero/device.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/eddystone_beacon.py` & `bluezero-0.8.0/bluezero/eddystone_beacon.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/localGATT.py` & `bluezero-0.8.0/bluezero/localGATT.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Classes required to create a Bluetooth Peripheral."""
 
+from inspect import signature
+
 # D-Bus imports
 import dbus
 import dbus.exceptions
 import dbus.service
 from dbus.mainloop.glib import DBusGMainLoop
 
 # python-bluezero imports
@@ -346,15 +348,18 @@
     def ReadValue(self, options):  # pylint: disable=invalid-name
         """
         DBus method for getting the characteristic value
 
         :return: value
         """
         if self.read_callback:
-            value = self.read_callback()
+            if len(signature(self.read_callback).parameters) == 1:
+                value = self.read_callback(dbus_tools.dbus_to_python(options))
+            else:
+                value = self.read_callback()
             self.Set(constants.GATT_CHRC_IFACE, 'Value',
                      dbus.Array(value, signature='y'))
             logger.debug('ReadValue: %s', value)
         return self.GetAll(constants.GATT_CHRC_IFACE)['Value']
 
     @dbus.service.method(constants.GATT_CHRC_IFACE,
                          in_signature='aya{sv}', out_signature='')
```

### Comparing `bluezero-0.7.1/bluezero/media_player.py` & `bluezero-0.8.0/bluezero/media_player.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/microbit.py` & `bluezero-0.8.0/bluezero/microbit.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/observer.py` & `bluezero-0.8.0/bluezero/observer.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/peripheral.py` & `bluezero-0.8.0/bluezero/peripheral.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero/tools.py` & `bluezero-0.8.0/bluezero/tools.py`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/bluezero.egg-info/PKG-INFO` & `bluezero-0.8.0/bluezero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: bluezero
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python library for Bluetooth Low Energy (BLE) on Linux
 Home-page: https://github.com/ukBaz/python-bluezero
 Author: Barry Byford
 Author-email: barry_byford@yahoo.co.uk
 Maintainer: Barry Byford
 Maintainer-email: barry_byford@yahoo.co.uk
 License: MIT
 Keywords: Bluetooth BLE development
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Education
@@ -138,9 +137,7 @@
 
 It is based on a proprietary UART service specification by Nordic Semiconductors.
 Data sent to and from this service can be viewed using the nRF UART apps from Nordic
 Semiconductors for Android and iOS.
 
 It uses the Bluezero peripheral file (level 10) so should be easier than the previous CPU
 Temperature example that was a level 100.
-
-
```

### Comparing `bluezero-0.7.1/bluezero.egg-info/SOURCES.txt` & `bluezero-0.8.0/bluezero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluezero-0.7.1/setup.py` & `bluezero-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 setup(
     name='bluezero',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.7.1',
+    version='0.8.0',
 
     description='Python library for Bluetooth Low Energy (BLE) on Linux',
     long_description=long_description,
     long_description_content_type='text/x-rst',
 
     # The project's main homepage.
     url='https://github.com/ukBaz/python-bluezero',
```

