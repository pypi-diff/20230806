# Comparing `tmp/pyosutools-0.2.4.tar.gz` & `tmp/pyosutools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosutools-0.2.4.tar", last modified: Mon Jul 24 10:04:06 2023, max compression
+gzip compressed data, was "pyosutools-0.2.5.tar", last modified: Sat Aug  5 22:10:38 2023, max compression
```

## Comparing `pyosutools-0.2.4.tar` & `pyosutools-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 10:03:53.000000 pyosutools-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 10:04:06.664161 pyosutools-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.000000 pyosutools-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.660161 pyosutools-0.2.4/pyosutools/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/pyosutools/beatmaps/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/beatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/beatmaps/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/pyosutools/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/osu.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/db/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyosutools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:04:06.664161 pyosutools-0.2.4/pyosutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 10:04:06.000000 pyosutools-0.2.4/pyosutools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-24 10:03:53.000000 pyosutools-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:04:06.664161 pyosutools-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:38.543686 pyosutools-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 22:10:28.000000 pyosutools-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-05 22:10:38.543686 pyosutools-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:28.000000 pyosutools-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:38.539687 pyosutools-0.2.5/pyosutools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:38.539687 pyosutools-0.2.5/pyosutools/beatmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/beatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/beatmap/beatmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:38.543686 pyosutools-0.2.5/pyosutools/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/database/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/database/osu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/database/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/database/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyosutools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:38.539687 pyosutools-0.2.5/pyosutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-05 22:10:38.000000 pyosutools-0.2.5/pyosutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-05 22:10:38.000000 pyosutools-0.2.5/pyosutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 22:10:38.000000 pyosutools-0.2.5/pyosutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 22:10:38.000000 pyosutools-0.2.5/pyosutools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 22:10:38.000000 pyosutools-0.2.5/pyosutools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-05 22:10:28.000000 pyosutools-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 22:10:38.543686 pyosutools-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:10:38.543686 pyosutools-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-05 22:10:28.000000 pyosutools-0.2.5/tests/test_beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-05 22:10:28.000000 pyosutools-0.2.5/tests/test_db.py
```

### Comparing `pyosutools-0.2.4/LICENSE` & `pyosutools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.4/PKG-INFO` & `pyosutools-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.4/pyosutools/db/collection.py` & `pyosutools-0.2.5/pyosutools/database/collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
-from typing import List, Union
+from typing import List, ByteString
 import os
 import io
 
 from pyosutools import utils
-from pyosutools.db.datatypes import Collection
+from pyosutools.datatypes import Collection
 
 
 @dataclass
 class Collectiondb:
     """
     Class representing collection.db file
 
@@ -23,51 +23,44 @@
     collections: List[Collection]
         List of collections represented by "Collection" class
     """
     version: int
     count_collections: int
     collections: List[Collection]
 
+    @staticmethod
+    def from_path(path: os.PathLike):
+        with open(path, "rb") as f:
+            return Collectiondb.from_file(f)
+
+    @staticmethod
+    def from_file(file: io.BufferedReader):
+        return Collectiondb.from_data(file.read())
+
+    @staticmethod
+    def from_data(data: ByteString):
+        return _Parser(data).parse()
+
 
 class _Parser:
-    def __init__(self, collection_db_file) -> None:
-        self.collection_db_file = collection_db_file
+    def __init__(self, data) -> None:
+        self.data_io = io.BytesIO(data)
         self.offset = 0
 
     def parse(self) -> Collectiondb:
-        version = utils.read_uint(self.collection_db_file)
-        count_collections = utils.read_uint(self.collection_db_file)
-        collections = []
-        for _ in range(count_collections):
-            collections.append(self.parse_collection(version))
-
+        version = utils.read_uint(self.data_io)
+        count_collections = utils.read_uint(self.data_io)
+        collections = [
+            self.parse_collection(version) for _ in range(count_collections)
+        ]
         return Collectiondb(version, count_collections, collections)
 
     def parse_collection(self, game_ver: int = 0):
