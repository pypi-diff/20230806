# Comparing `tmp/rayter_generator-1.0.8.tar.gz` & `tmp/rayter_generator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayter_generator-1.0.8.tar", last modified: Sat Mar 11 09:10:03 2023, max compression
+gzip compressed data, was "rayter_generator-1.0.9.tar", last modified: Sun Mar 12 14:47:34 2023, max compression
```

## Comparing `rayter_generator-1.0.8.tar` & `rayter_generator-1.0.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.730723 rayter_generator-1.0.8/rayter_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/players.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/render.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.730723 rayter_generator-1.0.8/rayter_generator/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/rayter_generator/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/static/css/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/static/css/normalize.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/rayter_generator/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/static/img/arrow_down.gif
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/static/img/arrow_up.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/rayter_generator/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/static/js/charts.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/rayter_generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/templates/game.html
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/rayter_generator/templates/player.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/rayter_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-11 09:10:03.000000 rayter_generator-1.0.8/rayter_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-11 09:10:03.000000 rayter_generator-1.0.8/rayter_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 09:10:03.000000 rayter_generator-1.0.8/rayter_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-11 09:10:03.000000 rayter_generator-1.0.8/rayter_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-11 09:10:03.000000 rayter_generator-1.0.8/rayter_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-11 09:10:03.000000 rayter_generator-1.0.8/rayter_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 09:10:03.734722 rayter_generator-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-03-11 09:09:54.000000 rayter_generator-1.0.8/tests/test_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.919498 rayter_generator-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-12 14:47:34.919498 rayter_generator-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.915498 rayter_generator-1.0.9/rayter_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/global_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.915498 rayter_generator-1.0.9/rayter_generator/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.915498 rayter_generator-1.0.9/rayter_generator/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/static/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/static/css/normalize.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.915498 rayter_generator-1.0.9/rayter_generator/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/static/img/arrow_down.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/static/img/arrow_up.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.915498 rayter_generator-1.0.9/rayter_generator/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/static/js/charts.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.919498 rayter_generator-1.0.9/rayter_generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/templates/game.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/rayter_generator/templates/player.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.915498 rayter_generator-1.0.9/rayter_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-12 14:47:34.000000 rayter_generator-1.0.9/rayter_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-12 14:47:34.000000 rayter_generator-1.0.9/rayter_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 14:47:34.000000 rayter_generator-1.0.9/rayter_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-12 14:47:34.000000 rayter_generator-1.0.9/rayter_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-12 14:47:34.000000 rayter_generator-1.0.9/rayter_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-12 14:47:34.000000 rayter_generator-1.0.9/rayter_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 14:47:34.919498 rayter_generator-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 14:47:34.919498 rayter_generator-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-03-12 14:47:26.000000 rayter_generator-1.0.9/tests/test_generator.py
```

### Comparing `rayter_generator-1.0.8/rayter_generator/env.py` & `rayter_generator-1.0.9/rayter_generator/env.py`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator/main.py` & `rayter_generator-1.0.9/rayter_generator/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 import os
 import pathlib
 import shutil
 import sys
 
 from .env import GeneratorEnvironment
-from .games import parse_game_file
-from .players import get_players
+from .games import get_games
+from .players import get_all_players
 from .render import render_game_page, render_index_page, render_player_page, render_game_json, render_player_image
-
+from .global_chart import get_global_chart
 
 def _main(args):
     arg_parser = argparse.ArgumentParser(
         description="Generate Rayter website from game files",
     )
     arg_parser.add_argument(
         "--games-path",
@@ -44,30 +44,22 @@
         env = GeneratorEnvironment(
             games_path=args.games_path,
             output_path=args.output,
             config_path=args.config,
             players_path=args.players,
         )
 
-        games = []
-        # Create game list from game files
-        for filename in os.listdir(env.games_path):
-            if not filename.endswith(".txt"):
-                continue
-            if os.path.isdir(filename):
-                continue
-
-            # remove .txt from filename
-            slug = filename[:-4]
-            game = parse_game_file(os.path.join(env.games_path, filename), slug)
-            if game is not None:
-                games.append(game)
+        # get games
+        games = get_games(env)
+
+        # get players
+        players = get_all_players(games, env)
 
-        # Get players
-        players = get_players(games, env)
+        # get global chart
+        global_chart = get_global_chart(games)
 
         # render player images, with the side effect of adding image filenames to players
         for player in players.values():
             render_player_image(env, player)
 
         # render player pages
         for player in players.values():
@@ -78,27 +70,28 @@
             render_game_page(env, game, players)
 
         # render game json
         for game in games:
             render_game_json(env, game)
 
         # render index page
-        render_index_page(env, games, players)
+        render_index_page(env, games, players, global_chart)
 
         # recursively copy static files to output directory
         print("Copying static files")
         shutil.copytree(
             os.path.join(env.root_path, "static"),
             os.path.join(env.output_path, "static"),
             dirs_exist_ok=True,
         )
     except FileNotFoundError as e:
         sys.stderr.write(f"Error: {e.strerror} ({e.filename})\n")
         sys.exit(1)
 
 
+
 def main():
     _main(sys.argv[1:])
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `rayter_generator-1.0.8/rayter_generator/players.py` & `rayter_generator-1.0.9/rayter_generator/players.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import hashlib
 import urllib
 
 def create_player_from_games(name, games):
