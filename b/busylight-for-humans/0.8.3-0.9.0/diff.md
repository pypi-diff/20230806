# Comparing `tmp/busylight-for-humans-0.8.3.tar.gz` & `tmp/busylight-for-humans-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busylight-for-humans-0.8.3.tar", last modified: Thu Mar 25 14:22:07 2021, max compression
+gzip compressed data, was "busylight-for-humans-0.9.0.tar", last modified: Sat Apr 10 01:10:22 2021, max compression
```

## Comparing `busylight-for-humans-0.8.3.tar` & `busylight-for-humans-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     5809 2021-01-20 04:25:20.268595 busylight-for-humans-0.8.3/README.md
--rw-r--r--   0        0        0        8 2020-08-08 20:59:21.275315 busylight-for-humans-0.8.3/busylight/__init__.py
--rw-r--r--   0        0        0     8940 2021-01-17 18:23:03.554257 busylight-for-humans-0.8.3/busylight/__main__.py
--rw-r--r--   0        0        0       22 2021-03-25 14:21:52.190209 busylight-for-humans-0.8.3/busylight/__version__.py
--rw-r--r--   0        0        0    12768 2021-01-11 02:14:20.789739 busylight-for-humans-0.8.3/busylight/api/__init__.py
--rw-r--r--   0        0        0      509 2020-11-19 18:56:58.149621 busylight-for-humans-0.8.3/busylight/api/models.py
--rw-r--r--   0        0        0     3037 2021-01-11 02:14:20.790699 busylight-for-humans-0.8.3/busylight/color.py
--rw-r--r--   0        0        0     5609 2021-01-11 02:14:20.791413 busylight-for-humans-0.8.3/busylight/effects/__init__.py
--rw-r--r--   0        0        0      736 2021-01-11 02:14:20.792050 busylight-for-humans-0.8.3/busylight/effects/gradient.py
--rw-r--r--   0        0        0     1037 2021-01-11 02:14:20.793463 busylight-for-humans-0.8.3/busylight/effects/spectrum.py
--rw-r--r--   0        0        0      940 2021-01-01 21:40:21.154332 busylight-for-humans-0.8.3/busylight/lights/README.md
--rw-r--r--   0        0        0      663 2021-01-01 00:15:10.419765 busylight-for-humans-0.8.3/busylight/lights/__init__.py
--rw-r--r--   0        0        0       77 2021-01-03 16:11:23.447577 busylight-for-humans-0.8.3/busylight/lights/agile_innovations/__init__.py
--rw-r--r--   0        0        0     1562 2021-01-11 02:14:20.794224 busylight-for-humans-0.8.3/busylight/lights/agile_innovations/blinkstick.py
--rw-r--r--   0        0        0    13280 2021-01-11 02:14:20.794945 busylight-for-humans-0.8.3/busylight/lights/agile_innovations/dataframe.py
--rw-r--r--   0        0        0     2585 2021-01-11 02:14:20.797218 busylight-for-humans-0.8.3/busylight/lights/agile_innovations/hardware.py
--rw-r--r--   0        0        0       70 2021-01-01 00:15:10.421037 busylight-for-humans-0.8.3/busylight/lights/embrava/__init__.py
--rw-r--r--   0        0        0     1960 2021-03-25 14:19:29.010814 busylight-for-humans-0.8.3/busylight/lights/embrava/blynclight.py
--rw-r--r--   0        0        0     2657 2021-01-01 00:15:10.421433 busylight-for-humans-0.8.3/busylight/lights/embrava/hardware.py
--rw-r--r--   0        0        0      490 2021-01-01 00:15:10.421620 busylight-for-humans-0.8.3/busylight/lights/exceptions.py
--rw-r--r--   0        0        0       74 2021-01-01 00:15:10.421847 busylight-for-humans-0.8.3/busylight/lights/kuando/__init__.py
--rw-r--r--   0        0        0     2988 2021-01-11 02:14:20.799462 busylight-for-humans-0.8.3/busylight/lights/kuando/busylight.py
--rw-r--r--   0        0        0     4745 2021-01-11 02:14:20.801603 busylight-for-humans-0.8.3/busylight/lights/kuando/hardware.py
--rw-r--r--   0        0        0       52 2021-01-01 00:15:10.422557 busylight-for-humans-0.8.3/busylight/lights/luxafor/__init__.py
--rw-r--r--   0        0        0     1647 2021-01-11 02:14:20.802215 busylight-for-humans-0.8.3/busylight/lights/luxafor/flag.py
--rw-r--r--   0        0        0     4334 2021-01-11 02:14:20.804128 busylight-for-humans-0.8.3/busylight/lights/luxafor/hardware.py
--rw-r--r--   0        0        0      816 2021-01-01 21:23:16.845204 busylight-for-humans-0.8.3/busylight/lights/statevector.py
--rw-r--r--   0        0        0       58 2021-01-01 00:15:10.425295 busylight-for-humans-0.8.3/busylight/lights/thingm/__init__.py
--rw-r--r--   0        0        0     3862 2021-01-11 02:14:20.805603 busylight-for-humans-0.8.3/busylight/lights/thingm/blink1.py
--rw-r--r--   0        0        0     4111 2021-01-11 02:14:20.806590 busylight-for-humans-0.8.3/busylight/lights/thingm/hardware.py
--rw-r--r--   0        0        0     2021 2021-01-11 02:14:20.806950 busylight-for-humans-0.8.3/busylight/lights/thread.py
--rw-r--r--   0        0        0    17114 2021-01-11 02:14:20.807943 busylight-for-humans-0.8.3/busylight/lights/usblight.py
--rw-r--r--   0        0        0     8787 2021-01-11 02:14:20.808607 busylight-for-humans-0.8.3/busylight/manager.py
--rw-r--r--   0        0        0     1080 2021-03-25 14:21:52.127642 busylight-for-humans-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     7230 2021-03-25 14:22:07.488246 busylight-for-humans-0.8.3/setup.py
--rw-r--r--   0        0        0     6763 2021-03-25 14:22:07.488862 busylight-for-humans-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     6064 2021-04-10 01:08:42.560624 busylight-for-humans-0.9.0/README.md
+-rw-r--r--   0        0        0        8 2020-08-08 20:59:21.275315 busylight-for-humans-0.9.0/busylight/__init__.py
+-rw-r--r--   0        0        0     8940 2021-01-17 18:23:03.554257 busylight-for-humans-0.9.0/busylight/__main__.py
+-rw-r--r--   0        0        0       22 2021-04-10 01:10:19.864528 busylight-for-humans-0.9.0/busylight/__version__.py
+-rw-r--r--   0        0        0    12768 2021-01-11 02:14:20.789739 busylight-for-humans-0.9.0/busylight/api/__init__.py
+-rw-r--r--   0        0        0      509 2020-11-19 18:56:58.149621 busylight-for-humans-0.9.0/busylight/api/models.py
+-rw-r--r--   0        0        0     3037 2021-01-11 02:14:20.790699 busylight-for-humans-0.9.0/busylight/color.py
+-rw-r--r--   0        0        0     5609 2021-01-11 02:14:20.791413 busylight-for-humans-0.9.0/busylight/effects/__init__.py
+-rw-r--r--   0        0        0      736 2021-01-11 02:14:20.792050 busylight-for-humans-0.9.0/busylight/effects/gradient.py
+-rw-r--r--   0        0        0     1037 2021-01-11 02:14:20.793463 busylight-for-humans-0.9.0/busylight/effects/spectrum.py
+-rw-r--r--   0        0        0      940 2021-01-01 21:40:21.154332 busylight-for-humans-0.9.0/busylight/lights/README.md
+-rw-r--r--   0        0        0      681 2021-04-10 00:42:01.519509 busylight-for-humans-0.9.0/busylight/lights/__init__.py
+-rw-r--r--   0        0        0       77 2021-01-03 16:11:23.447577 busylight-for-humans-0.9.0/busylight/lights/agile_innovations/__init__.py
+-rw-r--r--   0        0        0     1562 2021-01-11 02:14:20.794224 busylight-for-humans-0.9.0/busylight/lights/agile_innovations/blinkstick.py
+-rw-r--r--   0        0        0    13280 2021-01-11 02:14:20.794945 busylight-for-humans-0.9.0/busylight/lights/agile_innovations/dataframe.py
+-rw-r--r--   0        0        0     2585 2021-01-11 02:14:20.797218 busylight-for-humans-0.9.0/busylight/lights/agile_innovations/hardware.py
+-rw-r--r--   0        0        0      137 2021-04-10 00:47:34.044225 busylight-for-humans-0.9.0/busylight/lights/embrava/__init__.py
+-rw-r--r--   0        0        0     1952 2021-04-10 01:00:24.205058 busylight-for-humans-0.9.0/busylight/lights/embrava/blynclight.py
+-rw-r--r--   0        0        0     2657 2021-01-01 00:15:10.421433 busylight-for-humans-0.9.0/busylight/lights/embrava/hardware.py
+-rw-r--r--   0        0        0     2323 2021-04-10 00:49:56.247899 busylight-for-humans-0.9.0/busylight/lights/embrava/status_indicator.py
+-rw-r--r--   0        0        0      490 2021-01-01 00:15:10.421620 busylight-for-humans-0.9.0/busylight/lights/exceptions.py
+-rw-r--r--   0        0        0       74 2021-01-01 00:15:10.421847 busylight-for-humans-0.9.0/busylight/lights/kuando/__init__.py
+-rw-r--r--   0        0        0     2988 2021-01-11 02:14:20.799462 busylight-for-humans-0.9.0/busylight/lights/kuando/busylight.py
+-rw-r--r--   0        0        0     4745 2021-01-11 02:14:20.801603 busylight-for-humans-0.9.0/busylight/lights/kuando/hardware.py
+-rw-r--r--   0        0        0       52 2021-01-01 00:15:10.422557 busylight-for-humans-0.9.0/busylight/lights/luxafor/__init__.py
+-rw-r--r--   0        0        0     1647 2021-01-11 02:14:20.802215 busylight-for-humans-0.9.0/busylight/lights/luxafor/flag.py
+-rw-r--r--   0        0        0     4334 2021-01-11 02:14:20.804128 busylight-for-humans-0.9.0/busylight/lights/luxafor/hardware.py
+-rw-r--r--   0        0        0      816 2021-01-01 21:23:16.845204 busylight-for-humans-0.9.0/busylight/lights/statevector.py
+-rw-r--r--   0        0        0       58 2021-01-01 00:15:10.425295 busylight-for-humans-0.9.0/busylight/lights/thingm/__init__.py
+-rw-r--r--   0        0        0     3862 2021-01-11 02:14:20.805603 busylight-for-humans-0.9.0/busylight/lights/thingm/blink1.py
+-rw-r--r--   0        0        0     4111 2021-01-11 02:14:20.806590 busylight-for-humans-0.9.0/busylight/lights/thingm/hardware.py
+-rw-r--r--   0        0        0     2021 2021-01-11 02:14:20.806950 busylight-for-humans-0.9.0/busylight/lights/thread.py
+-rw-r--r--   0        0        0    17114 2021-01-11 02:14:20.807943 busylight-for-humans-0.9.0/busylight/lights/usblight.py
+-rw-r--r--   0        0        0     8787 2021-01-11 02:14:20.808607 busylight-for-humans-0.9.0/busylight/manager.py
+-rw-r--r--   0        0        0     1080 2021-04-10 01:10:19.817535 busylight-for-humans-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7492 2021-04-10 01:10:22.693080 busylight-for-humans-0.9.0/setup.py
+-rw-r--r--   0        0        0     7018 2021-04-10 01:10:22.693806 busylight-for-humans-0.9.0/PKG-INFO
```

### Comparing `busylight-for-humans-0.8.3/README.md` & `busylight-for-humans-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,42 +19,48 @@
 <em>Back to Front, Left to Right</em> <br>
 <b>BlyncLight, BlyncLight Plus, Busylight</b> <br>
 <b>Blink(1), Flag, BlinkStick</b>
 
 ## Features
 - Control lights from the [command-line][HELP].
 - Control lights via a [Web API][WEBAPI].
