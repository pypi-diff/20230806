# Comparing `tmp/metaboatrace_models-0.6.0.tar.gz` & `tmp/metaboatrace_models-0.7.0.tar.gz`

## Comparing `metaboatrace_models-0.6.0.tar` & `metaboatrace_models-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/requirements-dev.lock
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/requirements.lock
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/metaboatrace/models/__init__.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/metaboatrace/models/boat.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/metaboatrace/models/race.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/metaboatrace/models/racer.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/metaboatrace/models/region.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/metaboatrace/models/stadium.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/test_boat.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/test_racer.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/test_region.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/test_stadium.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/race/test_bettings.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/race/test_race_entries.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/tests/metaboatrace/models/race/test_races.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/requirements-dev.lock
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/requirements.lock
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/metaboatrace/models/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/metaboatrace/models/boat.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/metaboatrace/models/race.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/metaboatrace/models/racer.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/metaboatrace/models/region.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/metaboatrace/models/stadium.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/test_boat.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/test_racer.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/test_region.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/test_stadium.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/race/test_bettings.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/race/test_race_entries.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/tests/metaboatrace/models/race/test_races.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 metaboatrace_models-0.7.0/PKG-INFO
```

### Comparing `metaboatrace_models-0.6.0/.github/workflows/lint.yml` & `metaboatrace_models-0.7.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/.github/workflows/publish.yml` & `metaboatrace_models-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/.github/workflows/tests.yml` & `metaboatrace_models-0.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/metaboatrace/models/boat.py` & `metaboatrace_models-0.7.0/metaboatrace/models/boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/metaboatrace/models/race.py` & `metaboatrace_models-0.7.0/metaboatrace/models/race.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,24 @@
     title: str
     number_of_laps: Literal[2, 3]
     deadline_at: datetime
     is_course_fixed: bool
     use_stabilizer: bool
 
 
+class WeatherCondition(_RaceIdentifier):
+    in_performance: bool
+    weather: Weather
+    wavelength: Optional[float]
+    wind_angle: Optional[float] = Field(None, ge=0, le=360)
+    wind_velocity: float
+    air_temperature: float
+    water_temperature: float
+
+
 class RaceEntry(_RaceEntryIdentifier):
     racer_registration_number: StrictInt
     is_absent: bool
     motor_number: StrictInt = Field(..., ge=1, le=99)
     boat_number: StrictInt = Field(..., ge=1, le=999)
```

### Comparing `metaboatrace_models-0.6.0/metaboatrace/models/racer.py` & `metaboatrace_models-0.7.0/metaboatrace/models/racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/metaboatrace/models/region.py` & `metaboatrace_models-0.7.0/metaboatrace/models/region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/metaboatrace/models/stadium.py` & `metaboatrace_models-0.7.0/metaboatrace/models/stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/test_boat.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/test_boat.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/test_racer.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/test_racer.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/test_region.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/test_region.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/test_stadium.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/test_stadium.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/race/test_bettings.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/race/test_bettings.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/race/test_race_entries.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/race/test_race_entries.py`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/tests/metaboatrace/models/race/test_races.py` & `metaboatrace_models-0.7.0/tests/metaboatrace/models/race/test_races.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, datetime
 
 import pytest
 from pydantic import ValidationError
 
-from metaboatrace.models.race import RaceInformation
+from metaboatrace.models.race import RaceInformation, Weather, WeatherCondition
 from metaboatrace.models.stadium import StadiumTelCode
 
 
 @pytest.mark.parametrize(
     "race_holding_date,stadium_tel_code,race_number,title,number_of_laps,deadline_at,is_course_fixed,use_stabilizer,expected",
     [
         # valid case
@@ -56,7 +56,72 @@
         assert race_information.number_of_laps == data["number_of_laps"]
         assert race_information.deadline_at == data["deadline_at"]
         assert race_information.is_course_fixed == data["is_course_fixed"]
         assert race_information.use_stabilizer == data["use_stabilizer"]
     else:
         with pytest.raises(ValidationError):
             race_information = RaceInformation(**data)
+
+
+@pytest.mark.parametrize(
+    "race_holding_date, stadium_tel_code, race_number, in_performance, weather, wavelength, wind_angle, wind_velocity, air_temperature, water_temperature, expected",
+    [
+        # valid case
+        (
+            date.today(),
+            StadiumTelCode.HEIWAJIMA,
+            1,
+            True,
+            Weather.FINE,
+            1.5,
+            90,
+            5.0,
+            25.0,
+            20.0,
+            True,
+        ),
+        # invalid wind_angle
+        (
+            date.today(),
+            StadiumTelCode.HEIWAJIMA,
+            1,
+            True,
+            Weather.FINE,
+            1.5,
+            370,  # 無効な風の角度
+            5.0,
+            25.0,
+            20.0,
+            False,
+        ),
+    ],
+)
+def test_weather_condition(
+    race_holding_date,
+    stadium_tel_code,
+    race_number,
+    in_performance,
+    weather,
+    wavelength,
+    wind_angle,
+    wind_velocity,
+    air_temperature,
+    water_temperature,
+    expected,
+):
+    data = {
+        "race_holding_date": race_holding_date,
+        "stadium_tel_code": stadium_tel_code,
+        "race_number": race_number,
+        "in_performance": in_performance,
+        "weather": weather,
+        "wavelength": wavelength,
+        "wind_angle": wind_angle,
+        "wind_velocity": wind_velocity,
+        "air_temperature": air_temperature,
+        "water_temperature": water_temperature,
+    }
+    if expected:
+        WeatherCondition(**data)
+    else:
+        with pytest.raises(ValidationError):
+            WeatherCondition(**data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metaboatrace_models-0.6.0/.gitignore` & `metaboatrace_models-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/LICENSE.txt` & `metaboatrace_models-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metaboatrace_models-0.6.0/pyproject.toml` & `metaboatrace_models-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metaboatrace.models"
-version = "0.6.0"
+version = "0.7.0"
 description = "Models of Japanese boatrace"
 authors = [
     { name = "k0kishima", email = "okishimaxyz@gmail.com" }
 ]
 dependencies = [
     "pydantic>=2.0.3",
 ]
```

