# Comparing `tmp/pyoverkiz-1.9.0.tar.gz` & `tmp/pyoverkiz-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverkiz-1.9.0.tar", max compression
+gzip compressed data, was "pyoverkiz-1.9.1.tar", max compression
```

## Comparing `pyoverkiz-1.9.0.tar` & `pyoverkiz-1.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-27 17:33:31.662286 pyoverkiz-1.9.0/LICENSE
--rw-r--r--   0        0        0     3319 2023-06-27 17:33:31.662286 pyoverkiz-1.9.0/README.md
--rw-r--r--   0        0        0        0 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/__init__.py
--rw-r--r--   0        0        0    31865 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/client.py
--rw-r--r--   0        0        0     4183 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/const.py
--rw-r--r--   0        0        0      242 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/__init__.py
--rw-r--r--   0        0        0     8866 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/command.py
--rw-r--r--   0        0        0     1888 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/execution.py
--rw-r--r--   0        0        0     2945 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/gateway.py
--rw-r--r--   0        0        0    17241 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/general.py
--rw-r--r--   0        0        0     2141 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/measured_value_type.py
--rw-r--r--   0        0        0     1052 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/protocol.py
--rw-r--r--   0        0        0      645 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/server.py
--rw-r--r--   0        0        0    14019 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/state.py
--rw-r--r--   0        0        0    18346 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/enums/ui.py
--rw-r--r--   0        0        0     1774 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/exceptions.py
--rw-r--r--   0        0        0    24495 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/models.py
--rw-r--r--   0        0        0     1869 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/obfuscate.py
--rw-r--r--   0        0        0        0 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/py.typed
--rw-r--r--   0        0        0      518 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/types.py
--rw-r--r--   0        0        0      824 2023-06-27 17:33:31.678287 pyoverkiz-1.9.0/pyoverkiz/utils.py
--rw-r--r--   0        0        0      987 2023-06-27 17:33:55.635128 pyoverkiz-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-09 11:54:15.698381 pyoverkiz-1.9.1/LICENSE
+-rw-r--r--   0        0        0     3319 2023-07-09 11:54:15.698381 pyoverkiz-1.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/__init__.py
+-rw-r--r--   0        0        0    33927 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/client.py
+-rw-r--r--   0        0        0     4183 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/const.py
+-rw-r--r--   0        0        0      242 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/__init__.py
+-rw-r--r--   0        0        0     8866 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/command.py
+-rw-r--r--   0        0        0     1888 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/execution.py
+-rw-r--r--   0        0        0     2945 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/gateway.py
+-rw-r--r--   0        0        0    17241 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/general.py
+-rw-r--r--   0        0        0     2141 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/measured_value_type.py
+-rw-r--r--   0        0        0     1052 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/protocol.py
+-rw-r--r--   0        0        0      645 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/server.py
+-rw-r--r--   0        0        0    14019 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/state.py
+-rw-r--r--   0        0        0    18346 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/enums/ui.py
+-rw-r--r--   0        0        0     1774 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/exceptions.py
+-rw-r--r--   0        0        0    25266 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/models.py
+-rw-r--r--   0        0        0     1869 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/obfuscate.py
+-rw-r--r--   0        0        0        0 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/py.typed
+-rw-r--r--   0        0        0      518 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/types.py
+-rw-r--r--   0        0        0      824 2023-07-09 11:54:15.710381 pyoverkiz-1.9.1/pyoverkiz/utils.py
+-rw-r--r--   0        0        0      987 2023-07-09 11:54:30.778485 pyoverkiz-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 pyoverkiz-1.9.1/PKG-INFO
```

### Comparing `pyoverkiz-1.9.0/LICENSE` & `pyoverkiz-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/README.md` & `pyoverkiz-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/client.py` & `pyoverkiz-1.9.1/pyoverkiz/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     Command,
     Device,
     Event,
     Execution,
     Gateway,
     HistoryExecution,
     LocalToken,
+    Option,
+    OptionParameter,
     OverkizServer,
     Place,
     Scenario,
     Setup,
     State,
 )
 from pyoverkiz.obfuscate import obfuscate_sensitive_data
@@ -754,14 +756,72 @@
         on_backoff=relogin,
     )
     async def execute_scheduled_scenario(self, oid: str, timestamp: int) -> str:
         """Execute a scheduled scenario"""
         response = await self.__post(f"exec/schedule/{oid}/{timestamp}")
         return cast(str, response["triggerId"])
 