-
     ratings = []
 
     for game in games:
         players = game["ratings"]
         placement = 0
         for player_name, _0, rating, _1 in players:
             if player_name == name:
                 ratings.append(
                     (game["slug"], game["game_name"], rating, placement))
             placement += 1
 
     # Sort ratings by rating, best first. The actual rating is the third element in the tuple.
     ratings.sort(key=lambda rating: int(rating[2]), reverse=True)
 
-    # FIXME: (?)
-    # All games are traversed twice, first in the loop above and then inside
-    # get_games_and_toplist(), maybe they can be combined?
-# (games, global_chart) = get_games_and_toplist()
-
     player = {
         "name": name,
         "slug": name,
         "ratings": ratings,
     }
 
     return player
@@ -46,18 +40,19 @@
             's': str(gravatar_size)
         })
         return gravatar_url
     else:
         return None
 
 
-def get_players(games, env):
+def get_all_players(games, env):
     players = {}
     players_metadata = env.players_metadata
 
+    # Collect all players from all games
     for game in games:
         for player in game["ratings"]:
             name = player[0]
             if not name in players:
                 players[name] = create_player_from_games(name, games)
 
     # Overwrite generic player values with player metadata from file
@@ -65,13 +60,14 @@
         for player_name in players_metadata.keys():
             # If player exists in players, update it with all values in the player's metadata
             if player_name in players:
                 player_metadata = players_metadata[player_name]
                 players[player_name].update(player_metadata)
 
         # For every player, if they have no image url, try to create one from their metadata
+        # FIXME: Should this be moved into create_player_from_games()?
         for player_name in players.keys():
             player = players[player_name]
             if not 'imageUrl' in player:
                 player['imageUrl'] = make_image_url(player)
 
     return players
```

### Comparing `rayter_generator-1.0.8/rayter_generator/render.py` & `rayter_generator-1.0.9/rayter_generator/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 def render_player_page(env, player):
     filename = os.path.join(env.output_path, 'player', player['slug'], 'index.html')
     env.render_template("player.html", {
         "player": player,
         "STATIC_URL": "../../static/",
     }, output_path=filename)
 
+# FIXME: This function is quite long. Should the main parts be broken out into
+#        a separate file?
 def render_player_image(env, player):
     dir_path = os.path.join(env.output_path, 'player', player['slug'])
     # Ensure the player folder exists.
     os.makedirs(dir_path, exist_ok=True)
 
     if player['imageUrl'] is None:
         # If there is no image, generate a random avatar using py_avataaars.
@@ -114,17 +116,17 @@
             new_path = os.path.join(dir_path, filename)
             print("Mving 2 " + new_path)
             os.rename(file_path, new_path)
 
     # Update the player record with the new filename.
     player['image'] = filename
 
-def render_index_page(env, games, players):
+def render_index_page(env, games, players, global_chart):
     games.sort(key=lambda g: g["count"], reverse=True)
     filename = os.path.join(env.output_path, 'index.html')
     env.render_template("index.html", {
         "games": games,
         "players": players,
-        "global_chart": [],
+        "global_chart": global_chart,
         "log": [],
         "STATIC_URL": "static/",
     }, output_path=filename)
