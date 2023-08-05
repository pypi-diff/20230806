# Comparing `tmp/MySchedule.py-1.0.5.tar.gz` & `tmp/MySchedule.py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySchedule.py-1.0.5.tar", last modified: Mon Jul 31 09:26:23 2023, max compression
+gzip compressed data, was "MySchedule.py-1.0.6.tar", last modified: Sat Aug  5 22:51:41 2023, max compression
```

## Comparing `MySchedule.py-1.0.5.tar` & `MySchedule.py-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/MySchedule.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/schedule/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11523 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/schedule/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/schedule/structures.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 22:51:41.848702 MySchedule.py-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-08-05 22:51:31.000000 MySchedule.py-1.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 22:51:41.848702 MySchedule.py-1.0.6/MySchedule.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-08-05 22:51:41.000000 MySchedule.py-1.0.6/MySchedule.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-08-05 22:51:41.000000 MySchedule.py-1.0.6/MySchedule.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-05 22:51:41.000000 MySchedule.py-1.0.6/MySchedule.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-08-05 22:51:41.000000 MySchedule.py-1.0.6/MySchedule.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-05 22:51:41.000000 MySchedule.py-1.0.6/MySchedule.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-08-05 22:51:41.848702 MySchedule.py-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-08-05 22:51:31.000000 MySchedule.py-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 22:51:41.848702 MySchedule.py-1.0.6/schedule/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-08-05 22:51:31.000000 MySchedule.py-1.0.6/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11728 2023-08-05 22:51:31.000000 MySchedule.py-1.0.6/schedule/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-08-05 22:51:31.000000 MySchedule.py-1.0.6/schedule/structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-05 22:51:41.848702 MySchedule.py-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-08-05 22:51:31.000000 MySchedule.py-1.0.6/setup.py
```

### Comparing `MySchedule.py-1.0.5/LICENSE` & `MySchedule.py-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MySchedule.py-1.0.5/MySchedule.py.egg-info/PKG-INFO` & `MySchedule.py-1.0.6/MySchedule.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MySchedule.py
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python wrapper for the McDonalds Myschedule
 Author: olijeffers0n
 Author-email: pleaseUseMyDiscord@Please.com
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MySchedule.py-1.0.5/PKG-INFO` & `MySchedule.py-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MySchedule.py
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python wrapper for the McDonalds Myschedule
 Author: olijeffers0n
 Author-email: pleaseUseMyDiscord@Please.com
 License: MIT
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MySchedule.py-1.0.5/README.md` & `MySchedule.py-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `MySchedule.py-1.0.5/schedule/api.py` & `MySchedule.py-1.0.6/schedule/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,25 +211,27 @@
 
     def get_timecard(self, week_end_date: str = None) -> List[Clock]:
         """
         :param week_end_date: The string in format DD/MM/YYYY of the Sunday of the week to get the timecard for
         :return: A timecard for the given week code
         """
         data = {
-                "authToken": self.auth_token,
-                "reqType": "ESS",
-                "mm": "ESSTIMECARD",
-                "sm": "SUMMARY",
-            }
+            "authToken": self.auth_token,
+            "reqType": "ESS",
+            "mm": "ESSTIMECARD",
+            "sm": "SUMMARY",
+        }
 
         if week_end_date is not None:
-            data.update({
-                "weekendDate": week_end_date,
-                "weekend": week_end_date,
-            })
+            data.update(
+                {
+                    "weekendDate": week_end_date,
+                    "weekend": week_end_date,
+                }
+            )
 
         # Make a request to the timecard page
         tc_request = self.session.post(
             "https://mcduk.reflexisinc.co.uk/RWS4/rta/tcard.jsp",
             data=data,
         )
 
@@ -269,15 +271,15 @@
             time_nodes = row.xpath("cell[5]/text()")
             punch_type_nodes = row.xpath("cell[3]/text()")
 
             # Check if date is present, update the date variable and add a new entry to the data dictionary
             if date_nodes and date_nodes[0] != " ":
                 date = date_nodes[0]
                 data_dict[date] = {"punches": []}
-            
+
             # Check if time and punch is present
             if time_nodes and punch_type_nodes:
                 # Extract the time and punch type from the CDATA content
                 time = self.extract_time(time_nodes[0])
 
                 punch_type = punch_type_nodes[0]
 
@@ -306,23 +308,27 @@
 
                 if punch["type"] == "Meal End":
                     diff = datetime.strptime(punch["time"], "%H:%M") - break_time
                     time_clocked_out += diff
                     clock_in_time = datetime.strptime(punch["time"], "%H:%M")
 
             # Convert total seconds to hours and minutes
-            time_clocked_in_hours, remaining_seconds = divmod(time_clocked_in.seconds, 3600)
+            time_clocked_in_hours, remaining_seconds = divmod(
+                time_clocked_in.seconds, 3600
+            )
             time_clocked_in_minutes = remaining_seconds // 60
 
-            time_clocked_out_hours, remaining_seconds = divmod(time_clocked_out.seconds, 3600)
+            time_clocked_out_hours, remaining_seconds = divmod(
+                time_clocked_out.seconds, 3600
+            )
             time_clocked_out_minutes = remaining_seconds // 60
 
             clocks.append(
                 Clock(
                     date,
                     punches,
-                    f"{time_clocked_in_hours}:{time_clocked_in_minutes}",
-                    f"{time_clocked_out_hours}:{time_clocked_out_minutes}"
+                    f"{time_clocked_in_hours}:{time_clocked_in_minutes if time_clocked_in_minutes > 9 else f'0{time_clocked_in_minutes}'}",
+                    f"{time_clocked_out_hours}:{time_clocked_out_minutes if time_clocked_out_minutes > 9 else f'0{time_clocked_out_minutes}'}",
                 )
             )
 
         return clocks
```

