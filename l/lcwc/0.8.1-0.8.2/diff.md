# Comparing `tmp/lcwc-0.8.1.tar.gz` & `tmp/lcwc-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.8.1.tar", last modified: Wed Jul 12 15:57:55 2023, max compression
+gzip compressed data, was "lcwc-0.8.2.tar", last modified: Sun Aug  6 15:41:04 2023, max compression
```

## Comparing `lcwc-0.8.1.tar` & `lcwc-0.8.2.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.763323 lcwc-0.8.1/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     2327 2023-07-12 15:57:55.760825 lcwc-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.8.1/README.md
--rw-rw-rw-   0        0        0      804 2023-07-12 15:57:47.000000 lcwc-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 15:57:55.763323 lcwc-0.8.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.661822 lcwc-0.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.686823 lcwc-0.8.1/src/lcwc/
--rw-rw-rw-   0        0        0      192 2023-07-12 15:14:30.000000 lcwc-0.8.1/src/lcwc/__init__.py
--rw-rw-rw-   0        0        0      849 2023-07-12 15:14:30.000000 lcwc-0.8.1/src/lcwc/agency.py
--rw-rw-rw-   0        0        0     3957 2023-07-12 15:57:23.000000 lcwc-0.8.1/src/lcwc/agencyclient.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.732823 lcwc-0.8.1/src/lcwc/arcgis/
--rw-rw-rw-   0        0        0       72 2023-06-30 18:00:38.000000 lcwc-0.8.1/src/lcwc/arcgis/__init__.py
--rw-rw-rw-   0        0        0     6502 2023-07-12 15:13:32.000000 lcwc-0.8.1/src/lcwc/arcgis/client.py
--rw-rw-rw-   0        0        0      769 2023-07-07 07:11:12.000000 lcwc-0.8.1/src/lcwc/arcgis/incident.py
--rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.8.1/src/lcwc/category.py
--rw-rw-rw-   0        0        0      318 2023-06-30 18:02:43.000000 lcwc-0.8.1/src/lcwc/client.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.738323 lcwc-0.8.1/src/lcwc/feed/
--rw-rw-rw-   0        0        0       68 2023-06-30 17:57:06.000000 lcwc-0.8.1/src/lcwc/feed/__init__.py
--rw-rw-rw-   0        0        0     4468 2023-06-30 18:37:18.000000 lcwc-0.8.1/src/lcwc/feed/client.py
--rw-rw-rw-   0        0        0      241 2023-07-05 13:46:18.000000 lcwc-0.8.1/src/lcwc/feed/incident.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.740323 lcwc-0.8.1/src/lcwc/feed/utils/
--rw-rw-rw-   0        0        0     2373 2023-06-30 18:38:10.000000 lcwc-0.8.1/src/lcwc/feed/utils/__init__.py
--rw-rw-rw-   0        0        0      651 2023-07-01 15:08:06.000000 lcwc-0.8.1/src/lcwc/incident.py
--rw-rw-rw-   0        0        0      330 2023-07-09 20:02:44.000000 lcwc-0.8.1/src/lcwc/unit.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.752324 lcwc-0.8.1/src/lcwc/utils/
--rw-rw-rw-   0        0        0     2598 2023-07-12 15:14:30.000000 lcwc-0.8.1/src/lcwc/utils/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-07-07 07:17:11.000000 lcwc-0.8.1/src/lcwc/utils/encoding.py
--rw-rw-rw-   0        0        0     4286 2023-07-05 15:08:28.000000 lcwc-0.8.1/src/lcwc/utils/restadapter.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.758823 lcwc-0.8.1/src/lcwc/web/
--rw-rw-rw-   0        0        0       64 2023-06-30 17:55:06.000000 lcwc-0.8.1/src/lcwc/web/__init__.py
--rw-rw-rw-   0        0        0     3972 2023-06-30 18:34:22.000000 lcwc-0.8.1/src/lcwc/web/client.py
--rw-rw-rw-   0        0        0      232 2023-06-30 20:31:48.000000 lcwc-0.8.1/src/lcwc/web/incident.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:57:55.716324 lcwc-0.8.1/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     2327 2023-07-12 15:57:55.000000 lcwc-0.8.1/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-07-12 15:57:55.000000 lcwc-0.8.1/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:57:55.000000 lcwc-0.8.1/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-12 15:57:55.000000 lcwc-0.8.1/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 15:57:55.000000 lcwc-0.8.1/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.691534 lcwc-0.8.2/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0     2327 2023-08-06 15:41:04.691036 lcwc-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.8.2/README.md
+-rw-rw-rw-   0        0        0      861 2023-08-06 13:35:54.000000 lcwc-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:41:04.692035 lcwc-0.8.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.615535 lcwc-0.8.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.645535 lcwc-0.8.2/src/lcwc/
+-rw-rw-rw-   0        0        0      192 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-07-18 12:59:13.000000 lcwc-0.8.2/src/lcwc/agency.py
+-rw-rw-rw-   0        0        0     3957 2023-07-14 15:38:49.000000 lcwc-0.8.2/src/lcwc/agencyclient.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.660033 lcwc-0.8.2/src/lcwc/arcgis/
+-rw-rw-rw-   0        0        0       72 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/arcgis/__init__.py
+-rw-rw-rw-   0        0        0     6850 2023-07-17 16:49:26.000000 lcwc-0.8.2/src/lcwc/arcgis/client.py
+-rw-rw-rw-   0        0        0      827 2023-07-17 16:48:17.000000 lcwc-0.8.2/src/lcwc/arcgis/incident.py
+-rw-rw-rw-   0        0        0      326 2023-08-04 17:46:20.000000 lcwc-0.8.2/src/lcwc/category.py
+-rw-rw-rw-   0        0        0      318 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/client.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.672536 lcwc-0.8.2/src/lcwc/feed/
+-rw-rw-rw-   0        0        0       98 2023-08-06 13:33:16.000000 lcwc-0.8.2/src/lcwc/feed/__init__.py
+-rw-rw-rw-   0        0        0     1235 2023-08-06 13:33:16.000000 lcwc-0.8.2/src/lcwc/feed/client.py
+-rw-rw-rw-   0        0        0      241 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/feed/incident.py
+-rw-rw-rw-   0        0        0     3367 2023-08-06 13:33:16.000000 lcwc-0.8.2/src/lcwc/feed/parser.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.674536 lcwc-0.8.2/src/lcwc/feed/utils/
+-rw-rw-rw-   0        0        0     2373 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/feed/utils/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/incident.py
+-rw-rw-rw-   0        0        0      330 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/unit.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.679034 lcwc-0.8.2/src/lcwc/utils/
+-rw-rw-rw-   0        0        0     2598 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/utils/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-07-14 15:51:33.000000 lcwc-0.8.2/src/lcwc/utils/encoding.py
+-rw-rw-rw-   0        0        0     4303 2023-08-06 13:32:58.000000 lcwc-0.8.2/src/lcwc/utils/restadapter.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.690034 lcwc-0.8.2/src/lcwc/web/
+-rw-rw-rw-   0        0        0       97 2023-08-06 13:33:16.000000 lcwc-0.8.2/src/lcwc/web/__init__.py
+-rw-rw-rw-   0        0        0     1202 2023-08-06 13:33:16.000000 lcwc-0.8.2/src/lcwc/web/client.py
+-rw-rw-rw-   0        0        0      232 2023-07-13 13:44:15.000000 lcwc-0.8.2/src/lcwc/web/incident.py
+-rw-rw-rw-   0        0        0     2665 2023-08-06 13:33:16.000000 lcwc-0.8.2/src/lcwc/web/parser.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:41:04.654035 lcwc-0.8.2/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     2327 2023-08-06 15:41:04.000000 lcwc-0.8.2/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2023-08-06 15:41:04.000000 lcwc-0.8.2/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:41:04.000000 lcwc-0.8.2/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-08-06 15:41:04.000000 lcwc-0.8.2/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-06 15:41:04.000000 lcwc-0.8.2/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.8.1/LICENSE` & `lcwc-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.8.1/PKG-INFO` & `lcwc-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.8.1/README.md` & `lcwc-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `lcwc-0.8.1/pyproject.toml` & `lcwc-0.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
@@ -17,13 +17,18 @@
 dependencies = [
     "bs4", 
     "aiohttp", 
     "feedparser",
     "pytz"
 ]
 
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project.urls]
 "Homepage" = "https://github.com/NateShoffner/python-lcwc"
 "Bug Tracker" = "https://github.com/NateShoffner/python-lcwc/issues"
```

