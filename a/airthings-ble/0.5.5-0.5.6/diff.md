# Comparing `tmp/airthings_ble-0.5.5.tar.gz` & `tmp/airthings_ble-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings_ble-0.5.5.tar", max compression
+gzip compressed data, was "airthings_ble-0.5.6.tar", max compression
```

## Comparing `airthings_ble-0.5.5.tar` & `airthings_ble-0.5.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-01-22 17:45:39.851641 airthings_ble-0.5.5/LICENSE
--rw-r--r--   0        0        0      113 2023-01-22 17:45:39.851641 airthings_ble-0.5.5/README.md
--rw-r--r--   0        0        0      235 2023-01-22 17:45:40.779712 airthings_ble-0.5.5/airthings_ble/__init__.py
--rw-r--r--   0        0        0     1917 2023-01-22 17:45:39.851641 airthings_ble-0.5.5/airthings_ble/const.py
--rw-r--r--   0        0        0    18260 2023-01-22 17:45:39.851641 airthings_ble-0.5.5/airthings_ble/parser.py
--rw-r--r--   0        0        0        0 2023-01-22 17:45:39.851641 airthings_ble-0.5.5/airthings_ble/py.typed
--rw-r--r--   0        0        0     2158 2023-01-22 17:45:40.807714 airthings_ble-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 airthings_ble-0.5.5/setup.py
--rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 airthings_ble-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/LICENSE
+-rw-r--r--   0        0        0      113 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/README.md
+-rw-r--r--   0        0        0      235 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/const.py
+-rw-r--r--   0        0        0    20993 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/py.typed
+-rw-r--r--   0        0        0     2159 2023-08-06 13:20:24.792241 airthings_ble-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 airthings_ble-0.5.6/PKG-INFO
```

### Comparing `airthings_ble-0.5.5/LICENSE` & `airthings_ble-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.5/airthings_ble/const.py` & `airthings_ble-0.5.6/airthings_ble/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,7 +40,19 @@
 """
 VERY_LOW = (0, 49, "very low")
 LOW = (50, 99, "low")
 MODERATE = (100, 299, "moderate")
 HIGH = (300, None, "high")
 
 BQ_TO_PCI_MULTIPLIER = 0.027
+
+CO2_MAX = 65534
+VOC_MAX = 65534
+HUMIDITY_MAX = 100
+RADON_MAX = 16383
+
+DEVICE_TYPE = {
+    "2900": "Wave gen. 1",
+    "2920": "Wave Mini",
+    "2930": "Wave Plus",
+    "2950": "Wave Radon",
+}
```

### Comparing `airthings_ble-0.5.5/airthings_ble/parser.py` & `airthings_ble-0.5.6/airthings_ble/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Parser for Airthings BLE devices"""
 
 from __future__ import annotations
 
 import asyncio
 import dataclasses
+import re
 import struct
 from collections import namedtuple
 from datetime import datetime
 from logging import Logger
 from math import exp
-from typing import Any, Callable, Tuple
+from typing import Any, Callable, Optional, Tuple
 
 from bleak import BleakClient, BleakError
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import establish_connection
 
 from .const import (
     BQ_TO_PCI_MULTIPLIER,
@@ -28,32 +29,35 @@
     CHAR_UUID_RADON_1DAYAVG,
     CHAR_UUID_RADON_LONG_TERM_AVG,
     CHAR_UUID_SERIAL_NUMBER_STRING,
     CHAR_UUID_TEMPERATURE,
     CHAR_UUID_WAVE_2_DATA,
     CHAR_UUID_WAVE_PLUS_DATA,
     CHAR_UUID_WAVEMINI_DATA,
+    CO2_MAX,
     COMMAND_UUID,
+    DEVICE_TYPE,
     HIGH,
+    HUMIDITY_MAX,
     LOW,
     MODERATE,
+    RADON_MAX,
     VERY_LOW,
+    VOC_MAX,
 )
 
 Characteristic = namedtuple("Characteristic", ["uuid", "name", "format"])
 
