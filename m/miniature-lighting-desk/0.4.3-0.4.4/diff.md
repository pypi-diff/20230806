# Comparing `tmp/miniature_lighting_desk-0.4.3.tar.gz` & `tmp/miniature_lighting_desk-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniature_lighting_desk-0.4.3.tar", max compression
+gzip compressed data, was "miniature_lighting_desk-0.4.4.tar", max compression
```

## Comparing `miniature_lighting_desk-0.4.3.tar` & `miniature_lighting_desk-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.3/LICENSE
--rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.3/miniature_lighting_desk/__init__.py
--rw-r--r--   0        0        0    10974 2023-07-18 21:08:07.596413 miniature_lighting_desk-0.4.3/miniature_lighting_desk/async_hal.py
--rw-r--r--   0        0        0     3583 2023-07-18 21:17:53.179741 miniature_lighting_desk-0.4.3/miniature_lighting_desk/cli.py
--rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.4.3/miniature_lighting_desk/local_gui.py
--rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.4.3/miniature_lighting_desk/server.py
--rw-r--r--   0        0        0      833 2023-07-18 21:18:15.303074 miniature_lighting_desk-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-27 05:22:03.406650 miniature_lighting_desk-0.4.4/LICENSE
+-rw-r--r--   0        0        0       43 2023-07-27 05:22:03.406650 miniature_lighting_desk-0.4.4/miniature_lighting_desk/__init__.py
+-rw-r--r--   0        0        0    11485 2023-08-06 14:21:10.999995 miniature_lighting_desk-0.4.4/miniature_lighting_desk/async_hal.py
+-rw-r--r--   0        0        0     3595 2023-08-06 11:44:37.789976 miniature_lighting_desk-0.4.4/miniature_lighting_desk/cli.py
+-rw-r--r--   0        0        0     3035 2023-08-06 11:43:17.753312 miniature_lighting_desk-0.4.4/miniature_lighting_desk/local_gui.py
+-rw-r--r--   0        0        0     4404 2023-07-27 05:22:03.406650 miniature_lighting_desk-0.4.4/miniature_lighting_desk/server.py
+-rw-r--r--   0        0        0      833 2023-08-06 14:24:57.233321 miniature_lighting_desk-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.4.4/PKG-INFO
```

### Comparing `miniature_lighting_desk-0.4.3/LICENSE` & `miniature_lighting_desk-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.4.3/miniature_lighting_desk/async_hal.py` & `miniature_lighting_desk-0.4.4/miniature_lighting_desk/async_hal.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,34 +112,47 @@
 
 class FreqencyMixin:
     @abstractmethod
     def frequency(self, frequency_hz: "int | None" = None):
         """Get or set pwm frequency."""
 
 
-class MockController(ControllerABC):
+class MockController(WifiControllerABC, FreqencyMixin):
     def __init__(self, *args, no_channels=8, **kwargs):
         self.no_channels = no_channels
         self.vals = [0] * no_channels
         self.max_brightness = 100
         super().__init__(*args, **kwargs)
+        self._wifi = {}
+        self._frequency = 10_000
 
     async def _async_set_brightness(
         self, channel: int, brightness: int, pause: float = 0
     ) -> None:
         self.vals[channel] = brightness
         print(f"Setting channel {channel} to {brightness}")
         await asyncio.sleep(pause)
 
     async def _async_get_brightness(self, channel: int) -> int:
         print(f"Getting brightness for channel {channel}")
         return self.vals[channel]
 
     scale_brightness = unscale_brightness = lambda s, x: x
 
+    def wifi(self, ssid: str, password: str) -> dict:
+        self._wifi = dict(ssid=ssid, password=password)
+
+    def wifi_status(self) -> dict:
+        return self._wifi
+
+    def frequency(self, frequency_hz: "int | None" = None):
+        if frequency_hz:
+            self._frequency = frequency_hz
+        return self._frequency
+
 
 class PinguinoController(ControllerABC):
     def __init__(self, *args, timeout=100, **kwargs):
         VENDOR = 0x04D8
         PRODUCT = 0xFEAA
         CONFIGURATION = 0x01
         # find pinguino