```

### Comparing `rayter_generator-1.0.8/rayter_generator/static/css/main.css` & `rayter_generator-1.0.9/rayter_generator/static/css/main.css`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator/static/css/normalize.css` & `rayter_generator-1.0.9/rayter_generator/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator/static/js/charts.js` & `rayter_generator-1.0.9/rayter_generator/static/js/charts.js`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator/templates/base.html` & `rayter_generator-1.0.9/rayter_generator/templates/base.html`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator/templates/game.html` & `rayter_generator-1.0.9/rayter_generator/templates/game.html`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator/templates/index.html` & `rayter_generator-1.0.9/rayter_generator/templates/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -54,22 +54,25 @@
             <h2>Overall placement</h2>
             <table>
                 <tr>
                     <th>Position</th>
                     <th>Name</th>
                     <th>Average placement</th>
                 </tr>
-                {% for name, rating in global_chart %}
+                {% for placement in global_chart %}
+                    {% set name = placement["player_name"] %}
+                    {% set rating = placement["average"] %}
                     {% if name in players and 'displayName' in players[name] %}
                         {% set display_name = players[name]['displayName'] %}
                     {% else %}
                         {% set display_name = name %}
                     {% endif %}
-                    {% if name in players and 'imageUrl' in players[name] %}
-                        {% set image_url = players[name]['imageUrl'] %}
+                    {% if name in players and 'image' in players[name] %}
+                        {% set image_path = "../player/" + players[name]["name"] %}
+                        {% set image_url = image_path + "/" + players[name]["image"] %}
                     {% endif %}
                     <tr>
                         <td class="position">{{ loop.index }}</td>
                         <td class="name avatar">
                             {% if image_url %}
                                 <img class="player-image" src="{{image_url}}">
                             {% endif %}
@@ -94,23 +97,9 @@
             </p>
             <p>
                 The average is weighted, meaning
                 that a game where the player has played many matches will count more towards
                 the average than a match where the player only played a few matches.
             </p>
         </div>
-
-        <div id="event-log">
-            <h2>Events</h2>
-            <table>
-                <tr>
-                    <th>Event</th>
-                </tr>
-                {% for message in log %}
-                    <tr>
-                        <td >{{ message }}</td>
-                    </tr>
-                {% endfor %}
-            </table>
-        </div>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -20,11 +20,8 @@
 100% = first in all games, 0% = last in all games.
 The global chart includes only players with at least three games played and it
 only counts placements in games where the player has played at least three
 matches.
 The average is weighted, meaning that a game where the player has played many
 matches will count more towards the average than a match where the player only
 played a few matches.
-***** Events *****
-Event
-{{ message }}
 {% endblock %}
```

### Comparing `rayter_generator-1.0.8/rayter_generator/templates/player.html` & `rayter_generator-1.0.9/rayter_generator/templates/player.html`

 * *Files identical despite different names*

### Comparing `rayter_generator-1.0.8/rayter_generator.egg-info/SOURCES.txt` & `rayter_generator-1.0.9/rayter_generator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 pyproject.toml
 setup.py
 rayter_generator/__init__.py
 rayter_generator/env.py
 rayter_generator/games.py
+rayter_generator/global_chart.py
 rayter_generator/main.py
 rayter_generator/players.py
 rayter_generator/render.py
 rayter_generator/settings.py
 rayter_generator.egg-info/PKG-INFO
 rayter_generator.egg-info/SOURCES.txt
 rayter_generator.egg-info/dependency_links.txt
```

### Comparing `rayter_generator-1.0.8/tests/test_generator.py` & `rayter_generator-1.0.9/tests/test_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 
 class TestGenerator(TestCase):
     def setUp(self):
         super().setUp()
         self.games_path = TemporaryDirectory()
         self.output_path = TemporaryDirectory()
 
