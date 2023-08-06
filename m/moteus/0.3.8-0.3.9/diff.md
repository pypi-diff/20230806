# Comparing `tmp/moteus-0.3.8.tar.gz` & `tmp/moteus-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../bazel-out/k8-opt/bin/lib/python/moteus-0.3.8.tar", last modified: Sat Jan 23 22:08:11 2021, max compression
+gzip compressed data, was "../../bazel-out/k8-opt/bin/lib/python/moteus-0.3.9.tar", last modified: Sun Jan 24 21:56:15 2021, max compression
```

## Comparing `moteus-0.3.8.tar` & `moteus-0.3.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2021-01-23 22:08:11.565841 moteus-0.3.8/
--rw-r--r--   0 josh      (1000) josh      (1000)     4395 2021-01-23 22:08:11.565841 moteus-0.3.8/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)     2941 2021-01-12 01:53:04.000000 moteus-0.3.8/README.md
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2021-01-23 22:08:11.565841 moteus-0.3.8/moteus/
--rw-rw-r--   0 josh      (1000) josh      (1000)      721 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1061 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/aioserial.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2902 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/aiostream.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     8533 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/calibrate_encoder.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      735 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/command.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1518 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/export.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     5681 2021-01-23 22:06:29.000000 moteus-0.3.8/moteus/fdcanusb.py
--rw-rw-r--   0 josh      (1000) josh      (1000)    22892 2021-01-23 22:06:29.000000 moteus-0.3.8/moteus/moteus.py
--rw-rw-r--   0 josh      (1000) josh      (1000)    28091 2021-01-14 18:19:06.000000 moteus-0.3.8/moteus/moteus_tool.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     9579 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/multiplex.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2971 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/posix_aioserial.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2891 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/pythoncan.py
--rw-rw-r--   0 josh      (1000) josh      (1000)    11920 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/reader.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1183 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/regression.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2043 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/router.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1003 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/transport.py
--r-xr-xr-x   0 josh      (1000) josh      (1000)      608 2021-01-23 22:08:10.000000 moteus-0.3.8/moteus/version.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1841 2021-01-12 01:53:04.000000 moteus-0.3.8/moteus/win32_aioserial.py
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2021-01-23 22:08:11.565841 moteus-0.3.8/moteus.egg-info/
--rw-r--r--   0 josh      (1000) josh      (1000)     4395 2021-01-23 22:08:11.000000 moteus-0.3.8/moteus.egg-info/PKG-INFO
--rw-r--r--   0 josh      (1000) josh      (1000)      565 2021-01-23 22:08:11.000000 moteus-0.3.8/moteus.egg-info/SOURCES.txt
--rw-r--r--   0 josh      (1000) josh      (1000)        1 2021-01-23 22:08:11.000000 moteus-0.3.8/moteus.egg-info/dependency_links.txt
--rw-r--r--   0 josh      (1000) josh      (1000)       57 2021-01-23 22:08:11.000000 moteus-0.3.8/moteus.egg-info/entry_points.txt
--rw-r--r--   0 josh      (1000) josh      (1000)      107 2021-01-23 22:08:11.000000 moteus-0.3.8/moteus.egg-info/requires.txt
--rw-r--r--   0 josh      (1000) josh      (1000)        7 2021-01-23 22:08:11.000000 moteus-0.3.8/moteus.egg-info/top_level.txt
--rw-r--r--   0 josh      (1000) josh      (1000)       38 2021-01-23 22:08:11.565841 moteus-0.3.8/setup.cfg
--r-xr-xr-x   0 josh      (1000) josh      (1000)     1779 2021-01-23 22:08:10.000000 moteus-0.3.8/setup.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2021-01-24 21:56:15.836696 moteus-0.3.9/
+-rw-r--r--   0 josh      (1000) josh      (1000)     4395 2021-01-24 21:56:15.836696 moteus-0.3.9/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2941 2021-01-12 01:53:04.000000 moteus-0.3.9/README.md
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2021-01-24 21:56:15.836696 moteus-0.3.9/moteus/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      721 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/__init__.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1061 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/aioserial.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2902 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/aiostream.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     8533 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/calibrate_encoder.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)      735 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/command.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1518 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/export.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     5681 2021-01-23 22:06:29.000000 moteus-0.3.9/moteus/fdcanusb.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)    24608 2021-01-24 21:49:57.000000 moteus-0.3.9/moteus/moteus.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)    28091 2021-01-14 18:19:06.000000 moteus-0.3.9/moteus/moteus_tool.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     9579 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/multiplex.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2971 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/posix_aioserial.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2891 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/pythoncan.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)    11920 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/reader.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1183 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/regression.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     2043 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/router.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1003 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/transport.py
+-r-xr-xr-x   0 josh      (1000) josh      (1000)      608 2021-01-24 21:45:21.000000 moteus-0.3.9/moteus/version.py
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1841 2021-01-12 01:53:04.000000 moteus-0.3.9/moteus/win32_aioserial.py
+drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2021-01-24 21:56:15.836696 moteus-0.3.9/moteus.egg-info/
+-rw-r--r--   0 josh      (1000) josh      (1000)     4395 2021-01-24 21:56:15.000000 moteus-0.3.9/moteus.egg-info/PKG-INFO
+-rw-r--r--   0 josh      (1000) josh      (1000)      565 2021-01-24 21:56:15.000000 moteus-0.3.9/moteus.egg-info/SOURCES.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        1 2021-01-24 21:56:15.000000 moteus-0.3.9/moteus.egg-info/dependency_links.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       57 2021-01-24 21:56:15.000000 moteus-0.3.9/moteus.egg-info/entry_points.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)      107 2021-01-24 21:56:15.000000 moteus-0.3.9/moteus.egg-info/requires.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)        7 2021-01-24 21:56:15.000000 moteus-0.3.9/moteus.egg-info/top_level.txt
+-rw-r--r--   0 josh      (1000) josh      (1000)       38 2021-01-24 21:56:15.836696 moteus-0.3.9/setup.cfg
+-r-xr-xr-x   0 josh      (1000) josh      (1000)     1779 2021-01-24 21:45:21.000000 moteus-0.3.9/setup.py
```

### Comparing `moteus-0.3.8/PKG-INFO` & `moteus-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moteus
-Version: 0.3.8
+Version: 0.3.9
 Summary: moteus brushless controller library and tools
 Home-page: https://github.com/mjbots/pi3hat
 Author: mjbots Robotic Systems
 Author-email: info@mjbots.com
 License: UNKNOWN
 Description: # Python bindings for moteus brushless controller #