-- Individually addresable lights.
-- Supports Five Vendors & Multiple Models:
+- Import `busylight` into your own project.
+- Supports Six Vendors & Multiple Models:
   * [**Agile Innovations** BlinkStick ][2]
   * [**Embrava** Blynclight][3]
   * [**Kuando** BusyLight][4]
   * [**Luxafor** Flag][5]
+  * [**Plantronics** Status Indicator][3]
   * [**ThingM** Blink1][6]
 - Works on MacOS, Linux, probably Windows and BSD too!
 - Tested extensively on Raspberry Pi 3b+, Zero W and 4
 
-If you have a USB light that's not on this list, please open
-an issue with the make and model device you want supported.
+If you have a USB light that's not on this list open an issue
+with the make and model device you want supported, where I can get
+one, and any public hardware documentation you are aware of.
 
-## Basic Install 
+## Basic Install
+
+Installs only the command-line `busylight` tool and associated
+modules.
 
 ```console
 $ python3 -m pip install busylight-for-humans 
 ```
 
 ## Web API Install
 
 Installs `uvicorn` and `FastAPI` in addition to `busylight`:
 
 ```console
 $ python3 -m pip install busylight-for-humans[webapi]
 ```
 
 ## Linux Post-Install Activities
+
 Linux controls access to USB devices via the [udev subsystem][UDEV]. By
 default it denies non-root users access to devices it doesn't
 recognize. I've got you covered!
 
 You'll need root access to configure the udev rules:
 
 ```console
@@ -136,14 +142,15 @@
     "action": "effect",
     "name": "rainbow"
   }
 ```
 
 ## Code Examples
 