-        with open(os.path.join(self.games_path.name, "scrabble.txt"), "w") as f:
+        with open(os.path.join(self.games_path.name, "babble.txt"), "w") as f:
             f.write(dedent("""
-                # Scrabble
-                game_name Scrabble
+                game_name Babble
 
                 game 2023-02-20 17:06
                 PlayerOne   350
                 PlayerTwo   320
 
                 game 2023-02-24 13:00
                 PlayerOne   346
                 PlayerTwo   390
+                PlayerThree 94
+
+                game 2023-03-12 15:00
+                PlayerOne   512
+                PlayerTwo   100
             """))
 
         with open(os.path.join(self.output_path.name, "players_metadata.json"), "w") as f:
             f.write(dedent("""
                 {
                     "PlayerOne": {
                         "displayName": "Player One DisplayName"
@@ -46,27 +50,27 @@
     @patch("sys.stdout", new_callable=StringIO)
     def test_generate_website(self, mock_stdout, mock_stderr):
         _main([
             "--games-path", self.games_path.name,
             "--output", self.output_path.name,
         ])
         self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "index.html")))
-        self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "scrabble", "index.html")))
+        self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "babble", "index.html")))
 
         with open(os.path.join(self.output_path.name, "index.html"), "r") as f:
             contents = f.read()
-        self.assertIn("Scrabble", contents)
+        self.assertIn("Babble", contents)
 
-        with open(os.path.join(self.output_path.name, "scrabble", "index.html"), "r") as f:
+        with open(os.path.join(self.output_path.name, "babble", "index.html"), "r") as f:
             contents = f.read()
         self.assertIn("PlayerOne", contents)
 
         mock_stdout.seek(0)
         mock_stderr.seek(0)
-        self.assertIn("scrabble/index.html", mock_stdout.read())
+        self.assertIn("babble/index.html", mock_stdout.read())
 
     @patch("sys.stderr", new_callable=StringIO)
     @patch("sys.stdout", new_callable=StringIO)
     def test_generate_website_with_config(self, mock_stdout, mock_stderr):
         with NamedTemporaryFile() as config_file:
             config_file.write(dedent("""
                 site_name = "TestName"
@@ -109,15 +113,15 @@
         _main([
             "--games-path", self.games_path.name,
             "--output", self.output_path.name,
         ])
 
         with open(os.path.join(self.output_path.name, "player", "PlayerOne", "index.html"), "r") as f:
             contents = f.read()
-        self.assertIn("Scrabble", contents)
+        self.assertIn("Babble", contents)
 
     @patch("sys.stderr", new_callable=StringIO)
     @patch("sys.stdout", new_callable=StringIO)
     def test_player_metadata(self, mock_stdout, mock_stderr):
         _main([
             "--games-path", self.games_path.name,
             "--output", self.output_path.name,
@@ -131,17 +135,17 @@
     @patch("sys.stderr", new_callable=StringIO)
     @patch("sys.stdout", new_callable=StringIO)
     def test_generate_game_json(self, mock_stdout, mock_stderr):
         _main([
             "--games-path", self.games_path.name,
             "--output", self.output_path.name,
         ])
-        self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "scrabble", "game.json")))
+        self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "babble", "game.json")))
 
-        with open(os.path.join(self.output_path.name, "scrabble", "game.json"), "r") as f:
+        with open(os.path.join(self.output_path.name, "babble", "game.json"), "r") as f:
             contents = f.read()
         self.assertIn("PlayerOne", contents)
         self.assertIn("rating_history", contents)
 
 
     @patch("sys.stderr", new_callable=StringIO)
     @patch("sys.stdout", new_callable=StringIO)
@@ -149,7 +153,59 @@
         _main([
             "--games-path", self.games_path.name,
             "--output", self.output_path.name,
         ])
 
         self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "player", "PlayerOne", "image.png")))
         self.assertTrue(os.path.exists(os.path.join(self.output_path.name, "player", "PlayerTwo", "image.png")))
+
+    @patch("sys.stderr", new_callable=StringIO)
+    @patch("sys.stdout", new_callable=StringIO)
+    def test_global_chart(self, mock_stdout, mock_stderr):
+        with open(os.path.join(self.games_path.name, "catch_the_rabbit.txt"), "w") as f:
+            f.write(dedent("""
+                game_name Catch the Rabbit
+
+                game 2023-02-20 17:06
+                PlayerOne   1
+                PlayerTwo   10
+                PlayerThree 0
+
+                game 2023-02-24 13:00
+                PlayerOne   4
+                PlayerTwo   2
+
+                game 2023-03-12 15:00
+                PlayerOne   2
+                PlayerTwo   23
+            """))
+
+        with open(os.path.join(self.games_path.name, "reverse_chess.txt"), "w") as f:
+            f.write(dedent("""
+                game_name Reverse Chess
+
+                game 2023-02-20 17:06
+                PlayerOne   1
+                PlayerTwo   10
+
+                game 2023-02-24 13:00
+                PlayerOne   4
+                PlayerTwo   2
+
+                game 2023-03-12 15:00
+                PlayerOne   2
+                PlayerTwo   23
+                PlayerThree 1
+            """))
+
+        _main([
+            "--games-path", self.games_path.name,
+            "--output", self.output_path.name,
+        ])
+
+        with open(os.path.join(self.output_path.name, "index.html"), "r") as f:
+            contents = f.read()
+        self.assertIn('class="position"', contents)
+        self.assertIn('PlayerOne', contents)
+        self.assertIn('PlayerTwo', contents)
+        self.assertNotIn('PlayerThree', contents)
+
```