```

### Comparing `moteus-0.3.8/README.md` & `moteus-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/__init__.py` & `moteus-0.3.9/moteus/__init__.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/aioserial.py` & `moteus-0.3.9/moteus/aioserial.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/aiostream.py` & `moteus-0.3.9/moteus/aiostream.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/calibrate_encoder.py` & `moteus-0.3.9/moteus/calibrate_encoder.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/command.py` & `moteus-0.3.9/moteus/command.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/export.py` & `moteus-0.3.9/moteus/export.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/fdcanusb.py` & `moteus-0.3.9/moteus/fdcanusb.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/moteus.py` & `moteus-0.3.9/moteus/moteus.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,19 @@
     kp_scale = mp.F32
     kd_scale = mp.F32
     maximum_torque = mp.F32
     stop_position = mp.F32
     watchdog_timeout = mp.F32
 
 
+class CurrentResolution:
+    d_A = mp.F32
+    q_A = mp.F32
+
+
 class Parser(mp.RegisterParser):
     def read_position(self, resolution):
         return self.read_mapped(resolution, 0.01, 0.0001, 0.00001)
 
     def read_velocity(self, resolution):
         return self.read_mapped(resolution, 0.1, 0.00025, 0.00001)
 
@@ -276,14 +281,17 @@
 
     def write_temperature(self, value, resolution):
         self.write_mapped(value, 1.0, 0.1, 0.001, resolution)
 
     def write_time(self, value, resolution):
         self.write_mapped(value, 0.01, 0.001, 0.000001, resolution)
 
+    def write_current(self, value, resolution):
+        self.write_mapped(value, 1.0, 0.1, 0.001, resolution)
+
 
 def parse_register(parser, register, resolution):
     if register == Register.MODE:
         return parser.read_int(resolution)
     elif register == Register.POSITION:
         return parser.read_position(resolution)
     elif register == Register.VELOCITY:
