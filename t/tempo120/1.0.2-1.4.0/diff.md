# Comparing `tmp/tempo120-1.0.2.tar.gz` & `tmp/tempo120-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\products\tempo120\github - Kopie\dist\.tmp-2kzsfuo4\tempo120-1.0.2.tar", last modified: Fri Aug  4 19:25:25 2023, max compression
+gzip compressed data, was "D:\products\tempo120\github - Kopie\dist\.tmp-y0so325o\tempo120-1.4.0.tar", last modified: Sun Aug  6 17:08:00 2023, max compression
```

## Comparing `tempo120-1.0.2.tar` & `tempo120-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.896750 tempo120-1.0.2/
--rw-rw-rw-   0        0        0    35149 2023-07-11 18:42:22.000000 tempo120-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4879 2023-08-04 19:25:25.895750 tempo120-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3860 2023-08-04 19:25:07.000000 tempo120-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.852741 tempo120-1.0.2/gfx/
--rw-rw-rw-   0        0        0     6941 2023-07-08 15:23:15.000000 tempo120-1.0.2/gfx/car.png
--rw-rw-rw-   0        0        0   107076 2023-07-08 20:36:33.000000 tempo120-1.0.2/gfx/screenshot1.png
--rw-rw-rw-   0        0        0    29421 2023-07-08 20:36:19.000000 tempo120-1.0.2/gfx/screenshot2.png
--rw-rw-rw-   0        0        0    17458 2023-07-08 20:36:06.000000 tempo120-1.0.2/gfx/screenshot3.png
--rw-rw-rw-   0        0        0    16872 2023-07-08 20:35:55.000000 tempo120-1.0.2/gfx/screenshot4.png
--rw-rw-rw-   0        0        0    85199 2023-07-08 19:53:15.000000 tempo120-1.0.2/gfx/title.png
--rw-rw-rw-   0        0        0    30108 2023-08-02 17:31:30.000000 tempo120-1.0.2/gfx/track01.png
-drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.870744 tempo120-1.0.2/muzak/
--rw-rw-rw-   0        0        0    16512 2023-07-23 13:45:55.000000 tempo120-1.0.2/muzak/engine.ogg
--rw-rw-rw-   0        0        0  1955997 2023-07-08 18:57:12.000000 tempo120-1.0.2/muzak/track.ogg
-drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.881749 tempo120-1.0.2/scores/
--rw-rw-rw-   0        0        0       55 2023-07-10 18:10:59.000000 tempo120-1.0.2/scores/scores.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 19:25:25.896750 tempo120-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2069 2023-08-04 19:23:18.000000 tempo120-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.893752 tempo120-1.0.2/tempo120.egg-info/
--rw-rw-rw-   0        0        0     4879 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17472 2023-08-03 15:14:17.000000 tempo120-1.0.2/tempo120.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:08:00.012472 tempo120-1.4.0/
+-rw-rw-rw-   0        0        0    35149 2023-07-11 18:42:22.000000 tempo120-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4879 2023-08-06 17:08:00.011472 tempo120-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3860 2023-08-06 17:07:05.000000 tempo120-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 17:07:59.968463 tempo120-1.4.0/gfx/
+-rw-rw-rw-   0        0        0     6941 2023-07-08 15:23:15.000000 tempo120-1.4.0/gfx/car.png
+-rw-rw-rw-   0        0        0   107076 2023-07-08 20:36:33.000000 tempo120-1.4.0/gfx/screenshot1.png
+-rw-rw-rw-   0        0        0    29421 2023-07-08 20:36:19.000000 tempo120-1.4.0/gfx/screenshot2.png
+-rw-rw-rw-   0        0        0    17458 2023-07-08 20:36:06.000000 tempo120-1.4.0/gfx/screenshot3.png
+-rw-rw-rw-   0        0        0    16872 2023-07-08 20:35:55.000000 tempo120-1.4.0/gfx/screenshot4.png
+-rw-rw-rw-   0        0        0    85199 2023-07-08 19:53:15.000000 tempo120-1.4.0/gfx/title.png
+-rw-rw-rw-   0        0        0    30108 2023-08-02 17:31:30.000000 tempo120-1.4.0/gfx/track01.png
+drwxrwxrwx   0        0        0        0 2023-08-06 17:07:59.989467 tempo120-1.4.0/muzak/
+-rw-rw-rw-   0        0        0    16512 2023-07-23 13:45:55.000000 tempo120-1.4.0/muzak/engine.ogg
+-rw-rw-rw-   0        0        0  1955997 2023-07-08 18:57:12.000000 tempo120-1.4.0/muzak/track.ogg
+drwxrwxrwx   0        0        0        0 2023-08-06 17:07:59.999470 tempo120-1.4.0/scores/
+-rw-rw-rw-   0        0        0       55 2023-07-10 18:10:59.000000 tempo120-1.4.0/scores/scores.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 17:08:00.012472 tempo120-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2069 2023-08-06 16:30:32.000000 tempo120-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:08:00.010473 tempo120-1.4.0/tempo120.egg-info/
+-rw-rw-rw-   0        0        0     4879 2023-08-06 17:07:59.000000 tempo120-1.4.0/tempo120.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-08-06 17:07:59.000000 tempo120-1.4.0/tempo120.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 17:07:59.000000 tempo120-1.4.0/tempo120.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-06 17:07:59.000000 tempo120-1.4.0/tempo120.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-08-06 17:07:59.000000 tempo120-1.4.0/tempo120.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17510 2023-08-06 16:52:45.000000 tempo120-1.4.0/tempo120.py
```

### Comparing `tempo120-1.0.2/LICENSE` & `tempo120-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/PKG-INFO` & `tempo120-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempo120
-Version: 1.0.2
+Version: 1.4.0
 Summary: A party car racing game
 Home-page: https://dkrajzew.itch.io/tempo120
 Download-URL: http://pypi.python.org/pypi/tempo120
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/dkrajzew/tempo120
```

### Comparing `tempo120-1.0.2/README.md` & `tempo120-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/car.png` & `tempo120-1.4.0/gfx/car.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/screenshot1.png` & `tempo120-1.4.0/gfx/screenshot1.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/screenshot2.png` & `tempo120-1.4.0/gfx/screenshot2.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/screenshot3.png` & `tempo120-1.4.0/gfx/screenshot3.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/screenshot4.png` & `tempo120-1.4.0/gfx/screenshot4.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/title.png` & `tempo120-1.4.0/gfx/title.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/gfx/track01.png` & `tempo120-1.4.0/gfx/track01.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/muzak/engine.ogg` & `tempo120-1.4.0/muzak/engine.ogg`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/muzak/track.ogg` & `tempo120-1.4.0/muzak/track.ogg`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.2/setup.py` & `tempo120-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # --- definitions ---------------------------------------------------
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tempo120",
-    version="1.0.2",
+    version="1.4.0",
     author="dkrajzew",
     author_email="d.krajzewicz@gmail.com",
     description="A party car racing game",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://dkrajzew.itch.io/tempo120',
     download_url='http://pypi.python.org/pypi/tempo120',
