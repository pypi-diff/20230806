# Comparing `tmp/sunsynk-0.3.7.tar.gz` & `tmp/sunsynk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.7.tar", last modified: Wed Jul 19 12:53:30 2023, max compression
+gzip compressed data, was "sunsynk-0.4.0.tar", last modified: Sun Aug  6 19:18:30 2023, max compression
```

## Comparing `sunsynk-0.3.7.tar` & `sunsynk-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 12:53:21.000000 sunsynk-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 12:53:21.000000 sunsynk-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 12:53:30.366794 sunsynk-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-19 12:53:21.000000 sunsynk-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 12:53:30.366794 sunsynk-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-19 12:53:21.000000 sunsynk-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8207 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-19 12:53:21.000000 sunsynk-0.3.7/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:53:30.000000 sunsynk-0.3.7/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass-addon-sunsynk-dev.zip
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:30.366794 sunsynk-0.3.7/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_pysunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-19 12:53:21.000000 sunsynk-0.3.7/tests/sunsynk/test_usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:30.646280 sunsynk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 19:18:19.000000 sunsynk-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 19:18:19.000000 sunsynk-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-06 19:18:30.646280 sunsynk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-06 19:18:19.000000 sunsynk-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-06 19:18:30.646280 sunsynk-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-06 19:18:19.000000 sunsynk-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:30.642280 sunsynk-0.4.0/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8207 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/solarmansunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-06 19:18:19.000000 sunsynk-0.4.0/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:30.642280 sunsynk-0.4.0/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-06 19:18:30.000000 sunsynk-0.4.0/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-06 19:18:30.000000 sunsynk-0.4.0/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:18:30.000000 sunsynk-0.4.0/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-06 19:18:30.000000 sunsynk-0.4.0/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 19:18:30.000000 sunsynk-0.4.0/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:18:30.000000 sunsynk-0.4.0/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:30.642280 sunsynk-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass-addon-sunsynk-dev.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:30.642280 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:30.646280 sunsynk-0.4.0/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_pysunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-06 19:18:19.000000 sunsynk-0.4.0/tests/sunsynk/test_usunsynk.py
```

### Comparing `sunsynk-0.3.7/LICENSE` & `sunsynk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/PKG-INFO` & `sunsynk-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.7
+Version: 0.4.0
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.7/README.md` & `sunsynk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/setup.cfg` & `sunsynk-0.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 tests = 
 	pytest
 	pytest-asyncio
 	pytest-cov
 	pytest-github-actions-annotate-failures
 	types-PyYAML
 	pylint
-	paho-mqtt~=1.5.0
-	pyyaml~=5.4.1
-	mqtt-entity
+	mqtt-entity==0.0.3
+	pysolarmanv5==3.0.0
+	pyyaml==6.0.1
 
 [isort]
 profile = black
 
 [flake8]
 extend-ignore = E203, E501, W503