### Comparing `MySchedule.py-1.0.5/schedule/structures.py` & `MySchedule.py-1.0.6/schedule/structures.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,20 +58,49 @@
     def __init__(self, punch_type: PunchType, time: str) -> None:
         self.type = punch_type
         self.time = time
 
     def __repr__(self) -> str:
         return f"Punch({self.type}, {self.time})"
 
+    def to_dict(self):
+        return {"type": self.type.value, "time": self.time}
+
+    @classmethod
+    def from_dict(cls, data):
+        punch_type = PunchType(data["type"])
+        return cls(punch_type, data["time"])
+
 
 class Clock:
-    def __init__(self, date: str, punches: List[Punch], clocked_in_time: str, break_time: str) -> None:
+    def __init__(
+        self, date: str, punches: List[Punch], clocked_in_time: str, break_time: str
+    ) -> None:
         self.date = date
         self.punches = punches
         self.time_clocked_in = clocked_in_time
         self.time_clocked_out = break_time
 
     def __repr__(self) -> str:
         data = "Clock("
         for punch in self.punches:
             data += punch.__repr__() + ", "
-        return data + f"Time Clocked in: {self.time_clocked_in}, Time Clocked out: {self.time_clocked_out}" + ")"
+        return (
+            data
+            + f"Time Clocked in: {self.time_clocked_in}, Time Clocked out: {self.time_clocked_out}"
+            + ")"
+        )
+
+    def to_dict(self):
+        return {
+            "date": self.date,
+            "punches": [punch.to_dict() for punch in self.punches],
+            "time_clocked_in": self.time_clocked_in,
+            "time_clocked_out": self.time_clocked_out,
+        }
+
+    @classmethod
+    def from_dict(cls, data):
+        punches = [Punch.from_dict(punch_data) for punch_data in data["punches"]]
+        return cls(
+            data["date"], punches, data["time_clocked_in"], data["time_clocked_out"]
+        )
```

### Comparing `MySchedule.py-1.0.5/setup.py` & `MySchedule.py-1.0.6/setup.py`

 * *Files identical despite different names*