+    @backoff.on_exception(
+        backoff.expo,
+        (NotAuthenticatedException, ServerDisconnectedError),
+        max_tries=2,
+        on_backoff=relogin,
+    )
+    async def get_setup_options(self) -> list[Option]:
+        """
+        This operation returns all subscribed options of a given setup.
+        Per-session rate-limit : 1 calls per 1d period for this particular operation (bulk-load)
+        Access scope : Full enduser API access (enduser/*)
+        """
+        response = await self.__get("setup/options")
+        options = [Option(**o) for o in humps.decamelize(response)]
+
+        return options
+
+    @backoff.on_exception(
+        backoff.expo,
+        (NotAuthenticatedException, ServerDisconnectedError),
+        max_tries=2,
+        on_backoff=relogin,
+    )
+    async def get_setup_option(self, option: str) -> Option | None:
+        """
+        This operation returns the selected subscribed option of a given setup.
+        For example `developerMode-{gateway_id}` to understand if developer mode is on.
+        """
+        response = await self.__get(f"setup/options/{option}")
+
+        if response:
+            return Option(**humps.decamelize(response))
+
+        return None
+
+    @backoff.on_exception(
+        backoff.expo,
+        (NotAuthenticatedException, ServerDisconnectedError),
+        max_tries=2,
+        on_backoff=relogin,
+    )
+    async def get_setup_option_parameter(
+        self, option: str, parameter: str
+    ) -> OptionParameter | None:
+        """
+        This operation returns the selected parameters of a given setup and option.
+        For example `developerMode-{gateway_id}` and `gatewayId` to understand if developer mode is on.
+
+        If the option is not available, an OverkizException will be thrown.
+        If the parameter is not available you will receive None.
+        """
+        response = await self.__get(f"setup/options/{option}/{parameter}")
+
+        if response:
+            return OptionParameter(**humps.decamelize(response))
+
+        return None
+
     async def __get(self, path: str) -> Any:
         """Make a GET request to the OverKiz API"""
         headers = {}
 
         await self._refresh_token_if_expired()
         if self._access_token:
             headers["Authorization"] = f"Bearer {self._access_token}"
```

### Comparing `pyoverkiz-1.9.0/pyoverkiz/const.py` & `pyoverkiz-1.9.1/pyoverkiz/const.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/command.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/command.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/execution.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/execution.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/gateway.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/gateway.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/general.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/general.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/measured_value_type.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/measured_value_type.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/protocol.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/protocol.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/server.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/server.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/state.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/state.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/enums/ui.py` & `pyoverkiz-1.9.1/pyoverkiz/enums/ui.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/exceptions.py` & `pyoverkiz-1.9.1/pyoverkiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/models.py` & `pyoverkiz-1.9.1/pyoverkiz/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,15 +217,14 @@
             self.widget = UIWidget(widget)
         elif self.definition.widget_name:
             self.widget = UIWidget(self.definition.widget_name)
 
 
 @define(init=False, kw_only=True)
 class StateDefinition:
-
     qualified_name: str
     type: str | None = None
     values: list[str] | None = None
 
     def __init__(
         self,
         name: str | None = None,
@@ -793,7 +792,40 @@
 class LocalToken:
     label: str
     gateway_id: str = field(repr=obfuscate_id, default=None)
     expiration_time: int
     gateway_creation_time: int
     uuid: str
     scope: str
+
+
+@define(kw_only=True)
+class OptionParameter:
+    name: str
+    value: str
+
+
+@define(init=False, kw_only=True)
+class Option:
+    creation_time: int
+    last_update_time: int
+    option_id: str
+    start_date: int
+    parameters: list[OptionParameter] | None
+
+    def __init__(
+        self,
+        *,
+        creation_time: int,
+        last_update_time: int,
+        option_id: str,
+        start_date: int,
+        parameters: list[dict[str, Any]] | None,
+        **_: Any,
+    ) -> None:
+        self.creation_time = creation_time
+        self.last_update_time = last_update_time
+        self.option_id = option_id
+        self.start_date = start_date
+        self.parameters = (
+            [OptionParameter(**p) for p in parameters] if parameters else []
+        )
```

### Comparing `pyoverkiz-1.9.0/pyoverkiz/obfuscate.py` & `pyoverkiz-1.9.1/pyoverkiz/obfuscate.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/types.py` & `pyoverkiz-1.9.1/pyoverkiz/types.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyoverkiz/utils.py` & `pyoverkiz-1.9.1/pyoverkiz/utils.py`

 * *Files identical despite different names*

### Comparing `pyoverkiz-1.9.0/pyproject.toml` & `pyoverkiz-1.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoverkiz"
-version = "1.9.0"
+version = "1.9.1"
 description = "Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma)."
 authors = ["Mick Vleeshouwer", "Vincent Le Bourlot", "Thibaut Etienne"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iMicknl/python-overkiz-api"
 repository = "https://github.com/iMicknl/python-overkiz-api"
 packages = [
```

### Comparing `pyoverkiz-1.9.0/PKG-INFO` & `pyoverkiz-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoverkiz
-Version: 1.9.0
+Version: 1.9.1
 Summary: Async Python client to interact with internal OverKiz API (e.g. used by Somfy TaHoma).
 Home-page: https://github.com/iMicknl/python-overkiz-api
 License: MIT
 Author: Mick Vleeshouwer
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyoverkiz Version: 1.9.0 Summary: Async Python
+Metadata-Version: 2.1 Name: pyoverkiz Version: 1.9.1 Summary: Async Python
 client to interact with internal OverKiz API (e.g. used by Somfy TaHoma). Home-
 page: https://github.com/iMicknl/python-overkiz-api License: MIT Author: Mick
 Vleeshouwer Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