```

### Comparing `sunsynk-0.3.7/sunsynk/definitions.py` & `sunsynk-0.4.0/sunsynk/definitions.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/definitions3ph.py` & `sunsynk-0.4.0/sunsynk/definitions3ph.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/helpers.py` & `sunsynk-0.4.0/sunsynk/helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/pysunsynk.py` & `sunsynk-0.4.0/sunsynk/pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/rwsensors.py` & `sunsynk-0.4.0/sunsynk/rwsensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/sensors.py` & `sunsynk-0.4.0/sunsynk/sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/state.py` & `sunsynk-0.4.0/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk/sunsynk.py` & `sunsynk-0.4.0/sunsynk/sunsynk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Sunsync Modbus interface."""
 import asyncio
 import logging
+import time
 from typing import Iterable, Sequence
 
 import attrs
 
 from sunsynk.helpers import patch_bitmask
 from sunsynk.rwsensors import RWSensor
 from sunsynk.sensors import Sensor, ValType
@@ -20,14 +21,15 @@
     state: InverterState = attrs.field(factory=InverterState)
     port: str = attrs.field(default="/dev/tty0")
     baudrate: int = attrs.field(default=9600)
     server_id: int = attrs.field(default=1)
     timeout: int = attrs.field(default=10)
     read_sensors_batch_size: int = attrs.field(default=60)
     timeouts: int = 0
+    allow_gap: int = 1
 
     async def connect(self) -> None:
         """Connect."""
         raise NotImplementedError
 
     async def write_register(self, *, address: int, value: int) -> bool:
         """Write to a register - Sunsynk support function code 0x10."""
@@ -75,21 +77,31 @@
         assert self.state is not None
         for sen in sensors:
             if sen not in self.state.values:
                 _LOGGER.warning("sensor %s not being tracked", sen.id)
 
         new_regs: dict[int, int] = {}
         for grp in group_sensors(
-            sensors, allow_gap=1, max_group_size=self.read_sensors_batch_size
+            sensors,
+            allow_gap=self.allow_gap,
+            max_group_size=self.read_sensors_batch_size,
         ):
             glen = grp[-1] - grp[0] + 1
             try:
+                perf = time.perf_counter()
                 r_r = await asyncio.wait_for(
                     self.read_holding_registers(grp[0], glen), timeout=self.timeout + 1
                 )
+                perf = time.perf_counter() - perf
+                _LOGGER.debug(
+                    "Time taken to fetch %s registers starting at %s : %ss",
+                    glen,
+                    grp[0],
+                    f"{perf:.2f}",
+                )
             except asyncio.TimeoutError:
                 _LOGGER.error("timeout reading register %s (%s)", grp[0], glen)
                 self.timeouts += 1
                 raise
             except Exception as err:  # pylint: disable=broad-except
                 raise Exception(  # pylint: disable=raise-missing-from,broad-exception-raised
                     f"({self.server_id},{grp[0]},{glen}) {err}"
```

### Comparing `sunsynk-0.3.7/sunsynk/usunsynk.py` & `sunsynk-0.4.0/sunsynk/usunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/sunsynk.egg-info/PKG-INFO` & `sunsynk-0.4.0/sunsynk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.7
+Version: 0.4.0
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.7/sunsynk.egg-info/SOURCES.txt` & `sunsynk-0.4.0/sunsynk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 sunsynk/__init__.py
 sunsynk/definitions.py
 sunsynk/definitions3ph.py
 sunsynk/helpers.py
 sunsynk/pysunsynk.py
 sunsynk/rwsensors.py
 sunsynk/sensors.py
+sunsynk/solarmansunsynk.py
 sunsynk/state.py
 sunsynk/sunsynk.py
 sunsynk/usunsynk.py
 sunsynk.egg-info/PKG-INFO
 sunsynk.egg-info/SOURCES.txt
 sunsynk.egg-info/dependency_links.txt
 sunsynk.egg-info/requires.txt
```

### Comparing `sunsynk-0.3.7/tests/conftest.py` & `sunsynk-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.4.0/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/hass-addon-sunsynk.zip` & `sunsynk-0.4.0/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_filter.py` & `sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_filter.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_run.py` & `sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_run.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_sensors.py` & `sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/hass_addon_sunsynk_multi/test_state.py` & `sunsynk-0.4.0/tests/hass_addon_sunsynk_multi/test_state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_helpers.py` & `sunsynk-0.4.0/tests/sunsynk/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_pysunsynk.py` & `sunsynk-0.4.0/tests/sunsynk/test_pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_register.py` & `sunsynk-0.4.0/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.4.0/tests/sunsynk/test_rwsensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_sensors.py` & `sunsynk-0.4.0/tests/sunsynk/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.4.0/tests/sunsynk/test_sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.7/tests/sunsynk/test_usunsynk.py` & `sunsynk-0.4.0/tests/sunsynk/test_usunsynk.py`

 * *Files identical despite different names*