-        name = utils.read_string(self.collection_db_file)
-        count_beatmaps = utils.read_uint(self.collection_db_file)
-        beatmaps_hash = []
+        name = utils.read_string(self.data_io)
+        count_beatmaps = utils.read_uint(self.data_io)
 
-        for _ in range(count_beatmaps):
-            beatmaps_hash.append(utils.read_string(self.collection_db_file))
+        beatmaps_hash = [
+            utils.read_string(self.data_io)
+            for _ in range(count_beatmaps)
+        ]
 
         return Collection(name, count_beatmaps, beatmaps_hash)
-
-
-def parse_collectiondb(collectiondb_file: Union[str, os.PathLike, io.BytesIO]) -> Collectiondb:
-    """
-    Parse collection.db file
-
-    Args
-    ----
-    collectiondb_file: str | os.PathLike | io.BytesIO
-        Path or opened file
-
-    Returns
-    ----
-    Collectiondb
-        instance of Collectiondb class
-    """
-    if not isinstance(collectiondb_file, io.BytesIO):
-        collectiondb_file = open(collectiondb_file, "rb")
-
-    return _Parser(collectiondb_file).parse()
```

### Comparing `pyosutools-0.2.4/pyosutools/db/scores.py` & `pyosutools-0.2.5/pyosutools/database/scores.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
-from typing import List, Union
+from typing import List, ByteString
 import os
 import io
 
-from pyosutools.db.datatypes import BeatmapScores, Score
+from pyosutools.datatypes import BeatmapScores, ScoreDB
 from pyosutools.datatypes import GameMode, Mod
 from pyosutools import utils
 
 
 @dataclass
 class Scoresdb:
     """
@@ -24,28 +24,38 @@
     beatmaps_scores: List[BeatmapScores]
         List of scores on beatmaps represented by "BeatmapScores" class
     """
     version: int
     count_beatmaps_scores: int
     beatmaps_scores: List[BeatmapScores]
 
+    @staticmethod
+    def from_path(path: os.PathLike):
+        with open(path, "rb") as f:
+            return Scoresdb.from_file(f)
+
+    @staticmethod
+    def from_file(file: io.BufferedReader):
+        return Scoresdb.from_data(file.read())
+
+    @staticmethod
+    def from_data(data: ByteString):
+        return _Parser(data).parse()
+
 
 class _Parser:
-    def __init__(self, score_db_file) -> None:
-        self.score_db_file = score_db_file
-        self.offset = 0
+    def __init__(self, data) -> None:
+        self.data_io = io.BytesIO(data)
 
     def parse(self) -> Scoresdb:
-        version = utils.read_uint(self.score_db_file)
-        count_beatmaps = utils.read_uint(self.score_db_file)
-        beatmaps = []
-        for _ in range(count_beatmaps):
-            beatmaps.append(self.parse_beatmap_scores(version))
+        version = utils.read_uint(self.data_io)
+        count_beatmaps = utils.read_uint(self.data_io)
+        scores = [self.parse_beatmap_scores(version) for _ in range(count_beatmaps)]
 
-        return Scoresdb(version, count_beatmaps, beatmaps)
+        return Scoresdb(version, count_beatmaps, scores)
 
     def parse_score(self, game_ver: int = 0):
         """
         Parse score from file
 
         Args
         ----
@@ -55,68 +65,45 @@
             Version of game
 
         Returns
         ----
         Beatmap
             Parsed score
         """