+Adding light support to your own python applications is easy!
 
 ### Simple Case: Turn On a Single Light
 
 In this example, we pick an Embrava Blynclight to activate with
 the color white. 
 
 ```python
```

### Comparing `busylight-for-humans-0.8.3/busylight/__main__.py` & `busylight-for-humans-0.9.0/busylight/__main__.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/api/__init__.py` & `busylight-for-humans-0.9.0/busylight/api/__init__.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/color.py` & `busylight-for-humans-0.9.0/busylight/color.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/effects/__init__.py` & `busylight-for-humans-0.9.0/busylight/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/effects/gradient.py` & `busylight-for-humans-0.9.0/busylight/effects/gradient.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/effects/spectrum.py` & `busylight-for-humans-0.9.0/busylight/effects/spectrum.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/README.md` & `busylight-for-humans-0.9.0/busylight/lights/README.md`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/__init__.py` & `busylight-for-humans-0.9.0/busylight/lights/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .exceptions import USBLightUnknownProduct
 from .exceptions import USBLightInUse
 from .exceptions import USBLightIOError
 
 # EJO some kind of cool dynamic import would be sweet right here
 
 from .agile_innovations import BlinkStick
-from .embrava import Blynclight
+from .embrava import Blynclight, Status_Indicator
 from .kuando import BusyLight
 from .luxafor import Flag
 from .thingm import Blink1
 
 __all__ = [
     "USBLight",
     "USBLightNotFound",
```

### Comparing `busylight-for-humans-0.8.3/busylight/lights/agile_innovations/blinkstick.py` & `busylight-for-humans-0.9.0/busylight/lights/agile_innovations/blinkstick.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/agile_innovations/dataframe.py` & `busylight-for-humans-0.9.0/busylight/lights/agile_innovations/dataframe.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/agile_innovations/hardware.py` & `busylight-for-humans-0.9.0/busylight/lights/agile_innovations/hardware.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/embrava/blynclight.py` & `busylight-for-humans-0.9.0/busylight/lights/embrava/blynclight.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ..usblight import USBLight
 
 
 class Blynclight(USBLight):
     """Embrava Blynclight family of USB-connected presence lights."""
 
-    VENDOR_IDS: List[int] = [0x2C0D, 0x03E5, 0x047f]
+    VENDOR_IDS: List[int] = [0x2C0D, 0x03E5]
     PRODUCT_IDS: List[int] = []
     vendor = "Embrava"
 
     @property
     def state(self) -> BlynclightState:
         """Implementation dependent hardware state."""
         try:
```

### Comparing `busylight-for-humans-0.8.3/busylight/lights/embrava/hardware.py` & `busylight-for-humans-0.9.0/busylight/lights/embrava/hardware.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/kuando/busylight.py` & `busylight-for-humans-0.9.0/busylight/lights/kuando/busylight.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/kuando/hardware.py` & `busylight-for-humans-0.9.0/busylight/lights/kuando/hardware.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/luxafor/flag.py` & `busylight-for-humans-0.9.0/busylight/lights/luxafor/flag.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/luxafor/hardware.py` & `busylight-for-humans-0.9.0/busylight/lights/luxafor/hardware.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/statevector.py` & `busylight-for-humans-0.9.0/busylight/lights/statevector.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/thingm/blink1.py` & `busylight-for-humans-0.9.0/busylight/lights/thingm/blink1.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/thingm/hardware.py` & `busylight-for-humans-0.9.0/busylight/lights/thingm/hardware.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/thread.py` & `busylight-for-humans-0.9.0/busylight/lights/thread.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/lights/usblight.py` & `busylight-for-humans-0.9.0/busylight/lights/usblight.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/busylight/manager.py` & `busylight-for-humans-0.9.0/busylight/manager.py`

 * *Files identical despite different names*

### Comparing `busylight-for-humans-0.8.3/pyproject.toml` & `busylight-for-humans-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "busylight-for-humans"
-version = "0.8.3"
+version = "0.9.0"
 description = "Control USB connected LED lights, like a human."
 authors = ["JnyJny <erik.oshaughnessy@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/JnyJny/busylight.git"
 packages = [ {include = "busylight"} ]
```

### Comparing `busylight-for-humans-0.8.3/setup.py` & `busylight-for-humans-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 {'webapi': ['uvicorn>=0.12.2,<0.14.0', 'fastapi>=0.61.1,<0.64.0']}
 
 entry_points = \
 {'console_scripts': ['busylight = busylight.__main__:cli']}
 
 setup_kwargs = {
     'name': 'busylight-for-humans',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'Control USB connected LED lights, like a human.',
-    'long_description': '<!-- USB HID API embrava blynclight agile innovations blinkstick kuando busylight luxafor flag thingM blink(1) -->\n![BusyLight Project Logo][LOGO]\n\n![version][pypi-version]\n![dependencies][dependencies]\n![pytest][pytest-action]\n![license][license]\n![monthly-downloads][monthly-downloads]\n![Code style: black][code-style-black]\n\n[BusyLight for Humans™][0] gives you control of USB attached LED\nlights from a variety of vendors. Lights can be controlled via\nthe command-line, using a HTTP API or imported directly into your own\npython project.\n\n![All Supported Lights][DEMO]\n\n**Six Lights Attached to One Host**<br>\n<em>Back to Front, Left to Right</em> <br>\n<b>BlyncLight, BlyncLight Plus, Busylight</b> <br>\n<b>Blink(1), Flag, BlinkStick</b>\n\n## Features\n- Control lights from the [command-line][HELP].\n- Control lights via a [Web API][WEBAPI].\n- Individually addresable lights.\n- Supports Five Vendors & Multiple Models:\n  * [**Agile Innovations** BlinkStick ][2]\n  * [**Embrava** Blynclight][3]\n  * [**Kuando** BusyLight][4]\n  * [**Luxafor** Flag][5]\n  * [**ThingM** Blink1][6]\n- Works on MacOS, Linux, probably Windows and BSD too!\n- Tested extensively on Raspberry Pi 3b+, Zero W and 4\n\nIf you have a USB light that\'s not on this list, please open\nan issue with the make and model device you want supported.\n\n## Basic Install \n\n```console\n$ python3 -m pip install busylight-for-humans \n```\n\n## Web API Install\n\nInstalls `uvicorn` and `FastAPI` in addition to `busylight`:\n\n```console\n$ python3 -m pip install busylight-for-humans[webapi]\n```\n\n## Linux Post-Install Activities\nLinux controls access to USB devices via the [udev subsystem][UDEV]. By\ndefault it denies non-root users access to devices it doesn\'t\nrecognize. I\'ve got you covered!\n\nYou\'ll need root access to configure the udev rules:\n\n```console\n$ busylight udev-rules -o 99-busylights.rules\n$ sudo cp 99-busylights.rules /etc/udev/rules.d\n$ sudo udevadm control -R\n$ # unplug/plug your light\n$ busylight on\n```\n\n## Command-Line Examples\n\n```console\n$ busylight on               # light turns on green\n$ busylight on red           # now it\'s shining a friendly red\n$ busylight on 0xff0000      # still red\n$ busylight on #00ff00       # now it\'s blue!\n$ busylight blink            # it\'s slowly blinking on and off with a red color\n$ busylight blink green fast # blinking faster green and off\n$ busylight --all on         # turn all lights on green\n$ busylight --all off        # turn all lights off\n```\n\n## HTTP API Examples\n\nFirst start the `busylight` API server:\n```console\n$ busylight serve\nINFO:     Started server process [20189]\nINFO:     Waiting for application startup.\nINFO:     Application startup complete.\nINFO:     Uvicorn running on http://0.0.0.0:8888 (Press CTRL+C to quit)\n```\n\nThe API is fully documented and available @ `https://localhost:8888/redoc`\n\n\nNow you can use the web API endpoints which return JSON payloads:\n\n```console\n  $ curl -s http://localhost:8888/1/lights\n  ...\n  $ curl -s http://localhost:8888/1/lights/on | jq\n  {\n    "light_id": 0,\n    "action": "on",\n    "color": "green"\n  }\n  $ curl -s http://localhost:8888/1/lights/off | jq\n  {\n    "light_id": 0,\n    "action": "off"\n  }\n  $ curl -s http://localhost:8888/1/light/0/on/purple | jq\n  {\n    "light_id": 0,\n    "action": "on",\n    "color": "purple"\n  }\n  $ curl -s http://localhost:8888/1/light/0/off | jq\n  {\n    "light_id": 0,\n    "action": "off"\n  }\n  $ curl -s http://localhost:8888/1/lights/on | jq\n  {\n    "light_id": "all",\n    "action": "on",\n    "color": "green"\n  }\n  $ curl -s http://localhost:8888/1/lights/off | jq\n  {\n    "light_id": "all",\n    "action": "off"\n  }\n  $ curl -s http://localhost:8888/1/lights/rainbow | jq\n  {\n    "light_id": "all",\n    "action": "effect",\n    "name": "rainbow"\n  }\n```\n\n## Code Examples\n\n\n### Simple Case: Turn On a Single Light\n\nIn this example, we pick an Embrava Blynclight to activate with\nthe color white. \n\n```python\nfrom busylight.lights.embrava import Blynclight\n\nlight = Blynclight.first_light()\n\nlight.on((255, 255, 255))\n```\n\n### Slightly More Complicated\n\nThe `busylight` package includes a manager class that great for\nworking with multiple lights or lights that require a little\nmore direct intervention like the Kuando Busylight series.\n\n```python\nfrom busylight.manager import LightManager, ALL_LIGHTS\nfrom busylight.effects import rainbow\n\nmanager = LightManager()\nfor light in manager.lights:\n   print(light.name)\n\nmanager.apply_effect_to_light(ALL_LIGHTS, rainbow)\n...\nmanager.lights_off(ALL_LIGHTS)\n```\n\n[0]: https://pypi.org/project/busylight-for-humans/\n\n<!-- doc links -->\n[2]: https://github.com/JnyJny/busylight/blob/master/docs/devices/agile_innovations.md\n[3]: https://github.com/JnyJny/busylight/blob/master/docs/devices/embrava.md\n[4]: https://github.com/JnyJny/busylight/blob/master/docs/devices/kuando.md\n[5]: https://github.com/JnyJny/busylight/blob/master/docs/devices/luxafor.md\n[6]: https://github.com/JnyJny/busylight/blob/master/docs/devices/thingm.md\n\n[LOGO]: https://github.com/JnyJny/busylight/blob/master/docs/assets/BusyLightLogo.png\n[HELP]: https://github.com/JnyJny/busylight/blob/master/docs/busylight.1.md\n[WEBAPI]: https://github.com/JnyJny/busylight/blob/master/docs/busylight_api.pdf\n[DEMO]: https://github.com/JnyJny/busylight/raw/master/demo/demo.gif\n\n[UDEV]: https://en.wikipedia.org/wiki/Udev\n\n<!-- badges -->\n[pytest-action]: https://github.com/JnyJny/busylight/workflows/pytest/badge.svg\n[code-style-black]: https://img.shields.io/badge/code%20style-black-000000.svg\n[pypi-version]: https://img.shields.io/pypi/v/busylight-for-humans\n[license]: https://img.shields.io/pypi/l/busylight-for-humans\n[dependencies]: https://img.shields.io/librariesio/github/JnyJny/busylight\n[monthly-downloads]: https://img.shields.io/pypi/dm/busylight-for-humans\n',
+    'long_description': '<!-- USB HID API embrava blynclight agile innovations blinkstick kuando busylight luxafor flag thingM blink(1) -->\n![BusyLight Project Logo][LOGO]\n\n![version][pypi-version]\n![dependencies][dependencies]\n![pytest][pytest-action]\n![license][license]\n![monthly-downloads][monthly-downloads]\n![Code style: black][code-style-black]\n\n[BusyLight for Humans™][0] gives you control of USB attached LED\nlights from a variety of vendors. Lights can be controlled via\nthe command-line, using a HTTP API or imported directly into your own\npython project.\n\n![All Supported Lights][DEMO]\n\n**Six Lights Attached to One Host**<br>\n<em>Back to Front, Left to Right</em> <br>\n<b>BlyncLight, BlyncLight Plus, Busylight</b> <br>\n<b>Blink(1), Flag, BlinkStick</b>\n\n## Features\n- Control lights from the [command-line][HELP].\n- Control lights via a [Web API][WEBAPI].\n- Import `busylight` into your own project.\n- Supports Six Vendors & Multiple Models:\n  * [**Agile Innovations** BlinkStick ][2]\n  * [**Embrava** Blynclight][3]\n  * [**Kuando** BusyLight][4]\n  * [**Luxafor** Flag][5]\n  * [**Plantronics** Status Indicator][3]\n  * [**ThingM** Blink1][6]\n- Works on MacOS, Linux, probably Windows and BSD too!\n- Tested extensively on Raspberry Pi 3b+, Zero W and 4\n\nIf you have a USB light that\'s not on this list open an issue\nwith the make and model device you want supported, where I can get\none, and any public hardware documentation you are aware of.\n\n## Basic Install\n\nInstalls only the command-line `busylight` tool and associated\nmodules.\n\n```console\n$ python3 -m pip install busylight-for-humans \n```\n\n## Web API Install\n\nInstalls `uvicorn` and `FastAPI` in addition to `busylight`:\n\n```console\n$ python3 -m pip install busylight-for-humans[webapi]\n```\n\n## Linux Post-Install Activities\n\nLinux controls access to USB devices via the [udev subsystem][UDEV]. By\ndefault it denies non-root users access to devices it doesn\'t\nrecognize. I\'ve got you covered!\n\nYou\'ll need root access to configure the udev rules:\n\n```console\n$ busylight udev-rules -o 99-busylights.rules\n$ sudo cp 99-busylights.rules /etc/udev/rules.d\n$ sudo udevadm control -R\n$ # unplug/plug your light\n$ busylight on\n```\n\n## Command-Line Examples\n\n```console\n$ busylight on               # light turns on green\n$ busylight on red           # now it\'s shining a friendly red\n$ busylight on 0xff0000      # still red\n$ busylight on #00ff00       # now it\'s blue!\n$ busylight blink            # it\'s slowly blinking on and off with a red color\n$ busylight blink green fast # blinking faster green and off\n$ busylight --all on         # turn all lights on green\n$ busylight --all off        # turn all lights off\n```\n\n## HTTP API Examples\n\nFirst start the `busylight` API server:\n```console\n$ busylight serve\nINFO:     Started server process [20189]\nINFO:     Waiting for application startup.\nINFO:     Application startup complete.\nINFO:     Uvicorn running on http://0.0.0.0:8888 (Press CTRL+C to quit)\n```\n\nThe API is fully documented and available @ `https://localhost:8888/redoc`\n\n\nNow you can use the web API endpoints which return JSON payloads:\n\n```console\n  $ curl -s http://localhost:8888/1/lights\n  ...\n  $ curl -s http://localhost:8888/1/lights/on | jq\n  {\n    "light_id": 0,\n    "action": "on",\n    "color": "green"\n  }\n  $ curl -s http://localhost:8888/1/lights/off | jq\n  {\n    "light_id": 0,\n    "action": "off"\n  }\n  $ curl -s http://localhost:8888/1/light/0/on/purple | jq\n  {\n    "light_id": 0,\n    "action": "on",\n    "color": "purple"\n  }\n  $ curl -s http://localhost:8888/1/light/0/off | jq\n  {\n    "light_id": 0,\n    "action": "off"\n  }\n  $ curl -s http://localhost:8888/1/lights/on | jq\n  {\n    "light_id": "all",\n    "action": "on",\n    "color": "green"\n  }\n  $ curl -s http://localhost:8888/1/lights/off | jq\n  {\n    "light_id": "all",\n    "action": "off"\n  }\n  $ curl -s http://localhost:8888/1/lights/rainbow | jq\n  {\n    "light_id": "all",\n    "action": "effect",\n    "name": "rainbow"\n  }\n```\n\n## Code Examples\n\nAdding light support to your own python applications is easy!\n\n### Simple Case: Turn On a Single Light\n\nIn this example, we pick an Embrava Blynclight to activate with\nthe color white. \n\n```python\nfrom busylight.lights.embrava import Blynclight\n\nlight = Blynclight.first_light()\n\nlight.on((255, 255, 255))\n```\n\n### Slightly More Complicated\n\nThe `busylight` package includes a manager class that great for\nworking with multiple lights or lights that require a little\nmore direct intervention like the Kuando Busylight series.\n\n```python\nfrom busylight.manager import LightManager, ALL_LIGHTS\nfrom busylight.effects import rainbow\n\nmanager = LightManager()\nfor light in manager.lights:\n   print(light.name)\n\nmanager.apply_effect_to_light(ALL_LIGHTS, rainbow)\n...\nmanager.lights_off(ALL_LIGHTS)\n```\n\n[0]: https://pypi.org/project/busylight-for-humans/\n\n<!-- doc links -->\n[2]: https://github.com/JnyJny/busylight/blob/master/docs/devices/agile_innovations.md\n[3]: https://github.com/JnyJny/busylight/blob/master/docs/devices/embrava.md\n[4]: https://github.com/JnyJny/busylight/blob/master/docs/devices/kuando.md\n[5]: https://github.com/JnyJny/busylight/blob/master/docs/devices/luxafor.md\n[6]: https://github.com/JnyJny/busylight/blob/master/docs/devices/thingm.md\n\n[LOGO]: https://github.com/JnyJny/busylight/blob/master/docs/assets/BusyLightLogo.png\n[HELP]: https://github.com/JnyJny/busylight/blob/master/docs/busylight.1.md\n[WEBAPI]: https://github.com/JnyJny/busylight/blob/master/docs/busylight_api.pdf\n[DEMO]: https://github.com/JnyJny/busylight/raw/master/demo/demo.gif\n\n[UDEV]: https://en.wikipedia.org/wiki/Udev\n\n<!-- badges -->\n[pytest-action]: https://github.com/JnyJny/busylight/workflows/pytest/badge.svg\n[code-style-black]: https://img.shields.io/badge/code%20style-black-000000.svg\n[pypi-version]: https://img.shields.io/pypi/v/busylight-for-humans\n[license]: https://img.shields.io/pypi/l/busylight-for-humans\n[dependencies]: https://img.shields.io/librariesio/github/JnyJny/busylight\n[monthly-downloads]: https://img.shields.io/pypi/dm/busylight-for-humans\n',
     'author': 'JnyJny',
     'author_email': 'erik.oshaughnessy@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/JnyJny/busylight.git',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `busylight-for-humans-0.8.3/PKG-INFO` & `busylight-for-humans-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busylight-for-humans
-Version: 0.8.3
+Version: 0.9.0
 Summary: Control USB connected LED lights, like a human.
 Home-page: https://github.com/JnyJny/busylight.git
 License: Apache-2.0
 Author: JnyJny
 Author-email: erik.oshaughnessy@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -43,42 +43,48 @@
 <em>Back to Front, Left to Right</em> <br>
 <b>BlyncLight, BlyncLight Plus, Busylight</b> <br>
 <b>Blink(1), Flag, BlinkStick</b>
 
 ## Features
 - Control lights from the [command-line][HELP].
 - Control lights via a [Web API][WEBAPI].
-- Individually addresable lights.
-- Supports Five Vendors & Multiple Models:
+- Import `busylight` into your own project.
+- Supports Six Vendors & Multiple Models:
   * [**Agile Innovations** BlinkStick ][2]
   * [**Embrava** Blynclight][3]
   * [**Kuando** BusyLight][4]
   * [**Luxafor** Flag][5]
+  * [**Plantronics** Status Indicator][3]
   * [**ThingM** Blink1][6]
 - Works on MacOS, Linux, probably Windows and BSD too!
 - Tested extensively on Raspberry Pi 3b+, Zero W and 4
 
-If you have a USB light that's not on this list, please open
-an issue with the make and model device you want supported.
+If you have a USB light that's not on this list open an issue
+with the make and model device you want supported, where I can get
+one, and any public hardware documentation you are aware of.
 
-## Basic Install 
+## Basic Install
+
+Installs only the command-line `busylight` tool and associated
+modules.
 
 ```console
 $ python3 -m pip install busylight-for-humans 
 ```
 
 ## Web API Install
 
 Installs `uvicorn` and `FastAPI` in addition to `busylight`:
 
 ```console
 $ python3 -m pip install busylight-for-humans[webapi]
 ```
 
 ## Linux Post-Install Activities
+
 Linux controls access to USB devices via the [udev subsystem][UDEV]. By
 default it denies non-root users access to devices it doesn't
 recognize. I've got you covered!
 
 You'll need root access to configure the udev rules:
 
 ```console
@@ -160,14 +166,15 @@
     "action": "effect",
     "name": "rainbow"
   }
 ```
 
 ## Code Examples
 
+Adding light support to your own python applications is easy!
 
 ### Simple Case: Turn On a Single Light
 
 In this example, we pick an Embrava Blynclight to activate with
 the color white. 
 
 ```python
```