### Comparing `lcwc-0.8.1/src/lcwc/agency.py` & `lcwc-0.8.2/src/lcwc/agency.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,8 +31,11 @@
 
     """ The phone number of the agency """
     phone: str
 
     def __eq__(self, other):
         if not isinstance(other, Agency):
             return False
-        return self.station_number == other.station_number
+        return (
+            self.category == other.category
+            and self.station_number == other.station_number
+        )
```

### Comparing `lcwc-0.8.1/src/lcwc/agencyclient.py` & `lcwc-0.8.2/src/lcwc/agencyclient.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.8.1/src/lcwc/arcgis/client.py` & `lcwc-0.8.2/src/lcwc/arcgis/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import aiohttp
 import datetime
 import json
 import re
+
+import pytz
 from lcwc import Client
 from lcwc.arcgis.incident import ArcGISIncident, Coordinates
 from lcwc.category import IncidentCategory
 from lcwc.unit import Unit
 from lcwc.utils.restadapter import RestAdapter, RestException
 
 
@@ -39,36 +41,39 @@
                 "IncidentMunicipality",
                 "IncidentOrigination",
                 "PrimaryAgency",
                 "CurrentUnits",
                 "PublicLocation",
                 "PublicType",
                 "IsPublic",
+                "OBJECTID"
             ],
             IncidentCategory.MEDICAL: [
                 "IncidentNumber",
                 "IncidentMunicipality",
                 "IncidentOrigination",
                 "PrimaryAgency",
                 "CurrentUnits",
                 "PublicLocation",
                 "PublicType",
                 "IsPublic",
                 "Priority",
+                "OBJECTID"
             ],
             IncidentCategory.TRAFFIC: [
                 "IncidentNumber",
                 "IncidentMunicipality",
                 "IncidentOrigination",
                 "PrimaryAgency",
                 "CurrentUnits",
                 "PublicLocation",
                 "PublicType",
                 "IsPublic",
                 "Priority",
+                "OBJECTID"
             ],
         }
 
         incidents = []
 
         for cat in IncidentCategory:
             if cat == IncidentCategory.UNKNOWN:
