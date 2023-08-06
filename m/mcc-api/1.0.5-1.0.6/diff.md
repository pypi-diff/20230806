# Comparing `tmp/mcc_api-1.0.5.tar.gz` & `tmp/mcc_api-1.0.6.tar.gz`

## Comparing `mcc_api-1.0.5.tar` & `mcc_api-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.github/workflows/docs.yml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.5/docs/conf.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.5/docs/index.rst
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/exceptions.py
--rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.5/mcc_api/responses.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/run_tests.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_event.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_halloffame.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_participants.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/200_rundown.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/400_halloffame_game.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/400_participants_team.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/400_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.5/tests/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.5/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.5/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 mcc_api-1.0.6/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 mcc_api-1.0.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.6/docs/conf.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.6/docs/index.rst
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 mcc_api-1.0.6/mcc_api/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.6/mcc_api/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.6/mcc_api/exceptions.py
+-rw-r--r--   0        0        0    12687 2020-02-02 00:00:00.000000 mcc_api-1.0.6/mcc_api/responses.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/run_tests.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/test_event.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/test_halloffame.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/test_participants.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/404_halloffame_game.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/404_participants_team.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/404_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.6/tests/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.6/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.6/PKG-INFO
```

### Comparing `mcc_api-1.0.5/.github/workflows/docs.yml` & `mcc_api-1.0.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/.github/workflows/pypi_publish.yml` & `mcc_api-1.0.6/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/.github/workflows/tests.yml` & `mcc_api-1.0.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/docs/index.rst` & `mcc_api-1.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/mcc_api/__init__.py` & `mcc_api-1.0.6/mcc_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "get_rundown",
     "get_participants",
 
     "enums",
     "exceptions",
     "responses"
 ]
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 __base_url: t.Final[str] = "https://api.mcchampionship.com/v1"
 __user_agent: t.Final[str] = f"python_mcc_api/{__version__} (https://github.com/JamesMCo/python_mcc_api)"
 
 
 @ratelimit.sleep_and_retry
 @ratelimit.limits(calls=40, period=60)