-manufacturer_characteristics = Characteristic(
-    CHAR_UUID_MANUFACTURER_NAME, "manufacturer", "utf-8"
-)
-device_info_characteristics = [
-    manufacturer_characteristics,
+wave_gen_1_device_info_characteristics = [
+    Characteristic(CHAR_UUID_MANUFACTURER_NAME, "manufacturer", "utf-8"),
     Characteristic(CHAR_UUID_SERIAL_NUMBER_STRING, "serial_nr", "utf-8"),
-    Characteristic(CHAR_UUID_MODEL_NUMBER_STRING, "model_nr", "utf-8"),
     Characteristic(CHAR_UUID_DEVICE_NAME, "device_name", "utf-8"),
     Characteristic(CHAR_UUID_FIRMWARE_REV, "firmware_rev", "utf-8"),
+]
+device_info_characteristics = wave_gen_1_device_info_characteristics + [
     Characteristic(CHAR_UUID_HARDWARE_REV, "hardware_rev", "utf-8"),
 ]
 
 sensors_characteristics_uuid = [
     CHAR_UUID_DATETIME,
     CHAR_UUID_TEMPERATURE,
     CHAR_UUID_HUMIDITY,
@@ -79,60 +83,64 @@
             res = val
         return {name: res}
 
     return handler
 
 
 def _decode_attr(
-    name: str, format_type: str, scale: float
+    name: str, format_type: str, scale: float, max_value: Optional[float] = None
 ) -> Callable[[bytearray], dict[str, float | None | str]]:
     """same as base decoder, but expects only one value.. for real"""
 
     def handler(raw_data: bytearray) -> dict[str, float | None | str]:
         val = struct.unpack(format_type, raw_data)
         res: float | None = None
         if len(val) == 1:
             res = val[0] * scale
+        if res is not None and max_value is not None:
+            # Verify that the result is not above the maximum allowed value
+            if res > max_value:
+                res = None
         data: dict[str, float | None | str] = {name: res}
         return data
 
     return handler
 
 
 def __decode_wave_plus(
     name: str, format_type: str, scale: float
 ) -> Callable[[bytearray], dict[str, float | None | str]]:
     def handler(raw_data: bytearray) -> dict[str, float | None | str]:
         vals = _decode_base(name, format_type, scale)(raw_data)
         val = vals[name]
         data: dict[str, float | None | str] = {}
         data["date_time"] = str(datetime.isoformat(datetime.now()))
-        data["humidity"] = val[1] / 2.0
-        data["radon_1day_avg"] = val[4] if 0 <= val[4] <= 16383 else None
-        data["radon_longterm_avg"] = val[5] if 0 <= val[5] <= 16383 else None
+        data["humidity"] = val[1] / 2.0 if 0 <= val[1] / 2.0 <= HUMIDITY_MAX else None
+        data["radon_1day_avg"] = val[4] if 0 <= val[4] <= RADON_MAX else None
+        data["radon_longterm_avg"] = val[5] if 0 <= val[5] <= RADON_MAX else None
         data["temperature"] = val[6] / 100.0
         data["rel_atm_pressure"] = val[7] / 50.0
-        data["co2"] = val[8] * 1.0
-        data["voc"] = val[9] * 1.0
+        data["co2"] = val[8] * 1.0 if 0 <= val[8] * 1.0 <= CO2_MAX else None
+        data["voc"] = val[9] * 1.0 if 0 <= val[9] * 1.0 <= VOC_MAX else None
         return data
 
     return handler
 
 
 def __decode_wave_2(
     name: str, format_type: str, scale: float
 ) -> Callable[[bytearray], dict[str, float | None | str]]:
     def handler(raw_data: bytearray) -> dict[str, float | None | str]:
         vals = _decode_base(name, format_type, scale)(raw_data)
         val = vals[name]
         data: dict[str, float | None | str] = {}
         data["date_time"] = str(datetime.isoformat(datetime.now()))
-        data["humidity"] = val[1] / 2.0
-        data["radon_1day_avg"] = val[4] if 0 <= val[4] <= 16383 else None
-        data["radon_longterm_avg"] = val[5] if 0 <= val[5] <= 16383 else None
+        data["humidity"] = val[1] / 2.0 if 0 <= val[1] / 2.0 <= HUMIDITY_MAX else None
+        data["radon_1day_avg"] = val[4] if 0 <= val[4] <= RADON_MAX else None
+        data["radon_longterm_avg"] = val[5] if 0 <= val[5] <= RADON_MAX else None
         data["temperature"] = val[6] / 100.0
         return data
 
     return handler
 
 
 def _decode_wave_mini(
@@ -140,16 +148,18 @@
 ) -> Callable[[bytearray], dict[str, float | None | str]]:
     def handler(raw_data: bytearray) -> dict[str, float | None | str]:
         vals = _decode_base(name, format_type, scale)(raw_data)
         val = vals[name]
         data: dict[str, float | None | str] = {}
         data["date_time"] = str(datetime.isoformat(datetime.now()))
         data["temperature"] = round(val[1] / 100.0 - 273.15, 2)
-        data["humidity"] = val[3] / 100.0
-        data["voc"] = val[4] * 1.0
+        data["humidity"] = (
+            val[3] / 100.0 if 0 <= val[3] / 100.0 <= HUMIDITY_MAX else None
+        )
+        data["voc"] = val[4] * 1.0 if 0 <= val[4] * 1.0 <= VOC_MAX else None
         return data
 
     return handler
 
 
 def _decode_wave(
     name: str, format_type: str, scale: float
@@ -260,15 +270,16 @@
             self.message += data
         if self._full_message_received():
             self._event.set()
 
     async def wait_for_message(self) -> None:
         """Waits until the full message is received.
 
-        If the full message has already been received, this method returns immediately."""
+        If the full message has already been received, this method returns immediately.
+        """
         if not self._full_message_received():
             await self._event.wait()
 
 
 def get_radon_level(data: float) -> str:
     """Returns the applicable radon level"""
     if data <= VERY_LOW[1]:
@@ -293,21 +304,24 @@
     h = elevation  # m
     offset = (p0 - (p0 * exp(-g * h * M / (T0 * R0)))) / 100.0  # mbar
     return data + round(offset, 2)
 
 
 sensor_decoders: dict[str, Callable[[bytearray], dict[str, float | None | str]],] = {
     str(CHAR_UUID_WAVE_PLUS_DATA): __decode_wave_plus(
-        name="Pluss", format_type="BBBBHHHHHHHH", scale=0
+        name="Plus", format_type="BBBBHHHHHHHH", scale=0
     ),
     str(CHAR_UUID_DATETIME): _decode_wave(
         name="date_time", format_type="HBBBBB", scale=0
     ),
     str(CHAR_UUID_HUMIDITY): _decode_attr(
-        name="humidity", format_type="H", scale=1.0 / 100.0
+        name="humidity",
+        format_type="H",
+        scale=1.0 / 100.0,
+        max_value=HUMIDITY_MAX,
     ),
     str(CHAR_UUID_RADON_1DAYAVG): _decode_attr(
         name="radon_1day_avg", format_type="H", scale=1.0
     ),
     str(CHAR_UUID_RADON_LONG_TERM_AVG): _decode_attr(
         name="radon_longterm_avg", format_type="H", scale=1.0
     ),
@@ -333,27 +347,36 @@
 
 
 def short_address(address: str) -> str:
     """Convert a Bluetooth address to a short address."""
     return address.replace("-", "").replace(":", "")[-6:].upper()
 
 
+# pylint: disable=too-many-instance-attributes
 @dataclasses.dataclass
 class AirthingsDevice:
     """Response data with information about the Airthings device"""
 
+    manufacturer: str = ""
     hw_version: str = ""
     sw_version: str = ""
+    model: Optional[str] = None
+    model_raw: str = ""
     name: str = ""
     identifier: str = ""
     address: str = ""
     sensors: dict[str, str | float | None] = dataclasses.field(
         default_factory=lambda: {}
     )
 
+    def friendly_name(self) -> str:
+        """Generate a name for the device."""
+
+        return f"Airthings {self.model}"
+
 
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-branches
 class AirthingsBluetoothDeviceData:
     """Data for Airthings BLE sensors."""
 
     def __init__(
@@ -368,38 +391,81 @@
         self.is_metric = is_metric
         self.elevation = elevation
         self.voltage = voltage
 
     async def _get_device_characteristics(
         self, client: BleakClient, device: AirthingsDevice
     ) -> AirthingsDevice:
-        # device.identifier = short_address(client.address)
         device.address = client.address
-        for characteristic in device_info_characteristics:
+
+        # We need to fetch model to determ what to fetch.
+        try:
+            data = await client.read_gatt_char(CHAR_UUID_MODEL_NUMBER_STRING)
+        except BleakError as err:
+            self.logger.debug("Get device characteristics exception: %s", err)
+            return device
+        device.model_raw = data.decode("utf-8")
+        device.model = DEVICE_TYPE.get(device.model_raw)
+
+        if device.model is None:
+            self.logger.debug(
+                "Could not map model number to model name, most likely an unsupported device: %s",
+                device.model_raw,
+            )
+
+        if device.model_raw == "2900":
+            characteristics = wave_gen_1_device_info_characteristics
+        else:
+            characteristics = device_info_characteristics
+
+        for characteristic in characteristics:
             try:
                 data = await client.read_gatt_char(characteristic.uuid)
             except BleakError as err:
                 self.logger.debug("Get device characteristics exception: %s", err)
                 continue
+            if characteristic.name == "manufacturer":
+                device.manufacturer = data.decode(characteristic.format)
             if characteristic.name == "hardware_rev":
                 device.hw_version = data.decode(characteristic.format)
-                continue
-            if characteristic.name == "firmware_rev":
+            elif characteristic.name == "firmware_rev":
                 device.sw_version = data.decode(characteristic.format)
-                continue
-            if characteristic.name == "device_name":
+            elif characteristic.name == "device_name":
                 device.name = data.decode(characteristic.format)
-            if characteristic.name == "serial_nr":
-                device.identifier = data.decode(characteristic.format)
+            elif characteristic.name == "serial_nr":
+                identifier = data.decode(characteristic.format)
+                # Some devices return `Serial Number` on Mac instead of the actual serial number.
+                if identifier != "Serial Number":
+                    device.identifier = identifier
+            else:
+                self.logger.debug(
+                    "Characteristics not handled: %s", characteristic.uuid
+                )
+
+        if (
+            device.model_raw == "2900"
+            and device.name != ""
+            and (device.identifier == "" or device.identifier is None)
+        ):
+            # For the Wave gen. 1 we need to fetch the identifier in the device name.
+            # Example: From `AT#123456-2900Radon` we need to fetch `123456`.
+            wave1_identifier = re.search(r"(?<=\#)[0-9]{1,6}", device.name)
+            if wave1_identifier is not None and len(wave1_identifier.group()) == 6:
+                device.identifier = wave1_identifier.group()
+
+        # In some cases the device name will be empty, for example when using a Mac.
+        if device.name == "":
+            device.name = device.friendly_name()
+
         return device
 
     async def _get_service_characteristics(
         self, client: BleakClient, device: AirthingsDevice
     ) -> AirthingsDevice:
-        svcs = await client.get_services()
+        svcs = client.services
         for service in svcs:
             for characteristic in service.characteristics:
                 if (
                     characteristic.uuid in sensors_characteristics_uuid_str
                     and str(characteristic.uuid) in sensor_decoders
                 ):
                     try:
```

### Comparing `airthings_ble-0.5.5/pyproject.toml` & `airthings_ble-0.5.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airthings-ble"
-version = "0.5.5"
+version = "v0.5.6"
 description = "Manage Airthings BLE devices"
 authors = ["Vincent Giorgi"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/vincegio/airthings-ble"
 documentation = "https://airthings-ble.readthedocs.io"
 classifiers = [
```

### Comparing `airthings_ble-0.5.5/PKG-INFO` & `airthings_ble-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airthings-ble
-Version: 0.5.5
+Version: 0.5.6
 Summary: Manage Airthings BLE devices
 Home-page: https://github.com/vincegio/airthings-ble
 License: Apache Software License 2.0
 Author: Vincent Giorgi
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