-        gamemode = GameMode(utils.read_ubyte(self.score_db_file))
-        score_version = utils.read_uint(self.score_db_file)
-        beatmap_hash = utils.read_string(self.score_db_file)
-        username = utils.read_string(self.score_db_file)
-        replay_hash = utils.read_string(self.score_db_file)
-
-        count_300 = utils.read_ushort(self.score_db_file)
-        count_100 = utils.read_ushort(self.score_db_file)
-        count_50 = utils.read_ushort(self.score_db_file)
-        count_geki = utils.read_ushort(self.score_db_file)
-        count_katu = utils.read_ushort(self.score_db_file)
-        count_miss = utils.read_ushort(self.score_db_file)
-
-        total_score = utils.read_uint(self.score_db_file)
-        max_combo = utils.read_ushort(self.score_db_file)
-        perfect_combo = utils.read_bool(self.score_db_file)
-
-        mods = Mod(utils.read_uint(self.score_db_file))
-
-        utils.read_string(self.score_db_file)  # this one always should be empty for some reason, skip it
-        timestamp = utils.read_datetime(self.score_db_file)
-        utils.read_uint(self.score_db_file)  # always should be -1, skip it
-        online_score_id = utils.read_ulong(self.score_db_file)
+        gamemode = GameMode(utils.read_ubyte(self.data_io))
+        score_version = utils.read_uint(self.data_io)
+        beatmap_hash = utils.read_string(self.data_io)
+        username = utils.read_string(self.data_io)
+        replay_hash = utils.read_string(self.data_io)
+
+        count_300 = utils.read_ushort(self.data_io)
+        count_100 = utils.read_ushort(self.data_io)
+        count_50 = utils.read_ushort(self.data_io)
+        count_geki = utils.read_ushort(self.data_io)
+        count_katu = utils.read_ushort(self.data_io)
+        count_miss = utils.read_ushort(self.data_io)
+
+        total_score = utils.read_uint(self.data_io)
+        max_combo = utils.read_ushort(self.data_io)
+        perfect_combo = utils.read_bool(self.data_io)
+
+        mods = Mod(utils.read_uint(self.data_io))
+
+        utils.read_string(self.data_io)  # this one always should be empty for some reason, skip it
+        timestamp = utils.read_datetime(self.data_io)
+        utils.read_uint(self.data_io)  # always should be -1, skip it
+        online_score_id = utils.read_ulong(self.data_io)
 
         additional_info = None
         # if target practice in mods
         if Mod(1 << 23) in mods:
-            additional_info = utils.read_double(self.score_db_file)
+            additional_info = utils.read_double(self.data_io)
 
-        return Score(gamemode, score_version, beatmap_hash, username, replay_hash,
+        return ScoreDB(gamemode, score_version, beatmap_hash, username, replay_hash,
                      count_300, count_100, count_50, count_geki, count_katu, count_miss,
                      total_score, max_combo, perfect_combo, timestamp, online_score_id, additional_info)
 
     def parse_beatmap_scores(self, game_ver: int = 0):
-        beatmap_hash = utils.read_string(self.score_db_file)
-        count_scores = utils.read_uint(self.score_db_file)
-        scores = []
-        for _ in range(count_scores):
-            scores.append(self.parse_score(game_ver))
-
+        beatmap_hash = utils.read_string(self.data_io)
+        count_scores = utils.read_uint(self.data_io)
+        scores = [self.parse_score(game_ver) for _ in range(count_scores)]
         return BeatmapScores(beatmap_hash, count_scores, scores)
-
-
-def parse_scoresdb(scoresdb_file: Union[str, os.PathLike, io.BytesIO]) -> Scoresdb:
-    """
-    Parse scores.db file
-
-    Args
-    ----
-    scoresdb_file: str | os.PathLike | io.BytesIO
-        Path or opened file
-
-    Returns
-    ----
-    scoresdb
-        instance of scoresdb class
-    """
-    if not isinstance(scoresdb_file, io.BytesIO):
-        scoresdb_file = open(scoresdb_file, "rb")
-
-    return _Parser(scoresdb_file).parse()
```

### Comparing `pyosutools-0.2.4/pyosutools/utils.py` & `pyosutools-0.2.5/pyosutools/utils.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.4/pyosutools.egg-info/PKG-INFO` & `pyosutools-0.2.5/pyosutools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.4
+Version: 0.2.5
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.4/pyproject.toml` & `pyosutools-0.2.5/pyproject.toml`

 * *Files identical despite different names*

