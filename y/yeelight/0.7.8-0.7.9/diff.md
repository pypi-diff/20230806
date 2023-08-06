# Comparing `tmp/yeelight-0.7.8.tar.gz` & `tmp/yeelight-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeelight-0.7.8.tar", last modified: Fri Oct 15 00:14:49 2021, max compression
+gzip compressed data, was "yeelight-0.7.9.tar", last modified: Sun Feb  6 17:46:26 2022, max compression
```

## Comparing `yeelight-0.7.8.tar` & `yeelight-0.7.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-15 00:14:49.230369 yeelight-0.7.8/
--rw-rw-rw-   0 root         (0) root         (0)     5562 2021-10-15 00:14:35.000000 yeelight-0.7.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1520 2021-10-15 00:14:35.000000 yeelight-0.7.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      237 2021-10-15 00:14:35.000000 yeelight-0.7.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8562 2021-10-15 00:14:49.230369 yeelight-0.7.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7840 2021-10-15 00:14:48.000000 yeelight-0.7.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-15 00:14:49.221362 yeelight-0.7.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6003 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-15 00:14:49.223364 yeelight-0.7.8/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-15 00:14:49.224365 yeelight-0.7.8/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     5530 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/source/_static/yeelight.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8993 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4239 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/source/flow.rst
--rw-rw-rw-   0 root         (0) root         (0)       12 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/source/genindex.rst
--rw-rw-rw-   0 root         (0) root         (0)     7799 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1380 2021-10-15 00:14:35.000000 yeelight-0.7.8/docs/source/yeelight.rst
--rw-rw-rw-   0 root         (0) root         (0)      960 2021-10-15 00:14:35.000000 yeelight-0.7.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      688 2021-10-15 00:14:49.231370 yeelight-0.7.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1209 2021-10-15 00:14:35.000000 yeelight-0.7.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-15 00:14:49.228368 yeelight-0.7.8/yeelight/
--rw-rw-rw-   0 root         (0) root         (0)      612 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21710 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/aio.py
--rw-rw-rw-   0 root         (0) root         (0)    16243 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     7081 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/flow.py
--rw-rw-rw-   0 root         (0) root         (0)    11063 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/flows.py
--rw-rw-rw-   0 root         (0) root         (0)    43359 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/main.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/ssdp_discover.py
--rw-rw-rw-   0 root         (0) root         (0)    16815 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     8136 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/transitions.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-10-15 00:14:35.000000 yeelight-0.7.8/yeelight/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-15 00:14:49.230369 yeelight-0.7.8/yeelight.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8562 2021-10-15 00:14:49.000000 yeelight-0.7.8/yeelight.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      651 2021-10-15 00:14:49.000000 yeelight-0.7.8/yeelight.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-15 00:14:49.000000 yeelight-0.7.8/yeelight.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2021-10-15 00:14:49.000000 yeelight-0.7.8/yeelight.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-10-15 00:14:49.000000 yeelight-0.7.8/yeelight.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-06 17:46:26.232775 yeelight-0.7.9/
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2022-02-06 17:46:11.000000 yeelight-0.7.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2022-02-06 17:46:11.000000 yeelight-0.7.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      237 2022-02-06 17:46:11.000000 yeelight-0.7.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8691 2022-02-06 17:46:26.232775 yeelight-0.7.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7929 2022-02-06 17:46:25.000000 yeelight-0.7.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-06 17:46:26.225441 yeelight-0.7.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6003 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-06 17:46:26.226358 yeelight-0.7.9/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-06 17:46:26.227275 yeelight-0.7.9/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     5530 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/source/_static/yeelight.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8993 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/source/flow.rst
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/source/genindex.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2022-02-06 17:46:11.000000 yeelight-0.7.9/docs/source/yeelight.rst
+-rw-rw-rw-   0 root         (0) root         (0)      960 2022-02-06 17:46:11.000000 yeelight-0.7.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      688 2022-02-06 17:46:26.232775 yeelight-0.7.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1290 2022-02-06 17:46:11.000000 yeelight-0.7.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-06 17:46:26.230942 yeelight-0.7.9/yeelight/
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26063 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    16300 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     7081 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/flow.py
+-rw-rw-rw-   0 root         (0) root         (0)    11063 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/flows.py
+-rw-rw-rw-   0 root         (0) root         (0)    43639 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/ssdp_discover.py
+-rw-rw-rw-   0 root         (0) root         (0)    16815 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8136 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/transitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-02-06 17:46:11.000000 yeelight-0.7.9/yeelight/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-06 17:46:26.231859 yeelight-0.7.9/yeelight.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8691 2022-02-06 17:46:26.000000 yeelight-0.7.9/yeelight.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      651 2022-02-06 17:46:26.000000 yeelight-0.7.9/yeelight.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-06 17:46:26.000000 yeelight-0.7.9/yeelight.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2022-02-06 17:46:26.000000 yeelight-0.7.9/yeelight.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-02-06 17:46:26.000000 yeelight-0.7.9/yeelight.egg-info/top_level.txt
```

### Comparing `yeelight-0.7.8/CHANGELOG.md` & `yeelight-0.7.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Changelog
 
 
 ## Unreleased
 