@@ -382,18 +390,20 @@
       position_resolution: an instance of moteus.PositionResolution
       transport: something modeling moteus.Transport to send commands through
     """
 
     def __init__(self, id=1,
                  query_resolution=QueryResolution(),
                  position_resolution=PositionResolution(),
+                 current_resolution=CurrentResolution(),
                  transport=None):
         self.id = id
         self.query_resolution = query_resolution
         self.position_resolution = position_resolution
+        self.current_resolution = current_resolution
         self.transport = transport
         self._parser = make_parser(id)
         self._diagnostic_parser = make_diagnostic_parser(id)
 
         # Pre-compute our query string.
         self._query_data = self._make_query_data()
 
@@ -565,14 +575,59 @@
 
         return result
 
     async def set_position(self, *args, **kwargs):
         return self._extract(await self._get_transport().cycle(
             [self.make_position(**kwargs)]))
 
+    def make_current(self,
+                     *,
+                     d_A,
+                     q_A,
+                     query=False):
+        """Return a moteus.Command structure with data necessary to send a
+        current mode command.
+        """
+
+        result = self._make_command(query=query)
+        cr = self.current_resolution
+        resolutions = [
+            cr.d_A if d_A is not None else mp.IGNORE,
+            cr.q_A if q_A is not None else mp.IGNORE,
+        ]
+
+        data_buf = io.BytesIO()
+
+        writer = Writer(data_buf)
+        writer.write_int8(mp.WRITE_INT8 | 0x01)
+        writer.write_int8(int(Register.MODE))
+        writer.write_int8(int(Mode.CURRENT))
+
+        # Yes, annoyingly the register mapping as of version 4 still
+        # has the Q current first in this grouping, unlike everywhere
+        # else where D current is first.
+        combiner = mp.WriteCombiner(
+            writer, 0x00, int(Register.COMMAND_Q_CURRENT), resolutions)
+
+        if combiner.maybe_write():
+            writer.write_current(q_A, cr.q_A)
+        if combiner.maybe_write():
+            writer.write_current(d_A, cr.d_A)
+
+        if query:
+            data_buf.write(self._query_data)
+
+        result.data = data_buf.getvalue()
+
+        return result
+
+    async def set_current(self, *args, **kwargs):
+        return self._extract(await self._get_transport().cycle(
+            [self.make_current(**kwargs)]))
+
     def make_diagnostic_write(self, data):
         result = self._make_command(query=False)
 
         # CAN-FD frames can be at most 64 bytes long
         assert len(data) <= 61
 
         data_buf = io.BytesIO()
```

### Comparing `moteus-0.3.8/moteus/moteus_tool.py` & `moteus-0.3.9/moteus/moteus_tool.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/multiplex.py` & `moteus-0.3.9/moteus/multiplex.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/posix_aioserial.py` & `moteus-0.3.9/moteus/posix_aioserial.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/pythoncan.py` & `moteus-0.3.9/moteus/pythoncan.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/reader.py` & `moteus-0.3.9/moteus/reader.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/regression.py` & `moteus-0.3.9/moteus/regression.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/router.py` & `moteus-0.3.9/moteus/router.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/transport.py` & `moteus-0.3.9/moteus/transport.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus/version.py` & `moteus-0.3.9/moteus/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION="0.3.8"
+VERSION="0.3.9"
```

### Comparing `moteus-0.3.8/moteus/win32_aioserial.py` & `moteus-0.3.9/moteus/win32_aioserial.py`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/moteus.egg-info/PKG-INFO` & `moteus-0.3.9/moteus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moteus
-Version: 0.3.8
+Version: 0.3.9
 Summary: moteus brushless controller library and tools
 Home-page: https://github.com/mjbots/pi3hat
 Author: mjbots Robotic Systems
 Author-email: info@mjbots.com
 License: UNKNOWN
 Description: # Python bindings for moteus brushless controller #
```

### Comparing `moteus-0.3.8/moteus.egg-info/SOURCES.txt` & `moteus-0.3.9/moteus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moteus-0.3.8/setup.py` & `moteus-0.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setuptools.setup(
     name = 'moteus',
-    version = "0.3.8",
+    version = "0.3.9",
     description = 'moteus brushless controller library and tools',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/mjbots/pi3hat',
     author = 'mjbots Robotic Systems',
     author_email = 'info@mjbots.com',
     classifiers = [
```