```

### Comparing `mcc_api-1.0.5/mcc_api/enums.py` & `mcc_api-1.0.6/mcc_api/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/mcc_api/exceptions.py` & `mcc_api-1.0.6/mcc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/mcc_api/responses.py` & `mcc_api-1.0.6/mcc_api/responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
        }
     """
 
     def __init__(self: "HallOfFameGameResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
-        if self.code == 400:
+        if self.code == 404:
             raise InvalidGameError(self.code, self.reason)
 
         self.data = {
             record_name: HallOfFameRecord(
                 player=record_data["player"],
                 value=record_data["value"],
                 placement=record_data["placement"],
@@ -252,15 +252,15 @@
     data: EventRundown
     """Object representing the event's data."""
 
     def __init__(self: "RundownResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
-        if self.code == 400:
+        if self.code == 404:
             raise InvalidEventError(self.code, self.reason)
 
         self.data = EventRundown(
             dodgeboltData={Team[team]: score for team, score in data["data"]["dodgeboltData"].items()},
             eventPlacements={Team[team]: placement for team, placement in data["data"]["eventPlacements"].items()},
             eventScores={Team[team]: score for team, score in data["data"]["eventScores"].items()},
             individualScores=data["data"]["individualScores"],
@@ -317,15 +317,15 @@
     data: list[Creator]
     """List of detailed participant data."""
 
     def __init__(self: "ParticipantsTeamResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
-        if self.code == 400:
+        if self.code == 404:
             raise InvalidTeamError(self.code, self.reason)
 
         self.data = [
             Creator(
                 username=creator["username"],
                 uuid=creator["uuid"],
                 stream=creator["stream"]
```

### Comparing `mcc_api-1.0.5/tests/run_tests.py` & `mcc_api-1.0.6/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/tests/test_event.py` & `mcc_api-1.0.6/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/tests/test_halloffame.py` & `mcc_api-1.0.6/tests/test_halloffame.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,17 +73,17 @@
         self.assertIn("RECORD NAME 2", records)
         self.assertEqual(records["RECORD NAME 2"].placement, 1)
         self.assertEqual(records["RECORD NAME 2"].player, "MCChampionship")
         self.assertEqual(records["RECORD NAME 2"].value, 0)
         self.assertTrue(records["RECORD NAME 2"].changedHands)
 
 
-class TestHallOfFameGameEndpoint400(unittest.TestCase):
-    def test_halloffame_game_invalid_game_exception(self: "TestHallOfFameGameEndpoint400") -> None:
-        with open("mock_data/400_halloffame_game.json") as f:
+class TestHallOfFameGameEndpoint404(unittest.TestCase):
+    def test_halloffame_game_invalid_game_exception(self: "TestHallOfFameGameEndpoint404") -> None:
+        with open("mock_data/404_halloffame_game.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.InvalidGameError, mcc_api.HallOfFameGameResponse, response_json)
 
 
 class TestHallOfFameGameEndpoint429(unittest.TestCase):
     def test_halloffame_game_ratelimit_exception(self: "TestHallOfFameGameEndpoint429") -> None:
```

### Comparing `mcc_api-1.0.5/tests/test_participants.py` & `mcc_api-1.0.6/tests/test_participants.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,17 +67,17 @@
             usernames.add(participant.username)
             uuids.add(participant.uuid)
 
         self.assertEqual(participants_count, len(usernames))
         self.assertEqual(participants_count, len(uuids))
 
 
-class TestParticipantsTeamEndpoint400(unittest.TestCase):
-    def test_participants_team_invalid_team_exception(self: "TestParticipantsTeamEndpoint400") -> None:
-        with open("mock_data/400_participants_team.json") as f:
+class TestParticipantsTeamEndpoint404(unittest.TestCase):
+    def test_participants_team_invalid_team_exception(self: "TestParticipantsTeamEndpoint404") -> None:
+        with open("mock_data/404_participants_team.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.InvalidTeamError, mcc_api.ParticipantsTeamResponse, response_json)
 
 
 class TestParticipantsTeamEndpoint429(unittest.TestCase):
     def test_participants_team_ratelimit_exception(self: "TestParticipantsTeamEndpoint429") -> None:
```

### Comparing `mcc_api-1.0.5/tests/test_rundown.py` & `mcc_api-1.0.6/tests/test_rundown.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 
     def test_history_multipliers(self: "TestRundownEndpoint200") -> None:
         for game, multiplier in zip(range(8), [1, 1.5, 1.5, 2, 2, 2.5, 2.5, 3]):
             with self.subTest(game=game):
                 self.assertEqual(self.response_object.data.history[str(game)].multiplier, multiplier)
 
 
-class TestRundownEndpoint400(unittest.TestCase):
-    def test_rundown_invalid_event_exception(self: "TestRundownEndpoint400") -> None:
-        with open("mock_data/400_rundown.json") as f:
+class TestRundownEndpoint404(unittest.TestCase):
+    def test_rundown_invalid_event_exception(self: "TestRundownEndpoint404") -> None:
+        with open("mock_data/404_rundown.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
         self.assertRaises(mcc_api.exceptions.InvalidEventError, mcc_api.RundownResponse, response_json)
 
 
 class TestRundownEndpoint429(unittest.TestCase):
     def test_rundown_ratelimit_exception(self: "TestRundownEndpoint429") -> None:
```

### Comparing `mcc_api-1.0.5/tests/mock_data/200_halloffame.json` & `mcc_api-1.0.6/tests/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/tests/mock_data/200_participants.json` & `mcc_api-1.0.6/tests/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/tests/mock_data/200_participants_team.json` & `mcc_api-1.0.6/tests/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/tests/mock_data/200_rundown.json` & `mcc_api-1.0.6/tests/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/.gitignore` & `mcc_api-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/LICENSE` & `mcc_api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/README.md` & `mcc_api-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/pyproject.toml` & `mcc_api-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.5/PKG-INFO` & `mcc_api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcc-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