+### Features
+
+* Implement async music mode (closes #73) [Alex]
+
+
+## v0.7.8 (2021-10-15)
+
 ### Fixes
 
 * Use compact json commands. [J. Nick Koston]
 
 * Asyncio: Reconnect on protocol errors. [J. Nick Koston]
 
 * Reduce chance of overloading bulb. [J. Nick Koston]
```

### Comparing `yeelight-0.7.8/LICENSE` & `yeelight-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/PKG-INFO` & `yeelight-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeelight
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Python library for controlling YeeLight RGB bulbs.
 Home-page: https://gitlab.com/stavros/python-yeelight/
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Description
 ===========
 
 
 [![image](https://gitlab.com/stavros/python-yeelight/badges/master/pipeline.svg)](https://gitlab.com/stavros/python-yeelight/pipelines)
@@ -103,14 +104,21 @@
 -------
 
 `yeelight` is distributed under the BSD license.
 
 # Changelog
 
 
+## v0.7.9 (2022-02-06)
+
+### Features
+
+* Implement async music mode (closes #73) [Alex]
+
+
 ## v0.7.8 (2021-10-15)
 
 ### Fixes
 
 * Use compact json commands. [J. Nick Koston]
 
 * Asyncio: Reconnect on protocol errors. [J. Nick Koston]
```

### Comparing `yeelight-0.7.8/README.md` & `yeelight-0.7.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,21 @@
 -------
 
 `yeelight` is distributed under the BSD license.
 
 # Changelog
 
 
+## v0.7.9 (2022-02-06)
+
+### Features
+
+* Implement async music mode (closes #73) [Alex]
+
+
 ## v0.7.8 (2021-10-15)
 
 ### Fixes
 
 * Use compact json commands. [J. Nick Koston]
 
 * Asyncio: Reconnect on protocol errors. [J. Nick Koston]
```

### Comparing `yeelight-0.7.8/docs/Makefile` & `yeelight-0.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/docs/source/_static/yeelight.jpg` & `yeelight-0.7.9/docs/source/_static/yeelight.jpg`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/docs/source/conf.py` & `yeelight-0.7.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/docs/source/flow.rst` & `yeelight-0.7.9/docs/source/flow.rst`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/docs/source/index.rst` & `yeelight-0.7.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/docs/source/yeelight.rst` & `yeelight-0.7.9/docs/source/yeelight.rst`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/pyproject.toml` & `yeelight-0.7.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yeelight"
-version = "0.7.8"
+version = "0.7.9"
 
 [build-system]
 requires = ["flit_core >=2,<3"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "yeelight"
```

### Comparing `yeelight-0.7.8/setup.cfg` & `yeelight-0.7.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/setup.py` & `yeelight-0.7.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,20 @@
     name="yeelight",
     version=__version__,  # type: ignore
     author="Stavros Korokithakis",
     author_email="hi@stavros.io",
     url="https://gitlab.com/stavros/python-yeelight/",
     description="A Python library for controlling YeeLight RGB bulbs.",
     long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
     license="BSD",
     classifiers=classifiers,
     packages=["yeelight"],
     python_requires=">=3.4",
-    install_requires=["future", "ifaddr", 'pypiwin32;platform_system=="Windows"',],
+    install_requires=[
+        "future",
+        "ifaddr",
+        'pypiwin32;platform_system=="Windows"',
+    ],
     test_suite="yeelight.tests",
     tests_require=[],
 )
```

### Comparing `yeelight-0.7.8/yeelight/__init__.py` & `yeelight-0.7.9/yeelight/__init__.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/aio.py` & `yeelight-0.7.9/yeelight/aio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # encoding: utf8
 import asyncio
+import contextlib
 import json
 import logging
 import socket
 from typing import Dict
 
 from .enums import LightType
 from .main import _command_to_send_command
@@ -60,18 +61,25 @@
         self._async_listen_task = None
         self._async_reconnect_task = None
         self._async_writer = None
         self._async_reader = None
         self._async_cmd_id = 0
         self._async_command_lock = asyncio.Lock()
         self._socket_backoff = False
+        self._music_mode_params = None
 
     async def async_send_command(self, method, params):
         """Send a command to the bulb and wait for the result."""
         async with self._async_command_lock:
+            if self._music_mode:
+                await self._async_send_command(method, params, create_future=False)
+                # We can't check if it worked, so we just assume it did
+                if self._async_callback:
+                    self._async_callback({"result": ["ok"]})
+                return {"result": ["ok"]}
             future = await self._async_send_command(method, params)
             response = await asyncio.wait_for(future, TIMEOUT)
 
         if "error" in response:
             raise BulbException(response["error"])
 
         return response
@@ -103,15 +111,15 @@
     async def _async_run_listen(self):
         """Backend for async_listen."""
         _LOGGER.debug("%s: Starting listen task", self)
         while self._is_listening:
             try:
                 await self._async_connection_loop()
             finally:
-                self._async_close_reader_writer()
+                await self._async_close_reader_writer()
                 if self._async_callback:
                     self._async_callback({KEY_CONNECTED: False})
                 if self._is_listening:
                     await self._async_backoff()
                     await self._async_reconnect_loop()
 
     async def _async_reconnect_loop(self):
@@ -129,15 +137,21 @@
                 )
                 await asyncio.sleep(TIMEOUT)
             else:
                 _LOGGER.debug("%s: Reconnected successfully", self)
                 self._async_connected(writer, reader)
                 if self._async_callback:
                     self._async_callback({KEY_CONNECTED: True})
+                if self._music_mode:
+                    # Let user know we are no longer in music mode and try to re-enable it
+                    self._music_mode = False
+                    # Need to run this separately as starting music mode cancels this task
+                    asyncio.create_task(self.async_start_music(reconnect=True))
                 return
+
         _LOGGER.debug("%s: Reconnect loop stopped", self)
 
     async def _async_backoff(self):
         """Back off only if we had a previous failure without a success."""
         if self._socket_backoff:
             _LOGGER.debug("%s: Backing off %s seconds", self, TIMEOUT)
             await asyncio.sleep(TIMEOUT)
@@ -146,17 +160,21 @@
     async def _async_connection_loop(self) -> None:
         timeouts = 0
         ping_id = -1
         assert self._async_reader is not None
         while self._is_listening:
             try:
                 _LOGGER.debug("%s: Waiting for line", self)
-                line = await asyncio.wait_for(
-                    self._async_reader.readline(), PING_INTERVAL + TIMEOUT
-                )
+                # Don't expect a response in music mode
+                if self._music_mode:
+                    line = await self._async_reader.readline()
+                else:
+                    line = await asyncio.wait_for(
+                        self._async_reader.readline(), PING_INTERVAL + TIMEOUT
+                    )
             except asyncio.TimeoutError:
                 timeouts += 1
                 if timeouts == 2:
                     _LOGGER.debug("%s: Timeout waiting for line", self)
                     return
                 _LOGGER.debug(
                     "%s: No data in %s seconds, pinging bulb to make sure its still connected",
@@ -276,27 +294,31 @@
         self._async_callback({KEY_CONNECTED: True})
 
     def _async_stop_listen_task(self):
         if self._async_listen_task:
             self._async_listen_task.cancel()
             self._async_listen_task = None
 
-    def _async_close_reader_writer(self):
+    async def _async_close_reader_writer(self):
         self._async_pending_commands = {}
         if self._async_writer:
-            self._async_writer.close()
+            # Need to ignore socket errors if it was dropped
+            with contextlib.suppress(socket.error):
+                self._async_writer.close()
+                await self._async_writer.wait_closed()
             self._async_writer = None
         self._async_reader = None
 
-    async def async_stop_listening(self):
+    async def async_stop_listening(self, remove_callback=True):
         """Stop listening to notifications."""
         self._is_listening = False
         self._async_stop_listen_task()
-        self._async_close_reader_writer()
-        self._async_callback = None
+        await self._async_close_reader_writer()
+        if remove_callback:
+            self._async_callback = None
 
     async def async_get_properties(self, requested_properties=DEFAULT_PROPS):
         """
         Retrieve and return the properties of the bulb.
 
         This method also updates ``last_properties`` when it is called.
 
@@ -576,7 +598,88 @@
         Set the light power mode.
 
         If the light is off it will be turned on.
 
         :param yeelight.PowerMode mode: The mode to switch to.
         """
         return await self.async_turn_on(power_mode=mode)
+
+    async def async_start_music(self, port=0, ip=None, reconnect=False):
+        """
+        Start music mode.
+
+        Music mode essentially upgrades the existing connection to a reverse one
+        (the bulb connects to the library), removing all limits and allowing you
+        to send commands without being rate-limited.
+
+        Starting music mode will start a new listening socket, tell the bulb to
+        connect to that, and then close the old connection. If the bulb cannot
+        connect to the host machine for any reason, bad things will happen (such
+        as library freezes).
+
+        :param int port: The port to listen on. If none is specified, a random
+                         port will be chosen.
+
+        :param str ip: The IP address of the host this library is running on.
+                       Will be discovered automatically if not provided.
+        """
+        if reconnect:
+            # Music mode is enabled but we're not connected.
+            # Attempt to retrieve original parameters passed
+            port, ip = self._music_mode_params or (port, ip)
+        elif self._music_mode:
+            # Music mode is enabled and we're already connected.
+            raise AssertionError("Already in music mode, please stop music mode first.")
+
+        # Force populating the cache in case we are being called directly
+        # without ever fetching properties beforehand
+        await self.async_get_properties()
+        # await self.async_ensure_on()
+
+        future = asyncio.Future()
+        # The bulb doesn't send anything in music mode
+
+        def on_connect(reader, writer):
+            server.close()
+            future.set_result((reader, writer))
+
+        local_ip = ip if ip else self._socket.getsockname()[0]
+        server = await asyncio.start_server(
+            on_connect, local_ip, port, reuse_address=True
+        )
+        port = server.sockets[0].getsockname()[1]
+        await self.async_send_command("set_music", [1, local_ip, port])
+        await self.async_stop_listening(False)
+        reader, writer = await asyncio.wait_for(future, TIMEOUT)
+        self._async_writer = writer
+        self._async_reader = reader
+        # Manually enable listener to watch for disconnects
+        self._is_listening = True
+        self._async_listen_task = asyncio.ensure_future(self._async_run_listen())
+        # We are now connected
+        if self._async_callback:
+            self._async_callback({KEY_CONNECTED: True})
+
+        self._music_mode_params = (port, ip)
+        self._music_mode = True
+
+        if reconnect:
+            _LOGGER.debug("%s: Music mode reconnected successfully", self)
+
+        return "ok"
+
+    async def async_stop_music(self, **kwargs):
+        """
+        Stop music mode.
+
+        Stopping music mode will close the previous connection. Calling
+        ``stop_music`` more than once, or while not in music mode, is safe.
+        """
+        if not self._music_mode:
+            return
+
+        # flush out music mode socket
+        await self.async_stop_listening(False)
+
+        await self.async_listen(self._async_callback)
+        self._music_mode = False
+        return "set_music", [0], kwargs
```

### Comparing `yeelight-0.7.8/yeelight/decorator.py` & `yeelight-0.7.9/yeelight/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 if sys.version >= "3":
     from inspect import getfullargspec  # type: ignore
 
     def get_init(cls):
         return cls.__init__
 
-
 else:
 
     class getfullargspec(object):  # type: ignore
         "A quick and dirty replacement for getfullargspec for Python 2.X"
 
         def __init__(self, f):
             self.args, self.varargs, self.varkw, self.defaults = inspect.getargspec(f)
@@ -267,15 +266,19 @@
         # this is obsolete behavior; you should use decorate instead
         return decorate(_func, caller)
     # else return a decorator function
     if inspect.isclass(caller):
         name = caller.__name__.lower()
         doc = (
             "decorator(%s) converts functions/generators into "
-            "factories of %s objects" % (caller.__name__, caller.__name__,)
+            "factories of %s objects"
+            % (
+                caller.__name__,
+                caller.__name__,
+            )
         )
     elif inspect.isfunction(caller):
         if caller.__name__ == "<lambda>":
             name = "_lambda_"
         else:
             name = caller.__name__
         doc = caller.__doc__
```

### Comparing `yeelight-0.7.8/yeelight/enums.py` & `yeelight-0.7.9/yeelight/enums.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/flow.py` & `yeelight-0.7.9/yeelight/flow.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/flows.py` & `yeelight-0.7.9/yeelight/flows.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/main.py` & `yeelight-0.7.9/yeelight/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,14 +312,20 @@
                 self._last_properties["power"] = new_state
                 self._last_properties["bg_power"] = new_state
             elif method in action_property_map:
                 set_prop = action_property_map[method]
                 update_props = {
                     set_prop[prop]: params[prop] for prop in range(len(set_prop))
                 }
+                if "rgb" in method:
+                    update_props["color_mode"] = 1
+                elif "ct" in method:
+                    update_props["color_mode"] = 2
+                elif "hsv" in method:
+                    update_props["color_mode"] = 3
                 _LOGGER.debug("Music mode cache update: %s", update_props)
                 self._last_properties.update(update_props)
         # Add the effect parameters.
         params += [effect, duration]
         # Add power_mode parameter.
         if (
             method == "set_power"
@@ -695,15 +701,17 @@
             # Nightlight mode.
             cb = self._last_properties.get("nl_br")
         else:
             cb = self._last_properties.get("bright")
         self._last_properties["current_brightness"] = cb
 
     def get_properties(
-        self, requested_properties=DEFAULT_PROPS, ssdp_fallback=False,
+        self,
+        requested_properties=DEFAULT_PROPS,
+        ssdp_fallback=False,
     ):
         """
         Retrieve and return the properties of the bulb.
 
         This method also updates ``last_properties`` when it is called.
 
         The ``current_brightness`` property is calculated by the library (i.e. not returned
```

### Comparing `yeelight-0.7.8/yeelight/metadata.py` & `yeelight-0.7.9/yeelight/metadata.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/ssdp_discover.py` & `yeelight-0.7.9/yeelight/ssdp_discover.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/tests.py` & `yeelight-0.7.9/yeelight/tests.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/transitions.py` & `yeelight-0.7.9/yeelight/transitions.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight/utils.py` & `yeelight-0.7.9/yeelight/utils.py`

 * *Files identical despite different names*

### Comparing `yeelight-0.7.8/yeelight.egg-info/PKG-INFO` & `yeelight-0.7.9/yeelight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeelight
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Python library for controlling YeeLight RGB bulbs.
 Home-page: https://gitlab.com/stavros/python-yeelight/
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Description
 ===========
 
 
 [![image](https://gitlab.com/stavros/python-yeelight/badges/master/pipeline.svg)](https://gitlab.com/stavros/python-yeelight/pipelines)
@@ -103,14 +104,21 @@
 -------
 
 `yeelight` is distributed under the BSD license.
 
 # Changelog
 
 
+## v0.7.9 (2022-02-06)
+
+### Features
+
+* Implement async music mode (closes #73) [Alex]
+
+
 ## v0.7.8 (2021-10-15)
 
 ### Fixes
 
 * Use compact json commands. [J. Nick Koston]
 
 * Asyncio: Reconnect on protocol errors. [J. Nick Koston]
```

### Comparing `yeelight-0.7.8/yeelight.egg-info/SOURCES.txt` & `yeelight-0.7.9/yeelight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

