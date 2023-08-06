# Comparing `tmp/pyoscar_emr-0.9.1.tar.gz` & `tmp/pyoscar_emr-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoscar_emr-0.9.1.tar", max compression
+gzip compressed data, was "pyoscar_emr-0.9.2.tar", max compression
```

## Comparing `pyoscar_emr-0.9.1.tar` & `pyoscar_emr-0.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-27 18:31:38.067485 pyoscar_emr-0.9.1/LICENSE
--rw-r--r--   0        0        0      193 2023-04-27 18:32:41.748181 pyoscar_emr-0.9.1/README.md
--rw-r--r--   0        0        0      331 2023-04-19 03:35:10.246610 pyoscar_emr-0.9.1/pyoscar_emr/__init__.py
--rw-r--r--   0        0        0     2050 2023-04-19 03:35:19.937225 pyoscar_emr-0.9.1/pyoscar_emr/appointment.py
--rw-r--r--   0        0        0     1311 2023-04-19 03:35:17.453180 pyoscar_emr-0.9.1/pyoscar_emr/appointment_status.py
--rw-r--r--   0        0        0     2652 2023-04-19 03:35:22.570531 pyoscar_emr-0.9.1/pyoscar_emr/demographic.py
--rw-r--r--   0        0        0     2497 2023-04-19 03:35:25.414929 pyoscar_emr-0.9.1/pyoscar_emr/endpoints.py
--rw-r--r--   0        0        0      259 2023-04-27 18:22:39.524253 pyoscar_emr-0.9.1/pyoscar_emr/exceptions.py
--rw-r--r--   0        0        0     1081 2023-04-19 03:35:45.949559 pyoscar_emr-0.9.1/pyoscar_emr/ontario_health_card.py
--rw-r--r--   0        0        0    16062 2023-04-29 16:49:48.960440 pyoscar_emr-0.9.1/pyoscar_emr/oscar.py
--rw-r--r--   0        0        0      191 2023-04-19 03:36:01.949472 pyoscar_emr-0.9.1/pyoscar_emr/response_type.py
--rw-r--r--   0        0        0     7949 2023-04-27 18:10:49.311346 pyoscar_emr-0.9.1/pyoscar_emr/util/get_oauth_creds.py
--rw-r--r--   0        0        0      653 2023-04-29 16:55:56.374399 pyoscar_emr-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pyoscar_emr-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/LICENSE
+-rw-r--r--   0        0        0      193 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/README.md
+-rw-r--r--   0        0        0      331 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/__init__.py
+-rw-r--r--   0        0        0     2050 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/appointment.py
+-rw-r--r--   0        0        0     1311 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/appointment_status.py
+-rw-r--r--   0        0        0     2652 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/demographic.py
+-rw-r--r--   0        0        0     2746 2023-08-06 17:55:16.618600 pyoscar_emr-0.9.2/pyoscar_emr/endpoints.py
+-rw-r--r--   0        0        0      259 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/exceptions.py
+-rw-r--r--   0        0        0     1081 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/ontario_health_card.py
+-rw-r--r--   0        0        0    17383 2023-08-06 17:54:47.674570 pyoscar_emr-0.9.2/pyoscar_emr/oscar.py
+-rw-r--r--   0        0        0      191 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/response_type.py
+-rw-r--r--   0        0        0     7949 2023-08-06 17:52:34.306430 pyoscar_emr-0.9.2/pyoscar_emr/util/get_oauth_creds.py
+-rw-r--r--   0        0        0      653 2023-08-06 18:00:59.430961 pyoscar_emr-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 pyoscar_emr-0.9.2/PKG-INFO
```

### Comparing `pyoscar_emr-0.9.1/LICENSE` & `pyoscar_emr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/appointment.py` & `pyoscar_emr-0.9.2/pyoscar_emr/appointment.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/appointment_status.py` & `pyoscar_emr-0.9.2/pyoscar_emr/appointment_status.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/demographic.py` & `pyoscar_emr-0.9.2/pyoscar_emr/demographic.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/endpoints.py` & `pyoscar_emr-0.9.2/pyoscar_emr/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,33 +16,39 @@
 @dataclass()
 class APIEndpoints:
     """
     A class used to store all of the endpoints that are needed for using the OSCAR REST API.
     """
 
     appt: APIEndpoint