```

### Comparing `tempo120-1.0.2/tempo120.egg-info/PKG-INFO` & `tempo120-1.4.0/tempo120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempo120
-Version: 1.0.2
+Version: 1.4.0
 Summary: A party car racing game
 Home-page: https://dkrajzew.itch.io/tempo120
 Download-URL: http://pypi.python.org/pypi/tempo120
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/dkrajzew/tempo120
```

### Comparing `tempo120-1.0.2/tempo120.py` & `tempo120-1.4.0/tempo120.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,40 +82,41 @@
     "scores.txt" each entry is stored in one line, using tab ('\t') to divide the name 
     and the time.
     
     The list may include up to 15 entries. The player's name may be up to 16 characters
     long.
     """
     
-    def __init__(self):
+    def __init__(self, path):
         """Loads the scores using the load method."""
+        self._path = path
         self.load()
         
 
     def load(self):
         """Loads the scores.
         
         Loads scores from "scores.txt", sorts them by the needed time and prunes
         them to the maximum length of 15 entries.
         """
         scores = []
         try:
-            with open(os.path.join(os.path.dirname(__file__), "scores", "scores.txt")) as fd:
+            with open(os.path.join(self._path, "scores", "scores.txt")) as fd:
                 for l in fd:
                     name, t = l.strip().split("\t")
                     scores.append([name, int(t)])
             scores.sort(key=lambda x: x[1])
         except: pass
         self._scores = scores[:15]
         
         
     def save(self):
         """Saves the scores into "scores.txt"
         """
-        fd = open(os.path.join(os.path.dirname(__file__), "scores", "scores.txt"), "w")
+        fd = open(os.path.join(self._path, "scores", "scores.txt"), "w")
         for s in self._scores:
             fd.write("%s\t%s\n" % (s[0], s[1]))    
         fd.close()
 
 
     def add(self, name, t):
         """Adds an entry to the scores
@@ -307,28 +308,31 @@
 
 class Game:
     """The game class"""
     
     def __init__(self):
         """Initialises the game
         """
-        self._car_image = pygame.image.load(os.path.join(os.path.dirname(__file__), "gfx", "car.png"))
-        self._title_image = pygame.image.load(os.path.join(os.path.dirname(__file__), "gfx", "title.png"))
-        track_image = pygame.image.load(os.path.join(os.path.dirname(__file__), "gfx", "track01.png"))
-        self._theme_sound = pygame.mixer.Sound(os.path.join(os.path.dirname(__file__), "muzak", "track.ogg"))
+        path = os.path.dirname(__file__)
+        if not os.path.exists(os.path.join(path, "gfx", "car.png")):
+            path = "."
+        self._car_image = pygame.image.load(os.path.join(path, "gfx", "car.png"))
+        self._title_image = pygame.image.load(os.path.join(path, "gfx", "title.png"))
+        track_image = pygame.image.load(os.path.join(path, "gfx", "track01.png"))
+        self._theme_sound = pygame.mixer.Sound(os.path.join(path, "muzak", "track.ogg"))
         self._theme_sound.set_volume(1)
-        self._engine_sound = pygame.mixer.Sound(os.path.join(os.path.dirname(__file__), "muzak", "engine.ogg"))
+        self._engine_sound = pygame.mixer.Sound(os.path.join(path, "muzak", "engine.ogg"))
         self._engine_sound.set_volume(.2)
         self._font = pygame.font.SysFont(None, 48)
         self._height = track_image.get_height()
         self._width = track_image.get_width()
         self._track = Track(track_image)
         self._theme_channel = pygame.mixer.Channel(0)
         self._engine_channel = pygame.mixer.Channel(1)
-        self._scores = Scores()
+        self._scores = Scores(path)
         self._start_time = 0
         self._last_entered_time = 0
         self._quit = False
         self._pressed_keys = set()
         self.init()
```