@@ -201,19 +214,22 @@
     def unscale_brightness(self, scaled: int) -> int:
         return self.max_brightness - scaled
 
 
 class SerialRpcController(WifiControllerABC, FreqencyMixin):
     def __init__(self, *args, port="/dev/ttyUSB0", **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self.serial = AioSerial(port=port, baudrate=460800)
-        self.lock = asyncio.Lock()
+        self.submit_async(partial(self.init, port=port), block=True)
         self.no_channels = self.sync_call("channel_count")
         self.max_brightness = self.sync_call("max_brightness")
 
+    async def init(self, port):
+        self.serial = AioSerial(port=port, baudrate=460800)
+        self.lock = asyncio.Lock()
+
     def sync_call(self, method: str, **kwargs):
         future = self.submit_async(partial(self.call, method, **kwargs), block=True)
         return future.result()
 
     async def call(self, method: str, **kwargs):
         async with self.lock:  # dunno, might be needed...
             cmd = request_json(method, params=kwargs).encode()
```

### Comparing `miniature_lighting_desk-0.4.3/miniature_lighting_desk/cli.py` & `miniature_lighting_desk-0.4.4/miniature_lighting_desk/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 # Typer provides proper hinting like this
 _Controller = Enum("_Controller", {k: k for k in controllers.keys()})
 
 
 @app.command(help="Run local gui.")
 def local_gui(
-    controller: _Controller = _Controller.pinguino,
+    controller: _Controller = _Controller.pinguino.value,
     port: str = "",
 ):
     from .local_gui import main as gui
 
     kwargs = {"port": port} if port else {}
     controller = controllers[controller.value](**kwargs)
     gui(controller)
 
 
 @app.command(help="Run backend for web gui.")
 def backend(
-    controller: _Controller = _Controller.pinguino,
+    controller: _Controller = _Controller.pinguino.value,
     password: str = "",
     port: str = "",
 ):
     password = password or os.getenv("PASSWORD") or getpass("Enter Password: ")
     kwargs = {"port": port} if port else {}
     controller = controllers[controller.value](**kwargs)
     server.main(password, controller)
```

### Comparing `miniature_lighting_desk-0.4.3/miniature_lighting_desk/local_gui.py` & `miniature_lighting_desk-0.4.4/miniature_lighting_desk/local_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             filetypes=[("State CSV", "*.csv")],
             defaultextension=".csv",
         ) as f:
             reader = csv.reader(f)
             for row in reader:
                 states = row  # we just take the last row
 
-        if len(states) != 8:
+        if len(states) != self.lighting_controller.no_channels:
             print("Input file is corrupt.")  # we should use a dialog box for this.
 
         try:
             for i, state in enumerate(states):
                 self.channels[i].set(state)
         except Exception as e:
             print(f"Error loading state: {e}")
```

### Comparing `miniature_lighting_desk-0.4.3/miniature_lighting_desk/server.py` & `miniature_lighting_desk-0.4.4/miniature_lighting_desk/server.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.4.3/pyproject.toml` & `miniature_lighting_desk-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniature-lighting-desk"
-version = "0.4.3"
+version = "0.4.4"
 description = "Desk software for Miniature Lighting Controller"
 authors = ["John Maximilian <2e0byo@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyusb = "^1.2.1"
```

### Comparing `miniature_lighting_desk-0.4.3/PKG-INFO` & `miniature_lighting_desk-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniature-lighting-desk
-Version: 0.4.3
+Version: 0.4.4
 Summary: Desk software for Miniature Lighting Controller
 License: MIT
 Author: John Maximilian
 Author-email: 2e0byo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