@@ -151,15 +156,22 @@
 
     def __parse_incident(
         self, category: IncidentCategory, incident: dict
     ) -> ArcGISIncident:
         attributes = incident["attributes"]
         geometry = incident["geometry"]
 
-        date = datetime.datetime.fromtimestamp(attributes["IncidentOrigination"] / 1000)
+
+        # convert date to UTC
+
+        raw_date = datetime.datetime.fromtimestamp(attributes["IncidentOrigination"] / 1000)
+        local_tz = pytz.timezone("America/New_York")
+        local_dt = local_tz.localize(raw_date, is_dst=None)  
+        date = local_dt.astimezone(pytz.utc)
+        
         municipality = attributes["IncidentMunicipality"]
 
         intersection = re.sub(
             " +", " ", attributes["PublicLocation"]
         )  # collapse multiple spaces
 
         # unit names are condensed, lacking spaces and delimiters (ex: MED8611)
@@ -188,10 +200,11 @@
             municipality,
             intersection,
             units,
             number,
             priority,
             agency,
             public,
-            coords
+            coords,
+            attributes["OBJECTID"]
         )
         return incident
```

### Comparing `lcwc-0.8.1/src/lcwc/arcgis/incident.py` & `lcwc-0.8.2/src/lcwc/arcgis/incident.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,7 +28,10 @@
     agency: str
 
     """ Whether the incident is public """
     public: bool
 
     """ The coordinates of the incident """
     coordinates: Coordinates
+    
+    """ The ArcGIS ObjectID """
+    objectID: int
```

### Comparing `lcwc-0.8.1/src/lcwc/feed/utils/__init__.py` & `lcwc-0.8.2/src/lcwc/feed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.8.1/src/lcwc/incident.py` & `lcwc-0.8.2/src/lcwc/incident.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.8.1/src/lcwc/utils/__init__.py` & `lcwc-0.8.2/src/lcwc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.8.1/src/lcwc/utils/encoding.py` & `lcwc-0.8.2/src/lcwc/utils/encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 class IncidentDecoder(json.JSONDecoder):
     def decode(self, s, incident_type):
         if not issubclass(incident_type, Incident):
             raise TypeError("incident_type must implement Incident")
 
         obj = json.loads(s)
 
+        if isinstance(obj, list):
+            return [self.decode(json.dumps(item), incident_type) for item in obj]
+
         obj["category"] = IncidentCategory(obj["category"])
         if "date" in obj:
             obj["date"] = datetime.datetime.fromisoformat(obj["date"])
         if "units" in obj:
             obj["units"] = [Unit(**unit) for unit in obj["units"]]
         if "coordinates" in obj:
             obj["coordinates"] = Coordinates(**obj["coordinates"])
```

### Comparing `lcwc-0.8.1/src/lcwc/utils/restadapter.py` & `lcwc-0.8.2/src/lcwc/utils/restadapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 json=data,
             )
         except aiohttp.ClientError as e:
             raise RestException("Request failed") from e
 
         # deserialize
         try:
-            data_out = await response.json()
+            data_out = await response.json(content_type=None)
         except (ValueError, TypeError, JSONDecodeError) as e:
             raise RestException("Bad JSON in response") from e
 
         status_code = response.status
         # If status_code in 200-299 range, return success Result with data, otherwise raise exception
         is_success = 299 >= status_code >= 200  # 200 to 299 is OK
         if is_success:
```

### Comparing `lcwc-0.8.1/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.8.2/src/lcwc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.8.1/src/lcwc.egg-info/SOURCES.txt` & `lcwc-0.8.2/src/lcwc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 src/lcwc.egg-info/top_level.txt
 src/lcwc/arcgis/__init__.py
 src/lcwc/arcgis/client.py
 src/lcwc/arcgis/incident.py
 src/lcwc/feed/__init__.py
 src/lcwc/feed/client.py
 src/lcwc/feed/incident.py
+src/lcwc/feed/parser.py
 src/lcwc/feed/utils/__init__.py
 src/lcwc/utils/__init__.py
 src/lcwc/utils/encoding.py
 src/lcwc/utils/restadapter.py
 src/lcwc/web/__init__.py
 src/lcwc/web/client.py
-src/lcwc/web/incident.py
+src/lcwc/web/incident.py
+src/lcwc/web/parser.py
```