-    demographic: APIEndpoint
+    demographic_id: APIEndpoint
+    demographic_hin: APIEndpoint
     appt_history: APIEndpoint
     appt_statuses: APIEndpoint
     provider_monthly_appts: APIEndpoint
     appt_status_update: APIEndpoint
 
     def __init__(self, base_url: str):
         self.base_url = base_url
 
         # GET
         self.provider_monthly_appts = APIEndpoint(
             self.base_url
             + "/oscar/ws/services/schedule/fetchMonthly/{provider_id}/{year}/{month}",
             ResponseType.JSON,
         )
-        self.demographic = APIEndpoint(
+        self.demographic_id = APIEndpoint(
             self.base_url + "/oscar/ws/services/demographics/{id}",
             ResponseType.JSON,
         )
+        self.demographic_hin = APIEndpoint(
+            self.base_url
+            + "/oscar/ws/services/demographics/search?startIndex=0&itemsToReturn={itemsToReturn}",
+            ResponseType.JSON,
+        )
         self.appt_statuses = APIEndpoint(
             self.base_url + "/oscar/ws/services/schedule/statuses",
             ResponseType.JSON,
         )
 
         # POST
         self.appt = APIEndpoint(
```

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/ontario_health_card.py` & `pyoscar_emr-0.9.2/pyoscar_emr/ontario_health_card.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/oscar.py` & `pyoscar_emr-0.9.2/pyoscar_emr/oscar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
-import aiohttp
 import json
-
-from playwright.async_api import Playwright, BrowserType
-from playwright_stealth import stealth_async
-
-import oauthlib.oauth1
 from datetime import datetime
 import logging
 from xml.etree import ElementTree
 import re
+import aiohttp
+
+from playwright.async_api import BrowserType
+from playwright_stealth import stealth_async
+
+import oauthlib.oauth1
 
 from .endpoints import (
     APIEndpoints,
     APIEndpoint,
     WebScrapingEndpoints,
 )
 from .response_type import ResponseType
@@ -39,16 +39,17 @@
         oauth_secret: str,
         oauth_token: str,
         client_key: str,
         client_secret: str,
         session: aiohttp.ClientSession,
     ):
         """
-        The constructor for OscarAPI. You should seriously be running OscarAPI.create() instead, as it runs
-        any necessary functions (ex. getting appointment statuses) that this function cannot due to asynchronous behavior.
+        The constructor for OscarAPI. You should seriously be running OscarAPI.create() instead, as
+        it runs any necessary functions (ex. getting appointment statuses) that this function cannot
+        due to asynchronous behavior.
         """
 
         self._endpoint = APIEndpoints(base_url=base_url)
         self._endpoint_webscraping = WebScrapingEndpoints(base_url=base_url)
         self._session = session
 
         self._oauth_secret = oauth_secret
@@ -61,15 +62,16 @@
             client_secret=self._client_secret,
             resource_owner_key=self._oauth_token,
             resource_owner_secret=self._oauth_secret,
         )
 
         self._statuses = (
             {}
-        )  # This should be run at least once. If you are running this initializer directly, please run get_appointment_statuses()
+        )  # This should be run at least once. If you are running this initializer directly,
+        #    please run get_appointment_statuses()
 
         self._demographics_cache = {0: None}
 
         self.webscrapping_enabled = False
 
         # Set up logging without interefering with main progrma
         self._log = logging.getLogger(__name__)
@@ -81,15 +83,16 @@
         oauth_secret: str,
         oauth_token: str,
         client_key: str,
         client_secret: str,
         session: aiohttp.ClientSession,
     ):
         """
-        Creates an instance of OscarAPI and runs all necessary functions to properly initialize (ex. fetching all appointment statuses).
+        Creates an instance of OscarAPI and runs all necessary functions to properly
+        initialize (ex. fetching all appointment statuses).
         """
 
         self = OscarAPI(
             base_url=base_url,
             oauth_secret=oauth_secret,
             oauth_token=oauth_token,
             client_key=client_key,
@@ -147,15 +150,15 @@
 
         self.webscrapping_enabled = True
         self._log.info("Webscrapping capabilities has been enabled.")
 
     async def _to_format(self, response: aiohttp.ClientResponse, endpoint: APIEndpoint):
         if endpoint.response_type == ResponseType.JSON:
             return await response.json()
-        elif endpoint.response_type == ResponseType.XML:
+        if endpoint.response_type == ResponseType.XML:
             return ElementTree.fromstring(await response.text())
 
         return None
 
     async def _get(self, endpoint: APIEndpoint, **kwargs):
         # Sign with OAuth1 credentials
         uri, headers, _ = self._oauth_client.sign(
@@ -188,15 +191,16 @@
 
     async def get_appointment_statuses(
         self, force_refresh: bool = False
     ) -> dict[str, AppointmentStatus]:
         """
         Gets all possible appointment statuses in the OSCAR EMR instance.
 
-        Returns a dictionary, where key -> status attribute of AppointmentStatus, and value -> AppointmentStatus object.
+        Returns a dictionary, where key -> status attribute of AppointmentStatus,
+        and value -> AppointmentStatus object.
         """
 
         # Return cached version whenever possible
         if not force_refresh and len(self._statuses) != 0:
             return self._statuses
 
         res_data = await self._get(self._endpoint.appt_statuses)
@@ -329,20 +333,56 @@
 
         Will raise an aiohttp exception if no such demographic exists.
         """
 
         if id in self._demographics_cache and not force_refresh:
             return self._demographics_cache[id]
 
-        data = await self._get(self._endpoint.demographic, id=id)
+        data = await self._get(self._endpoint.demographic_id, id=id)
         assert isinstance(data, dict)
         demographic = Demographic.from_dict(data)
 
         self._demographics_cache[id] = demographic
-        return Demographic.from_dict(data)
+        return demographic
+
+    async def get_demographic_by_hin(self, hin: str) -> Demographic:
+        """
+        Get a Demographic from the person's Health Insurance Number (HIN)
+
+        Retruns a Demographic if one is found, otherwise returns None.
+        """
+
+        data = await self._post(
+            self._endpoint.demographic_hin,
+            {
+                "type": "HIN",
+                "term": hin,
+                "active": True,
+                "integrator": True,  # Check if this is necessary
+                "outofdomain": False,
+            },
+            itemsToReturn=2,
+        )
+        assert isinstance(data, dict)
+
+        # Check if only one thing was fetched (if there's two, there's a different problem)
+        assert data["total"] <= 1, "More than two demographics found with same HIN"
+        if data["total"] != 1 or len(data["content"]) != 1:
+            return None
+
+        # Get demographic no
+        # TODO: Consider adding caching of HIN to Demographic No?
+        demographic_no: int = data["content"][0]["demographicNo"]
+        assert isinstance(demographic_no, int), "Demographic No is corrupt (not an int)"
+
+        # Get demographic data using demo no
+        demographic = await self.get_demographic_by_id(demographic_no)
+
+        # Return demographic data
+        return demographic
 
     async def get_appointment_history(
         self, demographic: Demographic
     ) -> list[Appointment]:
         """
         Get a demographic's appointment history.
```

### Comparing `pyoscar_emr-0.9.1/pyoscar_emr/util/get_oauth_creds.py` & `pyoscar_emr-0.9.2/pyoscar_emr/util/get_oauth_creds.py`

 * *Files identical despite different names*

### Comparing `pyoscar_emr-0.9.1/pyproject.toml` & `pyoscar_emr-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoscar_emr"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python wrapper for the OSCAR EMR API"
 authors = ["Aritro <29025984+AritroSaha10@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = {extras = ["speedups"], version = "^3.8.4"}
```

### Comparing `pyoscar_emr-0.9.1/PKG-INFO` & `pyoscar_emr-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoscar-emr
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python wrapper for the OSCAR EMR API
 Author: Aritro
 Author-email: 29025984+AritroSaha10@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
```

