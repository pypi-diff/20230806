# Comparing `tmp/dgisim-0.2.dev2.tar.gz` & `tmp/dgisim-0.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgisim-0.2.dev2.tar", last modified: Sun Jul  9 16:37:52 2023, max compression
+gzip compressed data, was "dgisim-0.2.dev3.tar", last modified: Wed Jul 26 23:22:17 2023, max compression
```

## Comparing `dgisim-0.2.dev2.tar` & `dgisim-0.2.dev3.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.360333 dgisim-0.2.dev2/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1065 2023-02-15 18:18:52.000000 dgisim-0.2.dev2/LICENSE
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     7052 2023-07-09 16:37:52.359887 dgisim-0.2.dev2/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4465 2023-07-09 02:33:20.000000 dgisim-0.2.dev2/README.md
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.313663 dgisim-0.2.dev2/dgisim/
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.326321 dgisim-0.2.dev2/dgisim/src/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1278 2023-07-09 12:06:43.000000 dgisim-0.2.dev2/dgisim/src/__init__.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.329693 dgisim-0.2.dev2/dgisim/src/action/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:00.000000 dgisim-0.2.dev2/dgisim/src/action/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6827 2023-07-09 12:07:24.000000 dgisim-0.2.dev2/dgisim/src/action/action.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3475 2023-07-09 12:06:32.000000 dgisim-0.2.dev2/dgisim/src/action/action_generator.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    15596 2023-07-09 13:25:48.000000 dgisim-0.2.dev2/dgisim/src/action/action_generator_generator.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      276 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/action/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      647 2023-07-09 12:05:48.000000 dgisim-0.2.dev2/dgisim/src/action/types.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    11779 2023-07-09 12:06:32.000000 dgisim-0.2.dev2/dgisim/src/agents.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.331938 dgisim-0.2.dev2/dgisim/src/card/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:07.000000 dgisim-0.2.dev2/dgisim/src/card/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    34162 2023-07-09 16:26:30.000000 dgisim-0.2.dev2/dgisim/src/card/card.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4090 2023-07-09 15:18:03.000000 dgisim-0.2.dev2/dgisim/src/card/cards.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      686 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/card/cards_set.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.335249 dgisim-0.2.dev2/dgisim/src/character/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:12.000000 dgisim-0.2.dev2/dgisim/src/character/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    24957 2023-07-09 12:07:37.000000 dgisim-0.2.dev2/dgisim/src/character/character.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6586 2023-07-09 14:09:01.000000 dgisim-0.2.dev2/dgisim/src/character/characters.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      459 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/character/characters_set.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      683 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/character/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    11920 2023-07-09 12:06:32.000000 dgisim-0.2.dev2/dgisim/src/cli.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    10222 2023-07-09 12:05:48.000000 dgisim-0.2.dev2/dgisim/src/dices.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.339024 dgisim-0.2.dev2/dgisim/src/effect/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:16.000000 dgisim-0.2.dev2/dgisim/src/effect/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    44454 2023-07-09 13:30:24.000000 dgisim-0.2.dev2/dgisim/src/effect/effect.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2181 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/effect/effect_stack.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      802 2023-07-09 12:07:37.000000 dgisim-0.2.dev2/dgisim/src/effect/effects_template.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      720 2023-07-09 12:07:37.000000 dgisim-0.2.dev2/dgisim/src/effect/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1247 2023-07-09 12:07:24.000000 dgisim-0.2.dev2/dgisim/src/effect/structs.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5749 2023-07-09 12:05:57.000000 dgisim-0.2.dev2/dgisim/src/element.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      963 2023-07-09 12:06:32.000000 dgisim-0.2.dev2/dgisim/src/event.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     7122 2023-07-09 13:42:37.000000 dgisim-0.2.dev2/dgisim/src/game_state_machine.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.341176 dgisim-0.2.dev2/dgisim/src/helper/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       86 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/helper/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4623 2023-07-09 11:31:59.000000 dgisim-0.2.dev2/dgisim/src/helper/hashable_dict.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     9098 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/helper/level_print.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1284 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/helper/quality_of_life.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3827 2023-07-09 12:17:19.000000 dgisim-0.2.dev2/dgisim/src/mode.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.342311 dgisim-0.2.dev2/dgisim/src/phase/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       20 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/phase/__init__.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.346555 dgisim-0.2.dev2/dgisim/src/phase/default/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      397 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/phase/default/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    17213 2023-07-09 12:28:07.000000 dgisim-0.2.dev2/dgisim/src/phase/default/action_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6166 2023-07-09 12:27:43.000000 dgisim-0.2.dev2/dgisim/src/phase/default/card_select_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     7100 2023-07-09 12:28:32.000000 dgisim-0.2.dev2/dgisim/src/phase/default/end_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      906 2023-07-09 12:06:32.000000 dgisim-0.2.dev2/dgisim/src/phase/default/game_end_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5972 2023-07-09 12:27:57.000000 dgisim-0.2.dev2/dgisim/src/phase/default/roll_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4429 2023-07-09 12:27:34.000000 dgisim-0.2.dev2/dgisim/src/phase/default/starting_hand_select_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1366 2023-07-09 12:33:52.000000 dgisim-0.2.dev2/dgisim/src/phase/phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      572 2023-07-09 13:17:13.000000 dgisim-0.2.dev2/dgisim/src/player_agent.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.349350 dgisim-0.2.dev2/dgisim/src/state/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:04:22.000000 dgisim-0.2.dev2/dgisim/src/state/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      983 2023-07-09 12:06:43.000000 dgisim-0.2.dev2/dgisim/src/state/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    20470 2023-07-09 13:01:07.000000 dgisim-0.2.dev2/dgisim/src/state/game_state.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    11176 2023-07-09 13:08:35.000000 dgisim-0.2.dev2/dgisim/src/state/player_state.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.354196 dgisim-0.2.dev2/dgisim/src/status/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:35.000000 dgisim-0.2.dev2/dgisim/src/status/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      682 2023-07-09 12:07:06.000000 dgisim-0.2.dev2/dgisim/src/status/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    35182 2023-07-09 16:06:07.000000 dgisim-0.2.dev2/dgisim/src/status/status.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     8426 2023-07-09 12:07:30.000000 dgisim-0.2.dev2/dgisim/src/status/status_processing.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2849 2023-07-09 15:46:46.000000 dgisim-0.2.dev2/dgisim/src/status/statuses.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      180 2023-07-09 00:17:13.000000 dgisim-0.2.dev2/dgisim/src/status/types.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.356632 dgisim-0.2.dev2/dgisim/src/summon/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:39.000000 dgisim-0.2.dev2/dgisim/src/summon/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5106 2023-07-09 12:07:37.000000 dgisim-0.2.dev2/dgisim/src/summon/summon.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2621 2023-07-09 16:11:56.000000 dgisim-0.2.dev2/dgisim/src/summon/summons.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.359002 dgisim-0.2.dev2/dgisim/src/support/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:43.000000 dgisim-0.2.dev2/dgisim/src/support/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3237 2023-07-09 12:07:30.000000 dgisim-0.2.dev2/dgisim/src/support/support.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4135 2023-07-09 16:26:30.000000 dgisim-0.2.dev2/dgisim/src/support/supports.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 16:37:52.319403 dgisim-0.2.dev2/dgisim.egg-info/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     7052 2023-07-09 16:37:52.000000 dgisim-0.2.dev2/dgisim.egg-info/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2013 2023-07-09 16:37:52.000000 dgisim-0.2.dev2/dgisim.egg-info/SOURCES.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2023-07-09 16:37:52.000000 dgisim-0.2.dev2/dgisim.egg-info/dependency_links.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2023-07-09 16:37:52.000000 dgisim-0.2.dev2/dgisim.egg-info/requires.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        7 2023-07-09 16:37:52.000000 dgisim-0.2.dev2/dgisim.egg-info/top_level.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1475 2023-07-09 16:36:54.000000 dgisim-0.2.dev2/pyproject.toml
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2023-07-09 16:37:52.360446 dgisim-0.2.dev2/setup.cfg
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.555092 dgisim-0.2.dev3/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1065 2023-02-15 18:18:52.000000 dgisim-0.2.dev3/LICENSE
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7408 2023-07-26 23:22:17.554776 dgisim-0.2.dev3/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4821 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/README.md
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.522017 dgisim-0.2.dev3/dgisim/
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.532520 dgisim-0.2.dev3/dgisim/src/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1278 2023-07-09 16:43:29.000000 dgisim-0.2.dev3/dgisim/src/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.535555 dgisim-0.2.dev3/dgisim/src/action/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:00.000000 dgisim-0.2.dev3/dgisim/src/action/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5912 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/action/action.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3172 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/action/action_generator.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    15624 2023-07-17 01:23:00.000000 dgisim-0.2.dev3/dgisim/src/action/action_generator_generator.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      276 2023-07-09 00:17:13.000000 dgisim-0.2.dev3/dgisim/src/action/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      647 2023-07-09 12:05:48.000000 dgisim-0.2.dev3/dgisim/src/action/types.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    12432 2023-07-16 17:37:45.000000 dgisim-0.2.dev3/dgisim/src/agents.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.536965 dgisim-0.2.dev3/dgisim/src/card/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:07.000000 dgisim-0.2.dev3/dgisim/src/card/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    49215 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/card/card.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4184 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/card/cards.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1025 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/card/cards_set.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.538676 dgisim-0.2.dev3/dgisim/src/character/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-23 00:17:31.000000 dgisim-0.2.dev3/dgisim/src/character/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    40354 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/character/character.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6902 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/character/characters.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      521 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/character/characters_set.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      980 2023-07-16 17:37:45.000000 dgisim-0.2.dev3/dgisim/src/character/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11920 2023-07-20 21:47:13.000000 dgisim-0.2.dev3/dgisim/src/cli.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    10225 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/dices.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.541144 dgisim-0.2.dev3/dgisim/src/effect/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:16.000000 dgisim-0.2.dev3/dgisim/src/effect/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    47788 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/effect/effect.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2127 2023-07-13 21:12:02.000000 dgisim-0.2.dev3/dgisim/src/effect/effect_stack.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1259 2023-07-22 22:25:32.000000 dgisim-0.2.dev3/dgisim/src/effect/effects_template.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1133 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/effect/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1753 2023-07-20 23:24:41.000000 dgisim-0.2.dev3/dgisim/src/effect/structs.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6236 2023-07-20 23:24:41.000000 dgisim-0.2.dev3/dgisim/src/element.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2057 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/event.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7122 2023-07-09 16:43:29.000000 dgisim-0.2.dev3/dgisim/src/game_state_machine.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.543384 dgisim-0.2.dev3/dgisim/src/helper/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       86 2023-07-09 00:17:13.000000 dgisim-0.2.dev3/dgisim/src/helper/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4703 2023-07-13 21:12:02.000000 dgisim-0.2.dev3/dgisim/src/helper/hashable_dict.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     9100 2023-07-22 22:25:32.000000 dgisim-0.2.dev3/dgisim/src/helper/level_print.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1283 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/helper/quality_of_life.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3902 2023-07-20 23:24:41.000000 dgisim-0.2.dev3/dgisim/src/mode.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.544238 dgisim-0.2.dev3/dgisim/src/phase/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       20 2023-07-09 00:17:13.000000 dgisim-0.2.dev3/dgisim/src/phase/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.545254 dgisim-0.2.dev3/dgisim/src/phase/all_omni/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      442 2023-07-10 22:51:12.000000 dgisim-0.2.dev3/dgisim/src/phase/all_omni/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1019 2023-07-10 22:51:12.000000 dgisim-0.2.dev3/dgisim/src/phase/all_omni/roll_phase.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.549217 dgisim-0.2.dev3/dgisim/src/phase/default/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      397 2023-07-09 00:17:13.000000 dgisim-0.2.dev3/dgisim/src/phase/default/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    16705 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/phase/default/action_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6028 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/phase/default/card_select_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6518 2023-07-16 17:37:45.000000 dgisim-0.2.dev3/dgisim/src/phase/default/end_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      736 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/phase/default/game_end_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5596 2023-07-20 23:24:41.000000 dgisim-0.2.dev3/dgisim/src/phase/default/roll_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5117 2023-07-22 22:25:32.000000 dgisim-0.2.dev3/dgisim/src/phase/default/starting_hand_select_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1366 2023-07-09 16:43:29.000000 dgisim-0.2.dev3/dgisim/src/phase/phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      572 2023-07-09 16:43:29.000000 dgisim-0.2.dev3/dgisim/src/player_agent.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.550917 dgisim-0.2.dev3/dgisim/src/state/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:04:22.000000 dgisim-0.2.dev3/dgisim/src/state/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1003 2023-07-16 17:37:45.000000 dgisim-0.2.dev3/dgisim/src/state/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    21056 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/state/game_state.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11480 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/state/player_state.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.552352 dgisim-0.2.dev3/dgisim/src/status/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:35.000000 dgisim-0.2.dev3/dgisim/src/status/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      822 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/status/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    61431 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/status/status.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     8450 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/status/status_processing.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4364 2023-07-22 14:32:38.000000 dgisim-0.2.dev3/dgisim/src/status/statuses.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.553510 dgisim-0.2.dev3/dgisim/src/summon/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:39.000000 dgisim-0.2.dev3/dgisim/src/summon/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    13718 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/summon/summon.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3070 2023-07-20 23:24:41.000000 dgisim-0.2.dev3/dgisim/src/summon/summons.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.554353 dgisim-0.2.dev3/dgisim/src/support/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:43.000000 dgisim-0.2.dev3/dgisim/src/support/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3335 2023-07-26 23:14:20.000000 dgisim-0.2.dev3/dgisim/src/support/support.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4525 2023-07-14 23:05:33.000000 dgisim-0.2.dev3/dgisim/src/support/supports.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-26 23:22:17.527639 dgisim-0.2.dev3/dgisim.egg-info/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7408 2023-07-26 23:22:17.000000 dgisim-0.2.dev3/dgisim.egg-info/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2064 2023-07-26 23:22:17.000000 dgisim-0.2.dev3/dgisim.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2023-07-26 23:22:17.000000 dgisim-0.2.dev3/dgisim.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2023-07-26 23:22:17.000000 dgisim-0.2.dev3/dgisim.egg-info/requires.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        7 2023-07-26 23:22:17.000000 dgisim-0.2.dev3/dgisim.egg-info/top_level.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1475 2023-07-26 23:20:43.000000 dgisim-0.2.dev3/pyproject.toml
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2023-07-26 23:22:17.555174 dgisim-0.2.dev3/setup.cfg
```

### Comparing `dgisim-0.2.dev2/LICENSE` & `dgisim-0.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev2/PKG-INFO` & `dgisim-0.2.dev3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgisim
-Version: 0.2.dev2
+Version: 0.2.dev3
 Summary: A highly customizable Genius Invokation TCG Simulator for AI training
 Author: Jarvis Yu
 License: MIT License
         
         Copyright (c) 2023 Leyang Yu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,29 +65,35 @@
 ```
 pip install dgisim
 ```
 
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
 
-## [Documentation](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
+## [Wiki](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
 
-## Simple Guide
+- [v0.2.dev2 documentation](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev2-Documentation)
+- [state machine design](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/state_machine_design.md)
+- [run cloned repository locally](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/dev_readme.md)
+
+## Simple Start With CLI
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
 
 You might want to run a simple python program like this:
 
 ```py
 from dgisim import CLISession
 
 session = CLISession()
 session.run()
 ```
 
+Or try the CLI online on [Google Colab](https://colab.research.google.com/drive/1h6ckw4LQ2jMEnZAs9QQo6tHjCwWnR8KD?usp=sharing)
+
 See CLI's [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/cli_readme.md)
 for showcase and explanations of the CLI.
 
 ## Features of This Simulator
 
 First of all, it is modeled as a finite state machine, which means any intermediate state can be
 standalone and be used to proceed to other states.
@@ -100,59 +106,41 @@
 branches of possibilities in the future are not error-prone. Do not worry about memory efficiency,
 everything is immutable, so only the modified part between neighbouring game states are added to the
 memory.
 
 `GameState` implements `__eq__` and `__hash__`, enabling you to use any game state as a key in a
 dictionary, and discover game states on different 'game branches' being actually the same.
 
+## [State Machine Design](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/state_machine_design.md)
+
 ## Development Milestones
 
 - [x] Set up the framework for maintaining game states
 - [x] Implement game phase of Card Selection (card selection at the start of the game)
 - [x] Implement game phase of Starting Hand Select Phase (select active character)
 - [x] Implement game phase of Roll (Dice) Phase (roll dices between rounds)
 - [x] Implement game phase of Action Phase (players beat each other)
-  - [ ] Implement all cards (15/184 implemented)
-    - [x] Changing Shifts,
-          ColdBlooded Strike,
-          Jueyun Guoba,
-          Leave It to Me!,
-          Lightning Stiletto,
-          Lotus Flower Crisp,
-          Minty Meat Rolls,
-          Mondstadt Hash Brown,
-          Mushroom Pizza,
-          Nothern Smoked Chicken,
-          Starsigns,
-          Streaming Surge,
-          Sweet Madame,
-          Thundering Penance,
-          Xudong,
-  - [ ] Implement all characters with their talent cards (3/48 implemented)
-    - [x] Kaeya,
-          Keqing,
-          Rhodeia of Loch,
+  - [ ] Implement all cards (26/192 implemented) ([details](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/progress.md))
+  - [ ] Implement all characters with their talent cards (7/51 implemented) ([details](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/progress.md))
   - [x] Implement all reactions
+  - [x] Implement all logics to support the implemented cards and characters
 - [x] Implement game phase of End Phase (summons and some support card or statuses take action)
 - [x] Implement game phase of Game End Phase (one player wins or draw)
 - [x] Implement CLI for better debugging experience
 - [x] Implement interactive active CLI that accepts user input as action
 - [x] Implement lazy player agent for minimal testing purposes
 - [x] Implement random player agent for testing purposes
 - [x] Implement player action validity checker
 - [x] Implement player action choices provider
-- [ ] Implement greedy player agent for testing purposes
-
-> Just in case you don't know, **_WIP_** means "work in progress".
 
 ## Future Plans
 
 I have the plan to implement a simple cross-platform GUI interface for the simulator. But that will
 be in a separate repo.
 
 Once this project is done, I'll be reading relative papers and develop an AI for this game. The AI
 is supposed to be used for learning strategies and making decks, but not against another player
 directly.
 
-## Interested in the Project?
+## Wants To Contribute?
 
-Please read this [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/dev_readme.md).
+Please read [this](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/dev_readme.md).
```

### Comparing `dgisim-0.2.dev2/dgisim/src/__init__.py` & `dgisim-0.2.dev3/dgisim/src/__init__.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev2/dgisim/src/action/action.py` & `dgisim-0.2.dev3/dgisim/src/action/action.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "StaticTargetInstruction",
     "SourceTargetInstruction",
 ]
 
 @dataclass(frozen=True, repr=False)
 class PlayerAction:
     @classmethod
-    def _empty(cls) -> Self:
+    def _empty(cls) -> Self:  # pragma: no cover
         """
         This is just for action generator
         """
         return cls()
 
     @classmethod
     def _all_none(cls) -> Self:
@@ -50,65 +50,41 @@
         Sets all fields to None ready to be filled later
         """
         self = cls._empty()
         for field in fields(self):
             object.__setattr__(self, field.name, None)
         return self
 
-    def _set_attr(self, name: str, val: Any) -> Self:
-        """
-        This is just for action generator
-        """
-        other = replace(self)
-        object.__setattr__(other, name, val)
-        return other
-
     def _filled(self, exceptions: set[str] = set()) -> bool:
         """
         This is just for action generator
         """
         return all(
             self.__getattribute__(field.name) is not None
             for field in fields(self)
             if field.name not in exceptions
         )
 
-    def legal(self) -> bool:
-        field_type_val = (
-            (field.type, field.__getattribute__(field.name))
-            for field in fields(self)
-        )
-        return all(
-            isinstance(val, field_type)
-            for field_type, val in field_type_val
-        )
-
     def __repr__(self) -> str:
         return dataclass_repr(self)
 
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class CardsSelectAction(PlayerAction):
     selected_cards: Cards
 
-    def num_cards(self) -> int:
-        return self.selected_cards.num_cards()
-
     @classmethod
     def _empty(cls) -> Self:
         return cls(selected_cards=Cards({}))
 
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class DicesSelectAction(PlayerAction):
     selected_dices: ActualDices
 
-    def num_cards(self) -> int:
-        return self.selected_dices.num_dices()
-
     @classmethod
     def _empty(cls) -> Self:
         return cls(selected_dices=ActualDices({}))
 
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class CharacterSelectAction(PlayerAction):
@@ -122,16 +98,15 @@
 @dataclass(frozen=True, kw_only=True, repr=False)
 class EndRoundAction(PlayerAction):
     pass
 
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class GameAction(PlayerAction):
-    def is_valid_action(self, game_state: GameState) -> bool:
-        raise Exception("Not overriden")
+    ...
 
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class ElementalTuningAction(GameAction):
     card: type[Card]
     dice_elem: Element
 
@@ -195,33 +170,25 @@
         This is just for action generator
         """
         self = cls._empty()
         for field in fields(self):
             object.__setattr__(self, field.name, None)
         return self
 
-    def _set_attr(self, name: str, val: Any) -> Self:
-        """
-        This is just for action generator
-        """
-        other = replace(self)
-        object.__setattr__(other, name, val)
-        return other
-
     def _filled(self, exceptions: set[str] = set()) -> bool:
         """
         This is just for action generator
         """
         return all(
             self.__getattribute__(field.name) is not None
             for field in fields(self)
             if field.name not in exceptions
         )
 
-    def legal(self) -> bool:
+    def legal(self) -> bool:  # pragma: no cover
         field_type_val = (
             (field.type, field.__getattribute__(field.name))
             for field in fields(self)
         )
         return all(
             isinstance(val, field_type)
             for field_type, val in field_type_val
@@ -254,15 +221,15 @@
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class SourceTargetInstruction(Instruction):
     source: StaticTarget
     target: StaticTarget
 
     @classmethod
-    def _empty(cls) -> Self:
+    def _empty(cls) -> Self:  # pragma: no cover
         target = StaticTarget(
             pid=Pid.P1,
             zone=Zone.CHARACTERS,
             id=-1,
         )
         return cls(
             dices=ActualDices({}),
```

### Comparing `dgisim-0.2.dev2/dgisim/src/action/action_generator.py` & `dgisim-0.2.dev3/dgisim/src/action/action_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,30 +48,21 @@
         return self.action is None \
             or self.action._filled(exceptions={"instruction"})
 
     def _instruction_filled(self) -> bool:
         return self.instruction is None \
             or self.instruction._filled()
 
-    def _legal_action(self) -> bool:
-        return self.action is None or self.action.legal()
-
-    def _legal_instruction(self) -> bool:
-        return self.instruction is None or self.instruction.legal()
-
     def filled(self) -> bool:
         """
         Return if ActionGenerator is ready to produce the final action
         """
         return not (self.action is None and self.instruction is None) \
             and self._action_filled() and self._instruction_filled()
 
-    def valid(self) -> bool:
-        return self._legal_action() and self._legal_instruction()
-
     def generate_action(self) -> PlayerAction:
         assert self.filled()
         assert self.action is not None
         action = self.action
         if self.instruction is not None:
             action = replace(action, instruction=self.instruction)
         return action
```

### Comparing `dgisim-0.2.dev2/dgisim/src/action/action_generator_generator.py` & `dgisim-0.2.dev3/dgisim/src/action/action_generator_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     @classmethod
     def _choices_helper(cls, action_generator: ActionGenerator) -> GivenChoiceType:
         assert not action_generator.filled()
         game_state = action_generator.game_state
         pid = action_generator.pid
         return tuple(
             card_type
-            for card_type in game_state.get_player(pid).get_hand_cards()
+            for card_type in action_generator.hand_cards_available()
             if card_type.strictly_usable(game_state, pid)
         )
 
     @classmethod
     def _fill_helper(
         cls,
         action_generator: ActionGenerator,
@@ -69,15 +69,15 @@
 
     @classmethod
     def action_generator(
             cls,
             game_state: GameState,
             pid: Pid,
     ) -> None | ActionGenerator:
-        if not game_state.card_checker().playable(pid):
+        if not game_state.card_checker().playable(pid):  # pragma: no cover
             return None
         return ActionGenerator(
             game_state=game_state,
             pid=pid,
             _choices_helper=cls._choices_helper,
             _fill_helper=cls._fill_helper,
         )
@@ -89,15 +89,15 @@
     """
     @classmethod
     def _choices_helper(cls, action_generator: ActionGenerator) -> GivenChoiceType:
         assert not action_generator.filled()
         assert type(action_generator.action) is CardsSelectAction
         game_state = action_generator.game_state
         pid = action_generator.pid
-        hand_cards = game_state.get_player(pid).get_hand_cards()
+        hand_cards = action_generator.hand_cards_available()
         from ..card.card import OmniCard
         if hand_cards.contains(OmniCard):
             # TODO: further filter available cards
             publicly_used_cards = game_state.get_player(pid).get_publicly_used_cards()
             mode = game_state.get_mode()
             return tuple(
                 card
@@ -194,15 +194,15 @@
         game_state = action_generator.game_state
         pid = action_generator.pid
 
         action = action_generator.action
         assert type(action) is ElementalTuningAction
 
         if action.card is None:
-            return tuple(card for card in game_state.get_player(pid).get_hand_cards())
+            return tuple(card for card in action_generator.hand_cards_available())
 
         active_character = game_state.get_player(pid).just_get_active_character()
         if action.dice_elem is None:
             return tuple(
                 elem
                 for elem in game_state.get_player(pid).get_dices()
                 if elem is not Element.OMNI and elem is not active_character.element()
@@ -241,15 +241,15 @@
 
     @classmethod
     def action_generator(
             cls,
             game_state: GameState,
             pid: Pid,
     ) -> None | ActionGenerator:
-        if not game_state.elem_tuning_checker().usable(pid):
+        if not game_state.elem_tuning_checker().usable(pid):  # pragma: no cover
             return None
 
         return ActionGenerator(
             game_state=game_state,
             pid=pid,
             action=ElementalTuningAction._all_none(),
             instruction=None,
```

### Comparing `dgisim-0.2.dev2/dgisim/src/action/types.py` & `dgisim-0.2.dev3/dgisim/src/action/types.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev2/dgisim/src/agents.py` & `dgisim-0.2.dev3/dgisim/src/agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 This file contains different implementations of PlayerAgents.
 """
 import random
 from typing import Any, Callable, Iterable, Optional, TYPE_CHECKING, TypeVar
 
 from .action.action import *
+from .action.enums import ActionType
 from .action.action_generator import *
 from .action.action_generator_generator import *
 from .action.types import DecidedChoiceType
 from .card.card import *
 from .card.cards import Cards
 from .dices import AbstractDices, ActualDices
 from .effect.effect import *
+from .element import Element
 from .phase.default.action_phase import ActionPhase
 from .phase.default.card_select_phase import CardSelectPhase
 from .phase.default.end_phase import EndPhase
 from .phase.default.roll_phase import RollPhase
 from .phase.default.starting_hand_select_phase import StartingHandSelectPhase
 from .player_agent import PlayerAgent
 from .state.enums import Pid
@@ -46,15 +48,16 @@
 
     def choose_action(self, history: list[GameState], pid: Pid) -> PlayerAction:
         game_state = history[-1]
         curr_phase = game_state.get_phase()
 
         if isinstance(curr_phase, CardSelectPhase):
             _, selected_cards = game_state.get_player(
-                pid).get_hand_cards().pick_random_cards(self._NUM_PICKED_CARDS)
+                pid
+            ).get_hand_cards().pick_random_cards(self._NUM_PICKED_CARDS)
             return CardsSelectAction(selected_cards=selected_cards)
 
         elif isinstance(curr_phase, StartingHandSelectPhase):
             return CharacterSelectAction(char_id=1)
 
         elif isinstance(curr_phase, RollPhase):
             return EndRoundAction()
@@ -104,77 +107,86 @@
     """
     A player agent that make purely random (but of course valid) acions.
     """
     _NUM_PICKED_CARDS = 3
 
     def _card_select_phase(self, history: list[GameState], pid: Pid) -> PlayerAction:
         game_state = history[-1]
-        phase = game_state.get_phase()
-        act_gen = phase.action_generator(game_state, pid)
+        act_gen = game_state.action_generator(pid)
         assert act_gen is not None
         player_action = self._random_action_generator_chooser(act_gen)
         return player_action
 
     def _starting_hand_select_phase(
             self,
             history: list[GameState],
             pid: Pid
     ) -> PlayerAction:
         game_state = history[-1]
-        phase = game_state.get_phase()
-        act_gen = phase.action_generator(game_state, pid)
+        act_gen = game_state.action_generator(pid)
         assert act_gen is not None
         player_action = self._random_action_generator_chooser(act_gen)
         return player_action
 
     def _roll_phase(self, history: list[GameState], pid: Pid) -> PlayerAction:
         game_state = history[-1]
-        phase = game_state.get_phase()
-        act_gen = phase.action_generator(game_state, pid)
+        act_gen = game_state.action_generator(pid)
         assert act_gen is not None
         player_action = self._random_action_generator_chooser(act_gen)
         return player_action
 
     def _random_action_generator_chooser(self, action_generator: ActionGenerator) -> PlayerAction:
         while not action_generator.filled():
             choices = action_generator.choices()
             choice: DecidedChoiceType  # type: ignore
             if isinstance(choices, tuple):
+                game_state = action_generator.game_state
+                if game_state.get_phase() == game_state.get_mode().roll_phase() and random.random() < 0.8:
+                    choices = tuple(c for c in choices if c is not ActionType.END_ROUND)
                 choice = random.choice(choices)
                 action_generator = action_generator.choose(choice)
             elif isinstance(choices, AbstractDices):
                 optional_choice = action_generator.dices_available().basically_satisfy(choices)
                 if optional_choice is None:
                     raise Exception(f"There's not enough dices for {choices} from "
                                     + f"{action_generator.dices_available()} at game_state:"
                                     + f"{action_generator.game_state}")
                 choice = optional_choice
                 action_generator = action_generator.choose(choice)
             elif isinstance(choices, Cards):
                 _, choice = choices.pick_random_cards(random.randint(0, choices.num_cards()))
                 action_generator = action_generator.choose(choice)
             elif isinstance(choices, ActualDices):
-                _, choice = choices.pick_random_dices(random.randint(0, choices.num_dices()))
+                game_state = action_generator.game_state
+                wanted_elems = game_state.get_player(
+                    action_generator.pid
+                ).get_characters().all_elems()
+                if game_state.get_phase() == game_state.get_mode().roll_phase():
+                    choice = ActualDices(dict(
+                        (elem, choices[elem])
+                        for elem in choices.elems()
+                        if not(elem is Element.OMNI or elem in wanted_elems)
+                    ))
+                else:
+                    _, choice = choices.pick_random_dices(random.randint(0, choices.num_dices()))
                 action_generator = action_generator.choose(choice)
             else:
                 raise NotImplementedError
         return action_generator.generate_action()
 
     def _action_phase(self, history: list[GameState], pid: Pid) -> PlayerAction:
         game_state = history[-1]
-        phase = game_state.get_phase()
-        act_gen = phase.action_generator(game_state, pid)
+        act_gen = game_state.action_generator(pid)
         assert act_gen is not None
         player_action = self._random_action_generator_chooser(act_gen)
         return player_action
 
     def _end_phase(self, history: list[GameState], pid: Pid) -> PlayerAction:
         game_state = history[-1]
-        phase = game_state.get_phase()
-        act_gen = phase.action_generator(game_state, pid)
+        act_gen = game_state.action_generator(pid)
         assert act_gen is not None
         player_action = self._random_action_generator_chooser(act_gen)
         return player_action
 
     def choose_action(self, history: list[GameState], pid: Pid) -> PlayerAction:
         game_state = history[-1]
         curr_phase = game_state.get_phase()
```

### Comparing `dgisim-0.2.dev2/dgisim/src/card/card.py` & `dgisim-0.2.dev3/dgisim/src/card/card.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 
 - base class, which is Card
 - type classes, used to identify what type of card a card is
 - template classes, starting with an '_', are templates for other classes
 - concrete classes, the implementation of cards that are actually in the game
 """
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import cast, TYPE_CHECKING
 from dataclasses import replace
 from typing_extensions import override
 
 from ..action import action as act
 from ..action import action_generator as acg
 from ..character import character as chr
 from ..effect import effect as eft
 from ..status import status as stt
+from ..summon import summon as sm
 from ..support import support as sp
 
-from ..character.enums import CharacterSkill
+from ..character.enums import CharacterSkill, WeaponType
 from ..dices import AbstractDices, ActualDices
 from ..effect.enums import Zone
 from ..effect.structs import StaticTarget
 from ..element import Element
-from ..event import CardEvent
+from ..event import CardPEvent
 from ..helper.quality_of_life import BIG_INT
 from ..state.enums import Pid
 from ..status.enums import Preprocessables
 from ..status.status_processing import StatusProcessing
 
 if TYPE_CHECKING:
     from ..action.types import DecidedChoiceType, GivenChoiceType
@@ -43,47 +44,71 @@
 
     # special one
     "OmniCard",
 
     # type
     "EventCard",
     "EquipmentCard",
+    "TalentEquipmentCard",
+    "WeaponEquipmentCard",
+    "ArtifactEquipmentCard",
     "SupportCard",
     "CompanionCard",
     "LocationCard",
     "FoodCard",
 
+    # Weapon Card
+    ## Bow ##
+    "RavenBow",
+    ## Catalyst ##
+    "MagicGuide",
+    ## Claymore ##
+    "WhiteIronGreatsword",
+    ## Polearm ##
+    "WhiteTassel",
+    ## Sword ##
+    "TravelersHandySword",
+
     # Event Card
     ## Food Card ##
     "JueyunGuoba",
     "LotusFlowerCrisp",
     "MintyMeatRolls",
     "MondstadtHashBrown",
     "MushroomPizza",
     "NorthernSmokedChicken",
     "SweetMadame",
     ## Other ##
     "CalxsArts",
     "ChangingShifts",
     "LeaveItToMe",
+    "QuickKnit",
     "Starsigns",
 
     # Support Card
     ## Companion ##
     "Xudong",
     ## Location ##
 
     # Character Specific
+    ## Arataki Itto ##
+    "AratakiIchiban",
+    ## Kaedehara Kazuha ##
+    "PoeticsOfFuubutsu",
     ## Kaeya ##
     "ColdBloodedStrike",
     ## Keqing ##
     "LightningStiletto",
     "ThunderingPenance",
+    ## Klee ##
+    "PoundingSurprise",
     ## Rhodeia of Loch ##
     "StreamingSurge",
+    ## Tighnari ##
+    "KeenSight",
 ]
 
 ############################## base ##############################
 
 
 class Card:
     _DICE_COST = AbstractDices({Element.OMNI: BIG_INT})
@@ -94,15 +119,15 @@
             game_state: gs.GameState,
             pid: Pid,
             instruction: act.Instruction,
     ) -> tuple[eft.Effect, ...]:
         raise NotImplementedError
 
     @classmethod
-    def base_dice_cost(cls) -> AbstractDices:
+    def base_dice_cost(cls) -> AbstractDices:  # pragma: no cover
         return cls._DICE_COST
 
     @classmethod
     def preprocessed_dice_cost(
             cls,
             game_state: gs.GameState,
             pid: Pid
@@ -111,22 +136,22 @@
         Return a tuple of GameState and AbstractDices:
         - returned game-state is the game-state after preprocessing the usage of the card
         - returned abstract-dices are the actual cost of using the card at the provided game_state
         """
         game_state, card_event = StatusProcessing.preprocess_by_all_statuses(
             game_state=game_state,
             pid=pid,
-            item=CardEvent(
+            pp_type=Preprocessables.CARD,
+            item=CardPEvent(
                 pid=pid,
                 card_type=cls,
                 dices_cost=cls._DICE_COST,
             ),
-            pp_type=Preprocessables.CARD
         )
-        assert isinstance(card_event, CardEvent)
+        assert isinstance(card_event, CardPEvent)
         return game_state, card_event.dices_cost
 
     @classmethod
     def just_preprocessed_dice_cost(
             cls,
             game_state: gs.GameState,
             pid: Pid
@@ -177,15 +202,16 @@
             game_state: gs.GameState,
             pid: Pid,
             instruction: act.Instruction
     ) -> None | gs.GameState:
         """ Return the preprocessed game-state if instruction is valid, otherwise return None """
         if not game_state.get_player(pid).get_hand_cards().contains(cls) \
                 or not game_state.get_active_player_id() is pid \
-                or not cls._valid_instruction(game_state, pid, instruction):
+                or not cls._valid_instruction(game_state, pid, instruction) \
+                or not (game_state.get_player(pid).get_dices() - instruction.dices).is_legal():
             return None
         game_state, dices_cost = cls.preprocessed_dice_cost(game_state, pid)
         if instruction.dices.just_satisfy(dices_cost):
             return game_state
         else:
             return None
 
@@ -200,17 +226,17 @@
 
     @classmethod
     def action_generator(
             cls,
             game_state: gs.GameState,
             pid: Pid,
     ) -> None | acg.ActionGenerator:
-        return None
+        return None  # pragma: no cover
 
-    def __eq__(self, other: object) -> bool:
+    def __eq__(self, other: object) -> bool:  # pragma: no cover
         return type(self) == type(other)
 
     def __repr__(self) -> str:
         return self.__class__.__name__
 
     @staticmethod
     def is_combat_action() -> bool:
@@ -228,15 +254,15 @@
     def active_combat_talent_skill_card_usable(
             game_state: gs.GameState,
             pid: Pid,
             char: type[chr.Character]
     ):
         """ Check if active character is the character type and can cast skill """
         ac = game_state.get_player(pid).get_active_character()
-        if ac is None:
+        if ac is None:  # pragma: no cover
             return False
         if type(ac) is not char or not ac.can_cast_skill():
             return False
         return True
 
     @staticmethod
     def active_combat_talent_burst_card_usable(
@@ -245,32 +271,20 @@
             char: type[chr.Character]
     ):
         """
         Check if active character is the character type, can cast skill and have
         enough energy
         """
         active_character = game_state.get_player(pid).get_active_character()
-        if active_character is None:
+        if active_character is None:  # pragma: no cover
             return False
         return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, char) \
             and active_character.get_energy() == active_character.get_max_energy()
 
 
-class _ValidInstructionFuncs:
-    @staticmethod
-    def target_is_active_character(
-            game_state: gs.GameState,
-            pid: Pid,
-            instruction: act.StaticTargetInstruction,
-    ) -> bool:
-        return instruction.target.pid == pid \
-            and instruction.target.zone is Zone.CHARACTERS \
-            and instruction.target.id == game_state.get_player(pid).get_characters().get_active_character_id()
-
-
 class _DiceOnlyChoiceProvider(Card):
     @classmethod
     def _choices_helper(
             cls,
             action_generator: acg.ActionGenerator,
     ) -> GivenChoiceType:
         game_state = action_generator.game_state
@@ -279,18 +293,18 @@
         assert action_generator._action_filled()
 
         instruction = action_generator.instruction
         assert type(instruction) is act.DiceOnlyInstruction
         if instruction.dices is None:
             return cls.preprocessed_dice_cost(game_state, pid)[1]
 
-        raise Exception(
-            "Not Reached! Should be called when there is something to fill. action_generator:\n"
-            + f"{action_generator}"
-        )
+        raise Exception("Not Reached!"
+                        + "Should be called when there is something to fill. action_generator:\n"
+                        + f"{action_generator}"
+                        )
 
     @classmethod
     def _fill_helper(
         cls,
         action_generator: acg.ActionGenerator,
         player_choice: DecidedChoiceType,
     ) -> acg.ActionGenerator:
@@ -324,15 +338,15 @@
             _choices_helper=cls._choices_helper,
             _fill_helper=cls._fill_helper,
         )
 
 
 class _CharTargetChoiceProvider(Card):
     @classmethod
-    def _valid_char(cls, char: chr.Character) -> bool:
+    def _valid_char(cls, char: chr.Character) -> bool:  # pragma: no cover
         return not char.defeated()
 
     @classmethod
     def _choices_helper(
             cls,
             action_generator: acg.ActionGenerator,
     ) -> GivenChoiceType:
@@ -354,31 +368,32 @@
                 )
                 for char in chars
             )
 
         elif instruction.dices is None:
             return cls.preprocessed_dice_cost(game_state, pid)[1]
 
-        raise Exception(
-            "Not Reached! Should be called when there is something to fill. action_generator:\n"
-            + f"{action_generator}"
-        )
+        raise Exception("Not Reached!"
+                        + "Should be called when there is something to fill. action_generator:\n"
+                        + f"{action_generator}"
+                        )
 
     @classmethod
     def _fill_helper(
         cls,
         action_generator: acg.ActionGenerator,
         player_choice: DecidedChoiceType,
     ) -> acg.ActionGenerator:
         assert action_generator._action_filled()
 
         instruction = action_generator.instruction
         assert isinstance(instruction, act.StaticTargetInstruction)
         if instruction.target is None:
             assert isinstance(player_choice, StaticTarget)
+            assert player_choice.zone is Zone.CHARACTERS
             return replace(
                 action_generator,
                 instruction=replace(instruction, target=player_choice),
             )
 
         elif instruction.dices is None:
             assert isinstance(player_choice, ActualDices)
@@ -392,15 +407,111 @@
     @override
     @classmethod
     def action_generator(
             cls,
             game_state: gs.GameState,
             pid: Pid,
     ) -> None | acg.ActionGenerator:
-        if not cls.strictly_usable(game_state, pid):
+        if not cls.strictly_usable(game_state, pid):  # pragma: no cover
+            return None
+        return acg.ActionGenerator(
+            game_state=game_state,
+            pid=pid,
+            action=replace(act.CardAction._all_none(), card=cls),
+            instruction=act.StaticTargetInstruction._all_none(),
+            _choices_helper=cls._choices_helper,
+            _fill_helper=cls._fill_helper,
+        )
+
+
+class _SummonTargetChoiceProvider(Card):
+    """
+    If _MY_SIDE is set to true, then all summons on my side can be chosen
+    If _OPPO_SIDE is set to true, then all summons on the opponent's side can be chosen
+    """
+    _MY_SIDE: bool = False
+    _OPPO_SIDE: bool = False
+
+    @classmethod
+    def _valid_summon(cls, summon: sm.Summon) -> bool:  # pragma: no cover
+        return True
+
+    @classmethod
+    def _choices_helper(
+            cls,
+            action_generator: acg.ActionGenerator,
+    ) -> GivenChoiceType:
+        game_state = action_generator.game_state
+        pid = action_generator.pid
+
+        assert action_generator._action_filled()
+
+        instruction = action_generator.instruction
+        assert type(instruction) is act.StaticTargetInstruction
+        if instruction.target is None:
+            pids = []
+            if cls._MY_SIDE:
+                pids.append(pid)
+            if cls._OPPO_SIDE:
+                pids.append(pid.other())
+            choices = []
+            for this_pid in pids:
+                summons = game_state.get_player(this_pid).get_summons()
+                choices += [
+                    StaticTarget(
+                        pid=this_pid,
+                        zone=Zone.SUMMONS,
+                        id=type(summon),
+                    )
+                    for summon in summons
+                    if cls._valid_summon(summon)
+                ]
+            return tuple(choices)
+
+        elif instruction.dices is None:
+            return cls.preprocessed_dice_cost(game_state, pid)[1]
+
+        raise Exception("Not Reached!"
+                        + "Should be called when there is something to fill. action_generator:\n"
+                        + f"{action_generator}"
+                        )
+
+    @classmethod
+    def _fill_helper(
+        cls,
+        action_generator: acg.ActionGenerator,
+        player_choice: DecidedChoiceType,
+    ) -> acg.ActionGenerator:
+        instruction = action_generator.instruction
+        assert isinstance(instruction, act.StaticTargetInstruction)
+        if instruction.target is None:
+            assert isinstance(player_choice, StaticTarget)
+            assert player_choice.zone is Zone.SUMMONS
+            return replace(
+                action_generator,
+                instruction=replace(instruction, target=player_choice),
+            )
+
+        elif instruction.dices is None:
+            assert isinstance(player_choice, ActualDices)
+            return replace(
+                action_generator,
+                instruction=replace(instruction, dices=player_choice),
+            )
+
+        raise Exception("Not Reached!")
+
+    @override
+    @classmethod
+    def action_generator(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+    ) -> None | acg.ActionGenerator:
+        if not cls.strictly_usable(game_state, pid):  # pragma: no cover
             return None
         return acg.ActionGenerator(
             game_state=game_state,
             pid=pid,
             action=replace(act.CardAction._all_none(), card=cls),
             instruction=act.StaticTargetInstruction._all_none(),
             _choices_helper=cls._choices_helper,
@@ -427,17 +538,72 @@
     pass
 
 
 class EquipmentCard(Card):
     pass
 
 
-class SupportCard(Card):
-    # TODO: The effects are currently not handling support zone overflow
+class TalentEquipmentCard(EquipmentCard):
+    pass
+
+
+class WeaponEquipmentCard(EquipmentCard, _CharTargetChoiceProvider):
+    WEAPON_TYPE: WeaponType
+    WEAPON_STATUS: type[stt.WeaponEquipmentStatus]
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
+        chars = game_state.get_player(pid).get_characters().get_alive_characters()
+        return any(cls._valid_char(char) for char in chars) \
+            and super()._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def _valid_char(cls, char: chr.Character) -> bool:
+        return char.weapon_type() is cls.WEAPON_TYPE
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction
+    ) -> bool:
+        if not isinstance(instruction, act.StaticTargetInstruction) \
+                or pid is not instruction.target.pid:
+            return False  # pragma: no cover
+        char = game_state.get_target(instruction.target)
+        if not isinstance(char, chr.Character):  # pragma: no cover
+            return False
+        return cls._valid_char(char) and super()._valid_instruction(game_state, pid, instruction)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.StaticTargetInstruction)
+        return (
+            eft.AddCharacterStatusEffect(
+                target=instruction.target,
+                status=cls.WEAPON_STATUS,
+            ),
+        )
 
+
+class ArtifactEquipmentCard(EquipmentCard):
+    pass
+
+
+class SupportCard(Card):
     @override
     @classmethod
     def valid_instruction(
             cls,
             game_state: gs.GameState,
             pid: Pid,
             instruction: act.Instruction
@@ -462,25 +628,25 @@
             pid: Pid,
             instruction: act.Instruction,
     ) -> tuple[eft.Effect, ...]:
         es: list[eft.Effect] = []
         if type(instruction) is act.StaticTargetInstruction:
             es.append(eft.RemoveSupportEffect(
                 target_pid=pid,
-                sid=instruction.target.id,
+                sid=cast(int, instruction.target.id),
             ))
         return tuple(es) + cls._effects(game_state, pid)
 
     @classmethod
     def _effects(
             cls,
             game_state: gs.GameState,
             pid: Pid,
     ) -> tuple[eft.Effect, ...]:
-        raise
+        raise  # pragma: no cover
 
     @classmethod
     def _choices_helper(
             cls,
             action_generator: acg.ActionGenerator,
     ) -> GivenChoiceType:
         game_state = action_generator.game_state
@@ -502,18 +668,18 @@
 
         # only dices unfilled here
         assert type(instruction) is act.DiceOnlyInstruction \
             or type(instruction) is act.StaticTargetInstruction
         if instruction.dices is None:
             return cls.preprocessed_dice_cost(game_state, pid)[1]
 
-        raise Exception(
-            "Not Reached! Should be called when there is something to fill. action_generator:\n"
-            + f"{action_generator}"
-        )
+        raise Exception("Not Reached!"
+                        + "Should be called when there is something to fill. action_generator:\n"
+                        + f"{action_generator}"
+                        )
 
     @classmethod
     def _fill_helper(
         cls,
         action_generator: acg.ActionGenerator,
         player_choice: DecidedChoiceType,
     ) -> acg.ActionGenerator:
@@ -543,15 +709,15 @@
     @override
     @classmethod
     def action_generator(
             cls,
             game_state: gs.GameState,
             pid: Pid,
     ) -> None | acg.ActionGenerator:
-        if not cls.strictly_usable(game_state, pid):
+        if not cls.strictly_usable(game_state, pid):  # pragma: no cover
             return None
         if game_state.get_player(pid).get_supports().full():
             return acg.ActionGenerator(
                 game_state=game_state,
                 pid=pid,
                 action=replace(act.CardAction._all_none(), card=cls),
                 instruction=act.StaticTargetInstruction._all_none(),
@@ -591,17 +757,17 @@
     def _valid_instruction(
             cls,
             game_state: gs.GameState,
             pid: Pid,
             instruction: act.Instruction
     ) -> bool:
         """ This only applies to food with a single target, override if needed """
-        if not isinstance(instruction, act.StaticTargetInstruction):
-            return False
-
+        if not isinstance(instruction, act.StaticTargetInstruction) \
+                or pid is not instruction.target.pid:
+            return False  # pragma: no cover
         target = game_state.get_target(instruction.target)
         return isinstance(target, chr.Character) and not target.satiated()
 
     @classmethod
     def _valid_char(cls, char: chr.Character) -> bool:
         return not char.satiated() and not char.defeated()
 
@@ -618,22 +784,22 @@
             eft.AddCharacterStatusEffect(
                 instruction.target,
                 stt.SatiatedStatus,
             ),
         )
 
     @classmethod
-    def food_effects(cls, instruction: act.Instruction) -> tuple[eft.Effect, ...]:
+    def food_effects(cls, instruction: act.Instruction) -> tuple[eft.Effect, ...]:  # pragma: no cover
         assert isinstance(instruction, act.StaticTargetInstruction)
         return ()
 
 
 class _DirectHealCard(FoodCard):
     @classmethod
-    def heal_amount(cls) -> int:
+    def heal_amount(cls) -> int:  # pragma: no cover
         return 0
 
     @override
     @classmethod
     def food_effects(cls, instruction: act.Instruction) -> tuple[eft.Effect, ...]:
         assert isinstance(instruction, act.StaticTargetInstruction)
         return (
@@ -645,14 +811,55 @@
 
     @override
     @classmethod
     def _valid_char(cls, char: chr.Character) -> bool:
         return char.get_hp() < char.get_max_hp() \
             and super()._valid_char(char)
 
+# <<<<<<<<<<<<<<<<<<<< Equipment Cards <<<<<<<<<<<<<<<<<<<<
+########## Weapon Card ##########
+#### Bow ####
+
+
+class RavenBow(WeaponEquipmentCard):
+    _DICE_COST = AbstractDices({Element.OMNI: 2})
+    WEAPON_TYPE = WeaponType.BOW
+    WEAPON_STATUS = stt.RavenBowStatus
+
+#### Catalyst ####
+
+
+class MagicGuide(WeaponEquipmentCard):
+    _DICE_COST = AbstractDices({Element.OMNI: 2})
+    WEAPON_TYPE = WeaponType.CATALYST
+    WEAPON_STATUS = stt.MagicGuideStatus
+
+#### Claymore ####
+
+
+class WhiteIronGreatsword(WeaponEquipmentCard):
+    _DICE_COST = AbstractDices({Element.OMNI: 2})
+    WEAPON_TYPE = WeaponType.CLAYMORE
+    WEAPON_STATUS = stt.WhiteIronGreatswordStatus
+
+#### Polearm ####
+
+
+class WhiteTassel(WeaponEquipmentCard):
+    _DICE_COST = AbstractDices({Element.OMNI: 2})
+    WEAPON_TYPE = WeaponType.POLEARM
+    WEAPON_STATUS = stt.WhiteTasselStatus
+
+#### Sword ####
+
+
+class TravelersHandySword(WeaponEquipmentCard):
+    _DICE_COST = AbstractDices({Element.OMNI: 2})
+    WEAPON_TYPE = WeaponType.SWORD
+    WEAPON_STATUS = stt.TravelersHandySwordStatus
 
 # <<<<<<<<<<<<<<<<<<<< Event Cards <<<<<<<<<<<<<<<<<<<<
 # <<<<<<<<<<<<<<<<<<<< Event Cards / Food Cards <<<<<<<<<<<<<<<<<<<<
 
 
 class JueyunGuoba(FoodCard, _CharTargetChoiceProvider):
     _DICE_COST = AbstractDices({})
@@ -789,14 +996,44 @@
             game_state: gs.GameState,
             pid: Pid,
             instruction: act.Instruction
     ) -> bool:
         return isinstance(instruction, act.DiceOnlyInstruction) \
             and cls.loosely_usable(game_state, pid)
 
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        player = game_state.get_player(pid)
+        none_active_chars = player.get_characters().get_none_active_characters()
+        active_char_id = player.just_get_active_character().get_id()
+        effects: list[eft.Effect] = [
+            eft.EnergyDrainEffect(
+                target=StaticTarget(
+                    Pid.P1, Zone.CHARACTERS, char.get_id()
+                ),
+                drain=1,
+            )
+            for char in none_active_chars
+        ]
+        effects.append(
+            eft.EnergyRechargeEffect(
+                target=StaticTarget(
+                    Pid.P1, Zone.CHARACTERS, active_char_id
+                ),
+                recharge=sum(1 for char in none_active_chars if char.get_energy() > 0),
+            )
+        )
+        return tuple(effects)
+
 
 class ChangingShifts(EventCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({})
 
     @override
     @classmethod
     def _valid_instruction(
@@ -848,14 +1085,57 @@
             eft.AddCombatStatusEffect(
                 target_pid=pid,
                 status=stt.LeaveItToMeStatus,
             ),
         )
 
 
+class QuickKnit(EventCard, _SummonTargetChoiceProvider):
+    _DICE_COST = AbstractDices({Element.OMNI: 1})
+    _MY_SIDE = True
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
+        return not game_state.get_player(pid).get_summons().empty()
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction
+    ) -> bool:
+        if not isinstance(instruction, act.StaticTargetInstruction):  # pragma: no cover
+            return False
+
+        return (
+            instruction.target.pid is pid
+            and isinstance(game_state.get_target(instruction.target), sm.Summon)
+            and cls.loosely_usable(game_state, pid)
+        )
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.StaticTargetInstruction)
+        return (
+            eft.OneSummonIncreaseUsage(
+                target=instruction.target,
+                d_usages=1,
+            ),
+        )
+
+
 class Starsigns(EventCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({Element.ANY: 2})
 
     @override
     @classmethod
     def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
         """ Check active character doesn't have full energy """
@@ -869,15 +1149,15 @@
     def _valid_instruction(
             cls,
             game_state: gs.GameState,
             pid: Pid,
             instruction: act.Instruction
     ) -> bool:
         """ Check target is active character and .loosely_usable() """
-        if not isinstance(instruction, act.DiceOnlyInstruction):
+        if not isinstance(instruction, act.DiceOnlyInstruction):  # pragma: no cover
             return False
 
         return cls.loosely_usable(game_state, pid)
 
     @override
     @classmethod
     def effects(
@@ -919,18 +1199,126 @@
                 support=sp.XudongSupport,
             ),
         )
 
 # >>>>>>>>>>>>>>>>>>>> Support Cards / Companion Cards >>>>>>>>>>>>>>>>>>>>
 # >>>>>>>>>>>>>>>>>>>> Support Cards >>>>>>>>>>>>>>>>>>>>
 
+#### Arataki Itto ####
+
+
+class AratakiIchiban(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+    _DICE_COST = AbstractDices({Element.GEO: 1, Element.ANY: 2})
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
+        return (
+            _UsableFuncs.active_combat_talent_skill_card_usable(
+                game_state,
+                pid,
+                chr.AratakiItto
+            )
+            and super()._loosely_usable(game_state, pid)
+        )
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction
+    ) -> bool:
+        return isinstance(instruction, act.DiceOnlyInstruction) \
+            and cls._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.DiceOnlyInstruction)
+        target = StaticTarget(
+            pid=pid,
+            zone=Zone.CHARACTERS,
+            id=game_state.get_player(pid).just_get_active_character().get_id(),
+        )
+        return (
+            eft.AddCharacterStatusEffect(
+                target=target,
+                status=stt.AratakiIchibanStatus,
+            ),
+            eft.CastSkillEffect(
+                target=target,
+                skill=CharacterSkill.NORMAL_ATTACK,
+            ),
+        )
+
+#### Kaedehara Kazuha ####
+
+
+class PoeticsOfFuubutsu(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+    _DICE_COST = AbstractDices({Element.ANEMO: 3})
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
+        return (
+            _UsableFuncs.active_combat_talent_skill_card_usable(
+                game_state,
+                pid,
+                chr.KaedeharaKazuha
+            )
+            and super()._loosely_usable(game_state, pid)
+        )
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction
+    ) -> bool:
+        return isinstance(instruction, act.DiceOnlyInstruction) \
+            and cls._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.DiceOnlyInstruction)
+        target = StaticTarget(
+            pid=pid,
+            zone=Zone.CHARACTERS,
+            id=game_state.get_player(pid).just_get_active_character().get_id(),
+        )
+        return (
+            eft.AddCharacterStatusEffect(
+                target=target,
+                status=stt.PoeticsOfFuubutsuStatus,
+            ),
+            eft.CastSkillEffect(
+                target=target,
+                skill=CharacterSkill.ELEMENTAL_SKILL1,
+            ),
+        )
+
 #### Kaeya ####
 
 
-class ColdBloodedStrike(EquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+class ColdBloodedStrike(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({Element.CRYO: 4})
 
     @override
     @classmethod
     def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
         return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, chr.Kaeya) \
             and super()._loosely_usable(game_state, pid)
@@ -984,15 +1372,15 @@
             and super()._valid_char(char)
 
     @override
     @classmethod
     def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
         cs = game_state.get_player(pid).get_characters()
         keqings = [char for char in cs if type(char) is chr.Keqing]
-        if not keqings:
+        if not keqings:  # pragma: no cover
             return False
         if all(not keqing.can_cast_skill() for keqing in keqings):
             return False
         return super()._loosely_usable(game_state, pid)
 
     @override
     @classmethod
@@ -1027,15 +1415,15 @@
             eft.CastSkillEffect(
                 target=instruction.target,
                 skill=CharacterSkill.ELEMENTAL_SKILL1,
             ),
         )
 
 
-class ThunderingPenance(EquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+class ThunderingPenance(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({Element.ELECTRO: 3})
 
     @override
     @classmethod
     def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
         return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, chr.Keqing) \
             and super()._loosely_usable(game_state, pid)
@@ -1072,18 +1460,66 @@
             ),
             eft.CastSkillEffect(
                 target=target,
                 skill=CharacterSkill.ELEMENTAL_SKILL1,
             ),
         )
 
+#### Klee ####
+
+
+class PoundingSurprise(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+    _DICE_COST = AbstractDices({Element.PYRO: 3})
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
+        return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, chr.Klee) \
+            and super()._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction
+    ) -> bool:
+        return isinstance(instruction, act.DiceOnlyInstruction) \
+            and cls._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.DiceOnlyInstruction)
+        target = StaticTarget(
+            pid=pid,
+            zone=Zone.CHARACTERS,
+            id=game_state.get_player(pid).just_get_active_character().get_id(),
+        )
+        return (
+            eft.AddCharacterStatusEffect(
+                target=target,
+                status=stt.PoundingSurpriseStatus,
+            ),
+            eft.CastSkillEffect(
+                target=target,
+                skill=CharacterSkill.ELEMENTAL_SKILL1,
+            ),
+        )
 
 #### Rhodeia of Loch ####
 
-class StreamingSurge(EquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+
+class StreamingSurge(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({Element.HYDRO: 4})
 
     @override
     @classmethod
     def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
         return _UsableFuncs.active_combat_talent_burst_card_usable(game_state, pid, chr.RhodeiaOfLoch) \
             and super()._loosely_usable(game_state, pid)
@@ -1119,7 +1555,55 @@
                 status=stt.StreamingSurgeStatus,
             ),
             eft.CastSkillEffect(
                 target=target,
                 skill=CharacterSkill.ELEMENTAL_BURST,
             ),
         )
+
+#### Tighnari ####
+
+
+class KeenSight(TalentEquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+    _DICE_COST = AbstractDices({Element.DENDRO: 4})
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: Pid) -> bool:
+        return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, chr.Tighnari) \
+            and super()._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction
+    ) -> bool:
+        return isinstance(instruction, act.DiceOnlyInstruction) \
+            and cls._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: Pid,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.DiceOnlyInstruction)
+        target = StaticTarget(
+            pid=pid,
+            zone=Zone.CHARACTERS,
+            id=game_state.get_player(pid).just_get_active_character().get_id(),
+        )
+        return (
+            eft.AddCharacterStatusEffect(
+                target=target,
+                status=stt.KeenSightStatus,
+            ),
+            eft.CastSkillEffect(
+                target=target,
+                skill=CharacterSkill.ELEMENTAL_SKILL1,
+            ),
+        )
```

### Comparing `dgisim-0.2.dev2/dgisim/src/card/cards.py` & `dgisim-0.2.dev3/dgisim/src/card/cards.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         from .card import OmniCard
         if self[card] <= 0:
             assert self[OmniCard] > 0
             return self - {OmniCard: 1}  # type: ignore
         return self - {card: 1}
 
     def remove_all(self, card: type[Card]) -> Cards:
-        if self._cards[card] >= 1:
+        if self[card] >= 1:
             return self - {card: self._cards[card]}
         else:
             # if the card doesn't exist, even though there might be OmniCards
             # but we don't know how many to remove, so nothing is removed
             return self
 
     def hide_all(self) -> Cards:
@@ -95,15 +95,18 @@
 
     def __getitem__(self, card: type[Card]) -> int:
         return self._cards.get(card, 0)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Cards):
             return False
-        return self._cards == other._cards
+        return self is other or self._cards == other._cards
+
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return hash(self._cards)
 
     def __repr__(self) -> str:
         existing_cards = dict([
             (card.name(), str(num))
```

### Comparing `dgisim-0.2.dev2/dgisim/src/character/character.py` & `dgisim-0.2.dev3/dgisim/src/state/game_state.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,754 +1,591 @@
-"""
-This file contains the base class Character for all characters,
-and implementation of all characters. (in alphabetic order)
-"""
 from __future__ import annotations
-from typing import Callable, Optional, TYPE_CHECKING, Union
-from typing_extensions import override
-from functools import lru_cache
+from typing import Callable, cast, Optional
+from typing_extensions import Self
 
-from ..card import card as cd
+from .. import mode as md
+from ..action import action as act
+from ..action import action_generator as acg
 from ..effect import effect as eft
-from ..status import status as stt
-from ..status import statuses as stts
-from ..summon import summon as sm
+from ..phase import phase as ph
+from ..state import player_state as ps
 
+from ..action.action import PlayerAction
+from ..card.card import Card
+from ..character.character import Character
+from ..character.enums import CharacterSkill
 from ..dices import AbstractDices
-from ..effect.effects_template import *
-from ..effect.enums import Zone, DynamicCharacterTarget
-from ..effect.structs import StaticTarget, DamageType
-from ..element import *
-from ..state.enums import Pid
-from .enums import CharacterSkill
-
-if TYPE_CHECKING:
-    from ..state.game_state import GameState
+from ..effect.enums import Zone
+from ..effect.structs import StaticTarget
+from ..effect.effect_stack import EffectStack
+from ..effect.enums import Zone
+from ..effect.structs import StaticTarget
+from ..element import Element
+from ..event import *
+from ..helper.quality_of_life import case_val
+from ..status.status_processing import StatusProcessing
+from ..status.enums import Preprocessables
+from ..summon.summon import Summon
+from ..support.support import Support
+from .enums import Pid
 
 __all__ = [
-    # base
-    "Character",
-
-    # concretes
-    "Kaeya",
-    "Keqing",
-    "RhodeiaOfLoch",
+    "GameState",
 ]
 
-class Character:
-    _ELEMENT = Element.ANY
 
-    def __init__(
-        self,
-        id: int,
-        hp: int,
-        max_hp: int,
-        energy: int,
-        max_energy: int,
-        talents: stts.TalentStatuses,
-        equipments: stts.EquipmentStatuses,
-        statuses: stts.Statuses,
-        elemental_aura: ElementalAura,
-    ):
-        self._id = id
-        self._hp = hp
-        self._max_hp = max_hp
-        self._energy = energy
-        self._max_energy = max_energy
-        self._talents = talents
-        self._equipments = equipments
-        self._statuses = statuses
-        self._aura = elemental_aura
-
-    @staticmethod
-    def _talent_status() -> Optional[type[stt.EquipmentStatus]]:
-        return None
-
-    def get_id(self) -> int:
-        return self._id
-
-    def get_hp(self) -> int:
-        return self._hp
-
-    def get_max_hp(self) -> int:
-        return self._max_hp
-
-    def get_energy(self) -> int:
-        return self._energy
-
-    def get_max_energy(self) -> int:
-        return self._max_energy
-
-    def get_talent_statuses(self) -> stts.TalentStatuses:
-        return self._talents
-
-    def get_equipment_statuses(self) -> stts.EquipmentStatuses:
-        return self._equipments
-
-    def get_character_statuses(self) -> stts.Statuses:
-        return self._statuses
-
-    def get_elemental_aura(self) -> ElementalAura:
-        return self._aura
-
-    def get_all_statuses_ordered(self) -> list[stts.Statuses]:
-        return [self._talents, self._equipments, self._statuses]
-
-    def get_all_statuses_ordered_flattened(self) -> tuple[stt.Status, ...]:
-        return sum([statuses.get_statuses() for statuses in self.get_all_statuses_ordered()], ())
-
-    def factory(self) -> CharacterFactory:
-        return CharacterFactory(self, type(self))
-
-    def location(self, game_state: GameState) -> StaticTarget:
-        pid = game_state.belongs_to(self)
-        if pid is None:
-            raise Exception("target character is not in the current game state")
-        me = StaticTarget(pid, Zone.CHARACTERS, self.get_id())
-        return me
+class GameState:
+    """
+    The class which represents a moment or a state of the game, containing all
+    information required to proceed to the next game state.
 
-    @classmethod
-    def element(cls) -> Element:
-        return cls._ELEMENT
+    To proceed when the game doesn't require a player action at the moment,
+    run step(), otherwise run action_step(player_action).
 
-    @classmethod
-    def from_default(cls, id: int = -1) -> Character:
-        raise Exception("Not Overriden")
+    To tell if a player action is required, run waiting_for().
+    """
 
-    @classmethod
-    @lru_cache(maxsize=1)
-    def skills(cls) -> tuple[CharacterSkill, ...]:
-        """ Provides the skill types with corresponding cost that the character has """
-        my_skills: list[CharacterSkill] = []
-        if cls._normal_attack is not Character._normal_attack:
-            my_skills.append(CharacterSkill.NORMAL_ATTACK)
-        if cls._elemental_skill1 is not Character._elemental_skill1:
-            my_skills.append(CharacterSkill.ELEMENTAL_SKILL1)
-        if cls._elemental_skill2 is not Character._elemental_skill2:
-            my_skills.append(CharacterSkill.ELEMENTAL_SKILL2)
-        if cls._elemental_burst is not Character._elemental_burst:
-            my_skills.append(CharacterSkill.ELEMENTAL_BURST)
-        return tuple(my_skills)
+    def __init__(
+        self,
+        mode: md.Mode,
+        phase: ph.Phase,
+        round: int,
+        active_player_id: Pid,
+        player1: ps.PlayerState,
+        player2: ps.PlayerState,
+        effect_stack: EffectStack
+    ):
+        # REMINDER: don't forget to update factory when adding new fields
+        self._mode = mode
+        self._phase = phase
+        self._round = round
+        self._active_player_id = active_player_id
+        self._player1 = player1
+        self._player2 = player2
+        self._effect_stack = effect_stack
+
+        # checkers
+        self._card_checker = CardChecker(self)
+        self._swap_checker = SwapChecker(self)
+        self._skill_checker = SkillChecker(self)
+        self._elem_tuning_checker = ElementalTuningChecker(self)
 
     @classmethod
-    def skill_cost(cls, skill_type: CharacterSkill) -> AbstractDices:
-        raise NotImplementedError(f"{skill_type}'s cost is not defined for {cls.__name__}")
-
-    def skill(self, game_state: GameState, skill_type: CharacterSkill) -> tuple[eft.Effect, ...]:
-        return self._post_skill(
-            game_state,
-            skill_type,
-            self._skill(game_state, skill_type),
-        )
-
-    def _skill(self, game_state: GameState, skill_type: CharacterSkill) -> tuple[eft.Effect, ...]:
-        if skill_type is CharacterSkill.NORMAL_ATTACK:
-            return self.normal_attack(game_state)
-        elif skill_type is CharacterSkill.ELEMENTAL_SKILL1:
-            return self.elemental_skill1(game_state)
-        elif skill_type is CharacterSkill.ELEMENTAL_SKILL2:
-            return self.elemental_skill2(game_state)
-        elif skill_type is CharacterSkill.ELEMENTAL_BURST:
-            return self.elemental_burst(game_state)
-        raise Exception(f"Not Overriden, skill_type={skill_type}")
-
-    def _post_skill(
-            self,
-            game_state: GameState,
-            skill_type: CharacterSkill,
-            effects: tuple[eft.Effect, ...],
-    ) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return effects + (
-            eft.BroadCastSkillInfoEffect(
-                source=source,
-                skill=skill_type,
-            ),
-            eft.SwapCharacterCheckerEffect(
-                my_active=source,
-                oppo_active=StaticTarget(
-                    pid=source.pid.other(),
-                    zone=Zone.CHARACTERS,
-                    id=game_state.get_other_player(source.pid).just_get_active_character().get_id()
-                )
-            ),
-            eft.DeathCheckCheckerEffect(),
-        )
-
-    def normal_attack(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        return self._post_normal_attack(
-            game_state,
-            self._normal_attack(
-                self._pre_normal_attack(game_state)
-            )
-        )
-
-    def _pre_normal_attack(self, game_state: GameState) -> GameState:
-        return game_state
-
-    def _normal_attack(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        raise Exception("Not Overriden")
-
-    def _post_normal_attack(self, game_state: GameState, effects: tuple[eft.Effect, ...]) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return effects + (
-            eft.EnergyRechargeEffect(
-                target=source,
-                recharge=1,
-            ),
-        )
-
-    def elemental_skill1(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        return self._post_elemental_skill1(
-            game_state,
-            self._elemental_skill1(
-                self._pre_elemental_skill1(game_state)
-            )
-        )
-
-    def _pre_elemental_skill1(self, game_state: GameState) -> GameState:
-        return game_state
-
-    def _elemental_skill1(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        raise Exception("Not Overriden")
-
-    def _post_elemental_skill1(self, game_state: GameState, effects: tuple[eft.Effect, ...]) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return effects + (
-            eft.EnergyRechargeEffect(
-                target=source,
-                recharge=1,
-            ),
-        )
-
-    def elemental_skill2(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        return self._post_elemental_skill2(
-            game_state,
-            self._elemental_skill2(
-                self._pre_elemental_skill2(game_state)
-            )
+    def from_default(cls) -> Self:
+        mode = md.DefaultMode()
+        return cls(
+            mode=mode,
+            phase=mode.card_select_phase(),
+            round=0,
+            active_player_id=Pid.P1,
+            player1=ps.PlayerState.example_player(mode),
+            player2=ps.PlayerState.example_player(mode),
+            effect_stack=EffectStack(()),
         )
 
-    def _pre_elemental_skill2(self, game_state: GameState) -> GameState:
-        return game_state
-
-    def _elemental_skill2(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        raise Exception("Not Overriden")
-
-    def _post_elemental_skill2(self, game_state: GameState, effects: tuple[eft.Effect, ...]) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return effects + (
-            eft.EnergyRechargeEffect(
-                target=source,
-                recharge=1,
-            ),
-        )
+    @classmethod
+    def from_players(cls, mode: md.Mode, player1: ps.PlayerState, player2: ps.PlayerState) -> Self:
+        return cls(  # pragma: no cover
+            mode=mode,
+            phase=mode.card_select_phase(),
+            round=0,
+            active_player_id=Pid.P1,
+            player1=player1,
+            player2=player2,
+            effect_stack=EffectStack(()),
+        )
+
+    def factory(self) -> GameStateFactory:
+        return GameStateFactory(self)
+
+    def get_mode(self) -> md.Mode:
+        return self._mode
+
+    def get_phase(self) -> ph.Phase:
+        return self._phase
+
+    def get_round(self) -> int:
+        return self._round
+
+    def get_active_player_id(self) -> Pid:
+        return self._active_player_id
+
+    def get_effect_stack(self) -> EffectStack:
+        return self._effect_stack
+
+    def get_player1(self) -> ps.PlayerState:
+        return self._player1
+
+    def get_player2(self) -> ps.PlayerState:
+        return self._player2
+
+    def get_pid(self, player: ps.PlayerState) -> Pid:
+        if player is self._player1:
+            return Pid.P1
+        elif player is self._player2:
+            return Pid.P2
+        else:  # pragma: no cover
+            raise Exception("player unknown")
+
+    def get_player(self, player_id: Pid) -> ps.PlayerState:
+        if player_id.is_player1():
+            return self._player1
+        elif player_id.is_player2():
+            return self._player2
+        else:  # pragma: no cover
+            raise Exception("player_id unknown")
+
+    def get_other_player(self, player_id: Pid) -> ps.PlayerState:
+        if player_id.is_player1():
+            return self._player2
+        elif player_id.is_player2():
+            return self._player1
+        else:  # pragma: no cover
+            raise Exception("player_id unknown")
 
-    def elemental_burst(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        return self._post_elemental_burst(
-            game_state,
-            self._elemental_burst(
-                self._pre_elemental_burst(game_state)
+    def death_swapping(self, player_id: None | Pid = None) -> bool:
+        from ..effect.effect import DeathSwapPhaseStartEffect
+        return (
+            self._effect_stack.is_not_empty()
+            and isinstance(self._effect_stack.peek(), DeathSwapPhaseStartEffect)
+            and (
+                player_id is None
+                or self.get_player(player_id).get_phase().is_action_phase()
             )
         )
 
-    def _pre_elemental_burst(self, game_state: GameState) -> GameState:
-        return game_state
+    def card_checker(self) -> CardChecker:
+        return self._card_checker
 
-    def _elemental_burst(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        raise Exception("Not Overriden")
+    def swap_checker(self) -> SwapChecker:
+        return self._swap_checker
 
-    def _post_elemental_burst(self, game_state: GameState, effects: tuple[eft.Effect, ...]) -> tuple[eft.Effect, ...]:
-        return effects
+    def skill_checker(self) -> SkillChecker:
+        return self._skill_checker
 
-    def talent_equiped(self) -> bool:
-        talent_status = self._talent_status()
-        assert talent_status is not None
-        return self.get_equipment_statuses().contains(talent_status)
-
-    def alive(self) -> bool:
-        return not self.defeated()
-
-    def defeated(self) -> bool:
-        return self._hp == 0
+    def elem_tuning_checker(self) -> ElementalTuningChecker:
+        return self._elem_tuning_checker
+
+    def belongs_to(self, object: Character | Support) -> None | Pid:
+        """ int in object type is just place holder """
+        if self._player1.is_mine(object):
+            return Pid.P1
+        elif self._player2.is_mine(object):
+            return Pid.P2
+        else:  # pragma: no cover
+            return None
+
+    def get_target(self, target: StaticTarget) -> None | Character | Summon | Support:
+        player = self.get_player(target.pid)
+        if target.zone is Zone.CHARACTERS:
+            return player.get_characters().get_character(cast(int, target.id))
+        elif target.zone is Zone.SUMMONS:
+            return player.get_summons().find(cast(type[Summon], target.id))
+        elif target.zone is Zone.SUPPORTS:
+            return player.get_supports().find_by_sid(cast(int, target.id))
+        else:
+            raise Exception("Not Reached!")
 
-    def satiated(self) -> bool:
-        from ..status.status import SatiatedStatus
-        return self._statuses.contains(SatiatedStatus)
+    def get_character_target(self, target: StaticTarget) -> None | Character:
+        character = self.get_target(target)
+        if not isinstance(character, Character):  # pragma: no cover
+            return None
+        return character
+
+    def waiting_for(self) -> Optional[Pid]:
+        return self._phase.waiting_for(self)
+
+    def step(self) -> GameState:
+        return self._phase.step(self)
+
+    def action_step(self, pid: Pid, action: PlayerAction) -> Optional[GameState]:
+        """
+        Returns None if the action is illegal or undefined
+        """
+        return self._phase.step_action(self, pid, action)
+
+    def action_generator(self, pid: Pid) -> None | acg.ActionGenerator:
+        return self._phase.action_generator(self, pid)
+
+    def get_winner(self) -> Optional[Pid]:
+        assert self.game_end()
+        if self.get_player1().defeated():
+            return Pid.P2
+        elif self.get_player2().defeated():
+            return Pid.P1
+        else:
+            return None
 
-    def can_cast_skill(self) -> bool:
-        from ..status.status import FrozenStatus
-        return not self._statuses.contains(FrozenStatus) and not self.defeated()
+    def game_end(self) -> bool:
+        return type(self._phase) is type(self._mode.game_end_phase())
 
-    def name(self) -> str:
-        return self.__class__.__name__
+    def prespective_view(self, pid: Pid) -> GameState:
+        return self.factory().f_player(
+            pid.other(),
+            lambda p: p.hide_cards()
+        ).build()
 
     def _all_unique_data(self) -> tuple:
         return (
-            self._id,
-            self._hp,
-            self._max_hp,
-            self._energy,
-            self._max_energy,
+            self._phase,
+            self._round,
+            self._active_player_id,
+            self._player1,
+            self._player2,
+            self._effect_stack,
+            self._mode,
         )
 
     def __eq__(self, other: object) -> bool:
-        if not isinstance(other, type(self)):
+        if not isinstance(other, GameState):
             return False
-        return self._all_unique_data() == other._all_unique_data()
+        return self is other or self._all_unique_data() == other._all_unique_data()
 
     def __hash__(self) -> int:
         return hash(self._all_unique_data())
 
-    def dict_str(self) -> Union[dict, str]:
+    def __str__(self) -> str:
+        from ..helper.level_print import GamePrinter
+        return GamePrinter.dict_game_printer(self.dict_str())
+
+    def dict_str(self) -> dict:
         return {
-            "id": str(self._id),
-            "Aura": str(self._aura),
-            "HP": str(self._hp),
-            "Max HP": str(self._max_hp),
-            "Energy": str(self._energy),
-            "Max Energy": str(self._max_energy),
-            "Talents": self._talents.dict_str(),
-            "Equipments": self._equipments.dict_str(),
-            "Statuses": self._statuses.dict_str(),
+            "Mode": self._mode.dict_str(),
+            "Phase": self._phase.dict_str(),
+            "Round": str(self._round),
+            "Active Player": str(self._active_player_id),
+            "Player1": self._player1.dict_str(),
+            "Player2": self._player2.dict_str(),
+            "Effects": self._effect_stack.dict_str(),
         }
 
 
-class CharacterFactory:
-    def __init__(self, character: Character, char_type: type[Character]) -> None:
-        self._char = char_type
-        self._id = character.get_id()
-        self._hp = character.get_hp()
-        self._max_hp = character.get_max_hp()
-        self._energy = character.get_energy()
-        self._max_energy = character.get_max_energy()
-        self._talents = character.get_talent_statuses()
-        self._equipments = character.get_equipment_statuses()
-        self._statuses = character.get_character_statuses()
-        self._aura = character.get_elemental_aura()
-
-    def hp(self, hp: int) -> CharacterFactory:
-        self._hp = hp
-        return self
+class GameStateFactory:
+    def __init__(self, game_state: GameState):
+        self._mode = game_state.get_mode()
+        self._phase = game_state.get_phase()
+        self._round = game_state.get_round()
+        self._active_player = game_state.get_active_player_id()
+        self._player1 = game_state.get_player1()
+        self._player2 = game_state.get_player2()
+        self._effect_stack = game_state.get_effect_stack()
 
-    def energy(self, energy: int) -> CharacterFactory:
-        self._energy = energy
+    def mode(self, new_mode: md.Mode) -> GameStateFactory:
+        self._mode = new_mode
         return self
 
-    def talents(self, talents: stts.TalentStatuses) -> CharacterFactory:
-        self._talents = talents
+    def phase(self, new_phase: ph.Phase) -> GameStateFactory:
+        self._phase = new_phase
         return self
 
-    def f_talents(self, f: Callable[[stts.TalentStatuses], stts.TalentStatuses]) -> CharacterFactory:
-        return self.talents(f(self._talents))
+    def f_phase(self, f: Callable[[md.Mode], ph.Phase]) -> GameStateFactory:
+        return self.phase(f(self._mode))
 
-    def equipments(self, equipments: stts.EquipmentStatuses) -> CharacterFactory:
-        self._equipments = equipments
+    def round(self, new_round: int) -> GameStateFactory:
+        self._round = new_round
         return self
 
-    def f_equipments(self, f: Callable[[stts.EquipmentStatuses], stts.EquipmentStatuses]) -> CharacterFactory:
-        return self.equipments(f(self._equipments))
-
-    def character_statuses(self, statuses: stts.Statuses) -> CharacterFactory:
-        self._statuses = statuses
+    def effect_stack(self, effect_stack: EffectStack) -> GameStateFactory:
+        self._effect_stack = effect_stack
         return self
 
-    def f_character_statuses(self, f: Callable[[stts.Statuses], stts.Statuses]) -> CharacterFactory:
-        return self.character_statuses(f(self._statuses))
+    def f_effect_stack(self, f: Callable[[EffectStack], EffectStack]) -> GameStateFactory:
+        return self.effect_stack(f(self._effect_stack))
 
-    def elemental_aura(self, aura: ElementalAura) -> CharacterFactory:
-        self._aura = aura
+    def active_player_id(self, pid: Pid) -> GameStateFactory:
+        self._active_player = pid
         return self
 
-    def build(self) -> Character:
-        return self._char(
-            id=self._id,
-            hp=self._hp,
-            max_hp=self._max_hp,
-            energy=self._energy,
-            max_energy=self._max_energy,
-            talents=self._talents,
-            equipments=self._equipments,
-            statuses=self._statuses,
-            elemental_aura=self._aura,
-        )
-
-
-class Keqing(Character):
-    # basic info
-    _ELEMENT = Element.ELECTRO
-
-    # consts
-    BASE_ELECTRO_INFUSION_DURATION: int = 2
-
-    @override
-    @staticmethod
-    def _talent_status() -> Optional[type[stt.EquipmentStatus]]:
-        return stt.ThunderingPenanceStatus
-
-    @override
-    @classmethod
-    def skill_cost(cls, skill_type: CharacterSkill) -> AbstractDices:
-        if skill_type is CharacterSkill.NORMAL_ATTACK:
-            return AbstractDices({
-                Element.ELECTRO: 1,
-                Element.ANY: 2,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_SKILL1:
-            return AbstractDices({
-                Element.ELECTRO: 3,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_BURST:
-            return AbstractDices({
-                Element.ELECTRO: 4,
-            })
-        return super().skill_cost(skill_type)
-
-    def _normal_attack(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return normal_attack_template(
-            source=source,
-            element=Element.PHYSICAL,
-            damage=2,
-            dices_num=game_state.get_player(source.pid).get_dices().num_dices()
-        )
-
-    def _elemental_skill1(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        effects: list[eft.Effect] = [
-            eft.ReferredDamageEffect(
-                source=source,
-                target=DynamicCharacterTarget.OPPO_ACTIVE,
-                element=Element.ELECTRO,
-                damage=3,
-                damage_type=DamageType(elemental_skill=True)
-            )
-        ]
-
-        # check if can gain ElectroInfusionStatus
-        can_infuse = False
-
-        intrinsic_talent = self.get_talent_statuses().just_find(stt.KeqingTalentStatus)
-        if intrinsic_talent.can_infuse:
-            can_infuse = True
-            effects.append(
-                eft.OverrideCharacterStatusEffect(
-                    source,
-                    stt.KeqingTalentStatus(can_infuse=False),
-                )
-            )
-
-        cards = game_state.get_player(source.pid).get_hand_cards()
-        if not can_infuse and cards.contains(cd.LightningStiletto):
-            effects.append(
-                eft.PublicRemoveAllCardEffect(
-                    source.pid,
-                    cd.LightningStiletto,
-                )
-            )
-            can_infuse = True
-
-        if can_infuse:
-            if self.talent_equiped():
-                effects.append(
-                    eft.OverrideCharacterStatusEffect(
-                        target=source,
-                        status=stt.KeqingElectroInfusionStatus(
-                            usages=self.BASE_ELECTRO_INFUSION_DURATION + 1,
-                            damage_boost=1,
-                        ),
-                    )
-                )
-            else:
-                effects.append(
-                    eft.OverrideCharacterStatusEffect(
-                        target=source,
-                        status=stt.KeqingElectroInfusionStatus(
-                            usages=self.BASE_ELECTRO_INFUSION_DURATION
-                        ),
-                    )
-                )
-        else:
-            effects.append(
-                eft.PublicAddCardEffect(
-                    pid=source.pid,
-                    card=cd.LightningStiletto,
-                )
-            )
-
-        return tuple(effects)
+    def player1(self, new_player: ps.PlayerState) -> GameStateFactory:
+        self._player1 = new_player
+        return self
 
-    def _elemental_burst(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        assert self.get_energy() == self.get_max_energy()
-        source = self.location(game_state)
-        return (
-            eft.EnergyDrainEffect(
-                target=source,
-                drain=self.get_max_energy(),
-            ),
-            eft.ReferredDamageEffect(
-                source=source,
-                target=DynamicCharacterTarget.OPPO_OFF_FIELD,
-                element=Element.PIERCING,
-                damage=3,
-                damage_type=DamageType(elemental_burst=True),
-            ),
-            eft.ReferredDamageEffect(
-                source=source,
-                target=DynamicCharacterTarget.OPPO_ACTIVE,
-                element=Element.ELECTRO,
-                damage=4,
-                damage_type=DamageType(elemental_burst=True),
-            ),
-        )
+    def f_player1(self, f: Callable[[ps.PlayerState], ps.PlayerState]) -> GameStateFactory:
+        return self.player1(f(self._player1))
 
-    @classmethod
-    def from_default(cls, id: int = -1) -> Keqing:
-        return cls(
-            id=id,
-            hp=10,
-            max_hp=10,
-            energy=0,
-            max_energy=3,
-            statuses=stts.OrderedStatuses(()),
-            talents=stts.TalentStatuses((stt.KeqingTalentStatus(can_infuse=False),)),
-            equipments=stts.EquipmentStatuses(()),
-            elemental_aura=ElementalAura.from_default(),
-        )
+    def player2(self, new_player: ps.PlayerState) -> GameStateFactory:
+        self._player2 = new_player
+        return self
 
+    def f_player2(self, f: Callable[[ps.PlayerState], ps.PlayerState]) -> GameStateFactory:
+        return self.player2(f(self._player2))
 
-class Kaeya(Character):
-    # basic info
-    _ELEMENT = Element.CRYO
-
-    @override
-    @staticmethod
-    def _talent_status() -> Optional[type[stt.EquipmentStatus]]:
-        return stt.ColdBloodedStrikeStatus
+    def player(self, pid: Pid, new_player: ps.PlayerState) -> GameStateFactory:
+        if pid is Pid.P1:
+            return self.player1(new_player)
+        elif pid is Pid.P2:
+            return self.player2(new_player)
+        else:  # pragma: no cover
+            raise Exception("player_id unknown")
+
+    def f_player(self, pid: Pid, f: Callable[[ps.PlayerState], ps.PlayerState]) -> GameStateFactory:
+        if pid is Pid.P1:
+            return self.player1(f(self._player1))
+        elif pid is Pid.P2:
+            return self.player2(f(self._player2))
+        else:  # pragma: no cover
+            raise Exception("player_id unknown")
+
+    def other_player(self, pid: Pid, new_player: ps.PlayerState) -> GameStateFactory:
+        if pid is Pid.P1:
+            return self.player2(new_player)
+        elif pid is Pid.P2:
+            return self.player1(new_player)
+        else:  # pragma: no cover
+            raise Exception("player_id unknown")
+
+    def f_other_player(self, pid: Pid, f: Callable[[ps.PlayerState], ps.PlayerState]) -> GameStateFactory:
+        if pid is Pid.P1:
+            return self.player2(f(self._player2))
+        elif pid is Pid.P2:
+            return self.player1(f(self._player1))
+        else:  # pragma: no cover
+            raise Exception("player_id unknown")
+
+    def build(self) -> GameState:
+        return GameState(
+            mode=self._mode,
+            phase=self._phase,
+            round=self._round,
+            active_player_id=self._active_player,
+            effect_stack=self._effect_stack,
+            player1=self._player1,
+            player2=self._player2,
+        )
+
+
+class CardChecker:
+    def __init__(self, game_state: GameState) -> None:
+        self._game_state = game_state
+
+    def usable(self, pid: Pid, card_type: type[Card]) -> None | acg.ActionGenerator:
+        return card_type.action_generator(self._game_state, pid)
+
+    def playable(self, pid: Pid) -> bool:
+        """ Returns true if any card is playable """
+        return any(
+            card_type.strictly_usable(self._game_state, pid)
+            for card_type in self._game_state.get_player(pid).get_hand_cards()
+        )
+
+
+class SwapChecker:
+    def __init__(self, game_state: GameState) -> None:
+        self._game_state = game_state
+
+    def should_death_swap(self) -> bool:
+        effect_stack = self._game_state.get_effect_stack()
+        return effect_stack.is_not_empty() \
+            and isinstance(effect_stack.peek(), eft.DeathSwapPhaseStartEffect)
 
-    @override
-    @classmethod
-    def skill_cost(cls, skill_type: CharacterSkill) -> AbstractDices:
-        if skill_type is CharacterSkill.NORMAL_ATTACK:
-            return AbstractDices({
-                Element.CRYO: 1,
-                Element.ANY: 2,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_SKILL1:
-            return AbstractDices({
-                Element.CRYO: 3,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_BURST:
-            return AbstractDices({
-                Element.CRYO: 4,
-            })
-        return super().skill_cost(skill_type)
-
-    def _normal_attack(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return normal_attack_template(
-            source=source,
-            element=Element.PHYSICAL,
-            damage=2,
-            dices_num=game_state.get_player(source.pid).get_dices().num_dices()
+    def swappable(
+            self,
+            pid: Pid,
+    ) -> bool:
+        """ Returns true if a swap to any character is available """
+        return any(
+            self.swap_details(pid, char.get_id()) is not None
+            for char in self._game_state.get_player(pid).get_characters()
         )
 
-    def _elemental_skill1(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return (
-            eft.ReferredDamageEffect(
-                source=source,
-                target=DynamicCharacterTarget.OPPO_ACTIVE,
-                element=Element.CRYO,
-                damage=3,
-                damage_type=DamageType(elemental_skill=True),
+    def swap_details(
+            self,
+            pid: Pid,
+            char_id: int,
+    ) -> None | tuple[EventSpeed, None | AbstractDices]:
+        game_state = self._game_state
+        selected_char = game_state.get_player(pid).get_characters().get_character(char_id)
+        active_character_id = game_state.get_player(pid).get_characters().get_active_character_id()
+        if selected_char is None \
+                or selected_char.defeated() \
+                or selected_char.get_id() == active_character_id:
+            return None
+
+        if self.should_death_swap():
+            return EventSpeed.FAST_ACTION, None
+
+        # Check if player can afford Normal Swap
+        _, swap_action = StatusProcessing.preprocess_by_all_statuses(
+            game_state=game_state,
+            pid=pid,
+            pp_type=Preprocessables.SWAP,
+            item=ActionPEvent(
+                source=StaticTarget(
+                    pid=pid,
+                    zone=Zone.CHARACTERS,
+                    id=char_id,
+                ),
+                event_type=EventType.SWAP,
+                event_speed=game_state.get_mode().swap_speed(),
+                dices_cost=game_state.get_mode().swap_cost(),
             ),
         )
+        assert isinstance(swap_action, ActionPEvent)
+        if game_state.get_player(pid).get_dices().loosely_satisfy(swap_action.dices_cost):
+            return swap_action.event_speed, swap_action.dices_cost
+        else:
+            return None
 
-    def _elemental_burst(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return (
-            eft.EnergyDrainEffect(
-                target=source,
-                drain=self.get_max_energy(),
-            ),
-            eft.ReferredDamageEffect(
-                source=source,
-                target=DynamicCharacterTarget.OPPO_ACTIVE,
-                element=Element.CRYO,
-                damage=1,
-                damage_type=DamageType(elemental_burst=True),
-            ),
-            eft.OverrideCombatStatusEffect(
-                target_pid=source.pid,
-                status=stt.IcicleStatus(),
+    def valid_action(
+            self,
+            pid: Pid,
+            action: act.SwapAction | act.DeathSwapAction,
+    ) -> None | tuple[GameState, EventSpeed]:
+        """
+        Return None if the action is invalid,
+        otherwise return the GameState after preprocessing the swap event.
+        """
+        game_state = self._game_state
+        selected_char = game_state.get_player(
+            pid
+        ).get_characters().get_character(action.char_id)
+        active_character_id = game_state.get_player(pid).get_characters().get_active_character_id()
+        if selected_char is None \
+                or selected_char.defeated() \
+                or selected_char.get_id() == active_character_id:
+            return None
+        if isinstance(action, act.DeathSwapAction):
+            swap_details = self.swap_details(
+                pid=pid,
+                char_id=action.char_id,
             )
-        )
-
-    @classmethod
-    def from_default(cls, id: int = -1) -> Kaeya:
-        return cls(
-            id=id,
-            hp=10,
-            max_hp=10,
-            energy=0,
-            max_energy=2,
-            talents=stts.TalentStatuses(()),
-            equipments=stts.EquipmentStatuses(()),
-            statuses=stts.OrderedStatuses(()),
-            elemental_aura=ElementalAura.from_default(),
-        )
+            return case_val(
+                swap_details is not None,
+                (game_state, EventSpeed.FAST_ACTION),
+                None,
+            )
+        elif isinstance(action, act.SwapAction):
+            new_game_state, swap_action = StatusProcessing.preprocess_by_all_statuses(
+                game_state=game_state,
+                pid=pid,
+                pp_type=Preprocessables.SWAP,
+                item=ActionPEvent(
+                    source=StaticTarget(
+                        pid=pid,
+                        zone=Zone.CHARACTERS,
+                        id=action.char_id,
+                    ),
+                    event_type=EventType.SWAP,
+                    event_speed=game_state.get_mode().swap_speed(),
+                    dices_cost=game_state.get_mode().swap_cost(),
+                ),
+            )
+            assert isinstance(swap_action, ActionPEvent)
+            instruction_dices = action.instruction.dices
+            player_dices = game_state.get_player(pid).get_dices()
+            return case_val(
+                (player_dices - instruction_dices).is_legal()
+                and instruction_dices.just_satisfy(swap_action.dices_cost),
+                (new_game_state, swap_action.event_speed),
+                None
+            )
+        raise Exception("action ({action}) is not expected to be passed in")  # pragma: no cover
 
 
-class RhodeiaOfLoch(Character):
-    # basic info
-    _ELEMENT = Element.HYDRO
-
-    # consts
-    _SUMMONS = (
-        sm.OceanicMimicSquirrelSummon,
-        sm.OceanicMimicRaptorSummon,
-        sm.OceanicMimicFrogSummon,
-    )
-
-    @override
-    @staticmethod
-    def _talent_status() -> Optional[type[stt.EquipmentStatus]]:
-        return stt.StreamingSurgeStatus
+class SkillChecker:
+    def __init__(self, game_state: GameState) -> None:
+        self._game_state = game_state
 
-    @override
-    @classmethod
-    def skill_cost(cls, skill_type: CharacterSkill) -> AbstractDices:
-        if skill_type is CharacterSkill.NORMAL_ATTACK:
-            return AbstractDices({
-                Element.HYDRO: 1,
-                Element.ANY: 2,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_SKILL1:
-            return AbstractDices({
-                Element.HYDRO: 3,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_SKILL2:
-            return AbstractDices({
-                Element.HYDRO: 5,
-            })
-        elif skill_type is CharacterSkill.ELEMENTAL_BURST:
-            return AbstractDices({
-                Element.HYDRO: 3,
-            })
-        return super().skill_cost(skill_type)
-
-    def _normal_attack(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        return normal_attack_template(
-            source=source,
-            element=Element.HYDRO,
-            damage=1,
-            dices_num=game_state.get_player(source.pid).get_dices().num_dices()
+    def usable(
+            self,
+            pid: Pid,
+            char_id: int,
+            skill_type: CharacterSkill,
+    ) -> None | tuple[GameState, AbstractDices]:
+        game_state = self._game_state
+        character = game_state.get_player(pid).get_characters().get_character(char_id)
+        if character is None \
+                or not character.can_cast_skill() \
+                or skill_type not in character.skills():
+            return None
+        if skill_type is CharacterSkill.ELEMENTAL_BURST \
+                and character.get_energy() < character.get_max_energy():
+            return None
+        new_game_state, skill_event = StatusProcessing.preprocess_by_all_statuses(
+            game_state=game_state,
+            pid=pid,
+            pp_type=Preprocessables.SKILL,
+            item=ActionPEvent(
+                source=StaticTarget(
+                    pid=pid,
+                    zone=Zone.CHARACTERS,
+                    id=char_id,
+                ),
+                event_type=skill_type.to_event_type(),
+                event_speed=EventSpeed.COMBAT_ACTION,
+                dices_cost=character.skill_cost(skill_type),
+            ),
         )
+        assert isinstance(skill_event, ActionPEvent)
+        if game_state.get_player(pid).get_dices().loosely_satisfy(skill_event.dices_cost):
+            return new_game_state, skill_event.dices_cost
+        else:
+            return None
 
-    def _not_summoned_types(
+    def skillable(
             self,
-            game_state: GameState,
             pid: Pid
-    ) -> tuple[type[sm.Summon], ...]:
-        summons = game_state.get_player(pid).get_summons()
-        return tuple(
-            summon
-            for summon in self._SUMMONS
-            if summon not in summons
-        )
-
-    def _elemental_skill1(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        from random import choice
-        source = self.location(game_state)
-
-        summons_to_choose = self._not_summoned_types(game_state, source.pid)
-        summon: type[sm.Summon]
-        if summons_to_choose:
-            summon = choice(summons_to_choose)
-        else:  # if all kinds of summons have been summoned
-            summon = choice(self._SUMMONS)
-        return (
-            eft.AddSummonEffect(
-                target_pid=source.pid,
-                summon=summon,
-            ),
+    ) -> bool:
+        active_character_id = self._game_state.get_player(pid).just_get_active_character().get_id()
+        return any(
+            self.usable(pid, active_character_id, skill_type)
+            for skill_type in CharacterSkill
         )
 
-    def _elemental_skill2(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        from random import choice
-        source = self.location(game_state)
-
-        # first choice
-        summons_to_choose = self._not_summoned_types(game_state, source.pid)
-        fst_summon: type[sm.Summon]
-
-        if summons_to_choose:
-            fst_summon = choice(summons_to_choose)
-        else:  # if all kinds of summons have been summoned
-            fst_summon = choice(self._SUMMONS)
-
-        # second choice
-        summons_to_choose = tuple(
-            summon
-            for summon in summons_to_choose
-            if summon is not fst_summon
-        )
-        snd_summon: type[sm.Summon]
-
-        if summons_to_choose:
-            snd_summon = choice(summons_to_choose)
-        else:  # if all kinds of summons have been summoned, choose a random that is not chosen
-            snd_summon = choice([
-                summon
-                for summon in self._SUMMONS
-                if summon is not fst_summon
-            ])
-
-        assert fst_summon is not snd_summon
-        return (
-            eft.AddSummonEffect(
-                target_pid=source.pid,
-                summon=fst_summon,
-            ),
-            eft.AddSummonEffect(
-                target_pid=source.pid,
-                summon=snd_summon,
+    def valid_action(
+            self,
+            pid: Pid,
+            action: act.SkillAction,
+    ) -> None | GameState:
+        game_state = self._game_state
+        skill_type = action.skill
+        character = game_state.get_player(pid).get_active_character()
+        if character is None \
+                or not character.can_cast_skill() \
+                or skill_type not in character.skills():  # pragma: no cover
+            return None
+        if skill_type is CharacterSkill.ELEMENTAL_BURST \
+                and character.get_energy() < character.get_max_energy():  # pragma: no cover
+            return None
+        game_state, skill_event = StatusProcessing.preprocess_by_all_statuses(
+            game_state=game_state,
+            pid=pid,
+            pp_type=Preprocessables.SKILL,
+            item=ActionPEvent(
+                source=StaticTarget(
+                    pid=pid,
+                    zone=Zone.CHARACTERS,
+                    id=character.get_id(),
+                ),
+                event_type=skill_type.to_event_type(),
+                event_speed=EventSpeed.COMBAT_ACTION,
+                dices_cost=character.skill_cost(skill_type),
             ),
         )
+        assert isinstance(skill_event, ActionPEvent)
+        paid_dices = action.instruction.dices
+        if paid_dices.just_satisfy(skill_event.dices_cost) \
+                and (game_state.get_player(pid).get_dices() - paid_dices).is_legal():
+            return game_state
+        else:
+            return None
 
-    def _elemental_burst(self, game_state: GameState) -> tuple[eft.Effect, ...]:
-        source = self.location(game_state)
-        summons = game_state.get_player(source.pid).get_summons()
-        effects: list[eft.Effect] = [
-            eft.EnergyDrainEffect(
-                target=source,
-                drain=self.get_max_energy(),
-            ),
-            eft.ReferredDamageEffect(
-                source=source,
-                target=DynamicCharacterTarget.OPPO_ACTIVE,
-                element=Element.HYDRO,
-                damage=2 + 2 * len(summons),
-                damage_type=DamageType(elemental_burst=True)
-            ),
-        ]
-
-        if self.talent_equiped():
-            effects.append(eft.AllSummonIncreaseUsage(target_pid=source.pid, d_usages=1))
 
-        return tuple(effects)
+class ElementalTuningChecker:
+    def __init__(self, game_state: GameState) -> None:
+        self._game_state = game_state
 
-    @classmethod
-    def from_default(cls, id: int = -1) -> RhodeiaOfLoch:
-        return cls(
-            id=id,
-            hp=10,
-            max_hp=10,
-            energy=0,
-            max_energy=3,
-            talents=stts.TalentStatuses(()),
-            equipments=stts.EquipmentStatuses(()),
-            statuses=stts.OrderedStatuses(()),
-            elemental_aura=ElementalAura.from_default(),
+    def usable(self, pid: Pid, elem: None | Element = None) -> bool:
+        game_state = self._game_state
+        if not (type(game_state.get_phase()) == type(game_state.get_mode().action_phase())
+                or game_state.get_active_player_id() is pid):  # pragma: no cover
+            return False
+        player = game_state.get_player(pid)
+        active_character = player.get_active_character()
+        assert active_character is not None
+        active_character_elem = active_character.element()
+        dices = player.get_dices()
+        return (
+            player.get_hand_cards().not_empty()
+            and dices[Element.OMNI] + dices[active_character_elem] < dices.num_dices()
+            and (elem is None or dices[elem] > 0)
         )
```

### Comparing `dgisim-0.2.dev2/dgisim/src/character/characters.py` & `dgisim-0.2.dev3/dgisim/src/character/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 from typing import Callable, Iterator, Optional, TYPE_CHECKING, Union, Iterable
 
 if TYPE_CHECKING:
     from .character import Character
+    from ..element import Element
 
 __all__ = [
     "Characters",
 ]
 
+
 class Characters:
     def __init__(self, characters: tuple[Character, ...], active_character_id: None | int):
         self._characters = characters
         self._active_character_id = active_character_id
 
     @classmethod
     def from_default(cls, characters: tuple[Character, ...]) -> Characters:
@@ -29,27 +31,39 @@
 
     def get_characters(self) -> tuple[Character, ...]:
         return self._characters
 
     def get_active_character_id(self) -> None | int:
         return self._active_character_id
 
+    def just_get_active_character_id(self) -> int:
+        val = self.get_active_character_id()
+        assert val is not None
+        return val
+
     def get_character_in_activity_order(self) -> tuple[Character, ...]:
         for i, character in enumerate(self._characters):
             if character.get_id() == self._active_character_id:
                 return self._characters[i:] + self._characters[:i]
-        return tuple()
+        return self._characters
 
     def get_none_active_characters(self) -> tuple[Character, ...]:
         return tuple(
             char
             for char in self._characters
             if char.get_id() != self.get_active_character_id()
         )
 
+    def get_alive_characters(self) -> tuple[Character, ...]:
+        return tuple(
+            char
+            for char in self._characters
+            if char.alive()
+        )
+
     def get_character(self, id: int) -> None | Character:
         for character in self._characters:
             if id == character.get_id():
                 return character
         return None
 
     def just_get_character(self, id: int) -> Character:
@@ -83,77 +97,73 @@
 
     def get_id(self, character: Character) -> Optional[int]:
         for c in self._characters:
             if character is c:
                 return c.get_id()
         return None
 
-    def get_by_id(self, id: int) -> Optional[Character]:
+    def get_by_id(self, id: int) -> Optional[Character]:  # pragma: no cover
         return self.get_character(id)
 
-    def alive_ids(self) -> list[int]:
-        ids: list[int] = []
-        for character in self._characters:
-            if character.alive():
-                ids.append(character.get_id())
-        return ids
-
     def all_defeated(self) -> bool:
         return all([c.defeated() for c in self._characters])
 
     def char_id_valid(self, char_id: int) -> bool:
         return char_id >= 1 and char_id <= len(self._characters)
 
-    def get_swappable_ids(self) -> tuple[int, ...]:
-        return tuple([
-            i
-            for i, c in enumerate(self._characters)
-            if not c.defeated()
-        ])
-
     def num_characters(self) -> int:
         return len(self._characters)
 
+    def all_elems(self) -> set[Element]:
+        return set(
+            char.element()
+            for char in self._characters
+        )
+
     def factory(self) -> CharactersFactory:
         return CharactersFactory(self)
 
     def _all_unique_data(self) -> tuple:
         return (self._characters, self._active_character_id)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Characters):
             return False
         return self is other or self._all_unique_data() == other._all_unique_data()
 
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
     def __hash__(self) -> int:
         return hash(self._all_unique_data())
 
     def __iter__(self) -> Iterator[Character]:
         return iter(self.get_characters())
 
     def contains(self, char: Character | type[Character]) -> bool:
+        from .character import Character
         if isinstance(char, Character):
             return any(
                 c == char
                 for c in self._characters
             )
-        else:  # assert char: type[chr.Character]
+        else:  # assert char: type[Character]
             return any(
                 type(c) is char
                 for c in self._characters
             )
 
     def __contains__(self, char: Character | type[Character]) -> bool:
         return self.contains(char)
 
     def dict_str(self) -> Union[dict, str]:
         return {
-            "Active Character": self.get_active_character_name(),
+            "Active Character": f"{self.get_active_character_id()}-{self.get_active_character_name()}",
             "Characters": dict([
-                (char.name(), char.dict_str())
+                (f"{char.get_id()}-{char.name()}", char.dict_str())
                 for char in self._characters
             ]),
         }
 
 
 class CharactersFactory:
```

### Comparing `dgisim-0.2.dev2/dgisim/src/character/enums.py` & `dgisim-0.2.dev3/dgisim/src/character/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,7 +19,27 @@
         elif self is CharacterSkill.ELEMENTAL_SKILL1:
             return EventType.ELEMENTAL_SKILL1
         elif self is CharacterSkill.ELEMENTAL_SKILL2:
             return EventType.ELEMENTAL_SKILL2
         elif self is CharacterSkill.ELEMENTAL_BURST:
             return EventType.ELEMENTAL_BURST
         raise NotImplementedError
+
+class WeaponType(Enum):
+    BOW = 0
+    CATALYST = 1
+    CLAYMORE = 2
+    POLEARM = 3
+    SWORD = 4
+    NONE = 5
+
+class Faction(Enum):
+    MONDSTADT = 0
+    LIYUE = 1
+    INAZUMA = 2
+    SUMERU = 3
+    FONTAINE = 4
+    NATLAN = 5
+    SNEZHNAYA = 6
+    FATUI = 7
+    MONSTER = 8
+    HILICHURL = 9
```

### Comparing `dgisim-0.2.dev2/dgisim/src/cli.py` & `dgisim-0.2.dev3/dgisim/src/cli.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev2/dgisim/src/dices.py` & `dgisim-0.2.dev3/dgisim/src/dices.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         else:
             dices = other
         return type(self)(self._dices - dices)
 
     def num_dices(self) -> int:
         return sum(self._dices.values())
 
+    def is_even(self) -> bool:
+        return self.num_dices() % 2 == 0
+
     def is_legal(self) -> bool:
         return all(map(lambda x: x >= 0, self._dices.values())) \
             and all(elem in self._LEGAL_ELEMS for elem in self._dices)
 
     def validify(self) -> Self:
         if self.is_legal():
             return self
@@ -236,25 +239,30 @@
                     omni_required += pures[elem] - remaining.get(elem, 0)
                     remaining[elem] = 0
                 else:
                     answer[elem] += pures[elem]
                     remaining[elem] -= pures[elem]
         if omni > 0:
             best_elem: Optional[Element] = None
-            count = BIG_INT
+            best_count = 0
             for elem in list(_PURE_ELEMS) + [Element.OMNI]:
                 this_count = remaining.get(elem, 0)
-                if this_count >= omni and this_count < count:
+                if best_count > omni and this_count >= omni and this_count < best_count:
+                        best_elem = elem
+                        best_count = this_count
+                elif best_count < omni and this_count > best_count:
                     best_elem = elem
-                    count = this_count
-            if best_elem is None:
-                return None
-            else:
-                answer[best_elem] += omni
-                remaining[best_elem] -= omni
+                    best_count = this_count
+                elif best_count == omni:
+                    break
+            assert best_elem is not None
+            best_count = min(best_count, omni)
+            answer[best_elem] += best_count
+            remaining[best_elem] -= best_count
+            omni_required += omni - best_count
         if any > 0:
             from operator import itemgetter
             sorted_elems = sorted(remaining.items(), key=itemgetter(1))
             for elem, num in sorted_elems:
                 if elem in _PURE_ELEMS:
                     num = min(num, any)
                     answer[elem] += num
@@ -262,15 +270,15 @@
                     any -= num
                     if any == 0:
                         break
             if any > 0:
                 answer[Element.OMNI] += any
                 remaining[Element.OMNI] -= any
         if omni_required > 0:
-            if remaining[Element.OMNI] < omni_required:
+            if remaining.get(Element.OMNI, 0) < omni_required:
                 return None
             answer[Element.OMNI] += omni_required
         return ActualDices(answer)
 
     @classmethod
     def from_random(cls, size: int) -> ActualDices:
         dices = ActualDices.from_empty()
@@ -311,21 +319,13 @@
         Element.DENDRO,
         Element.CRYO,
         Element.GEO,
         Element.ANY,
     })
 
     @classmethod
-    def from_pre(cls, omni: int, any: int, element: Optional[Element] = None, num: Optional[int] = None) -> AbstractDices:
-        assert element is None or element in AbstractDices._LEGAL_ELEMS
-        dices = {Element.OMNI: omni, Element.ANY: any, }
-        if element is not None and num is not None:
-            dices[element] = num
-        return AbstractDices(dices)
-
-    @classmethod
     def from_dices(cls, dices: Dices) -> Optional[AbstractDices]:
         new_dices = AbstractDices(dices._dices)
         if not new_dices.is_legal():
             return None
         else:
             return new_dices
```

### Comparing `dgisim-0.2.dev2/dgisim/src/effect/effect.py` & `dgisim-0.2.dev3/dgisim/src/effect/effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 - base class, which is Effect
 - type classes, used to identify what type of effect an effect is
 - phase classes, effects that controls the flow of the game
 - concrete classes, the implementation of effects that are actually in the game
 """
 from __future__ import annotations
 from dataclasses import asdict, dataclass, field, replace
-from typing import FrozenSet, Iterable, Optional, TYPE_CHECKING, Union
+from typing import cast, FrozenSet, Iterable, Optional, TYPE_CHECKING, Union
 
 from ..character import character as chr
 from ..helper.quality_of_life import dataclass_repr
 from ..status import status as stt
 from ..summon import summon as sm
 from ..support import support as sp
 
 from ..character.enums import CharacterSkill
 from ..element import Element, Reaction, ReactionDetail
+from ..event import *
 from ..helper.quality_of_life import just, case_val
 from ..state.enums import Pid, Act
-from ..status.enums import Preprocessables
+from ..status.enums import Preprocessables, Informables
 from ..status.status_processing import StatusProcessing
 from .enums import DynamicCharacterTarget, TriggeringSignal, Zone
 from .structs import StaticTarget, DamageType
 
 if TYPE_CHECKING:
     from ..card.card import Card
     from ..dices import ActualDices
@@ -64,14 +65,15 @@
     "SwapCharacterCheckerEffect",
     "DeathCheckCheckerEffect",
     "DefeatedCheckerEffect",
 
     # Direct Effect
     "SwapCharacterEffect",
     "ForwardSwapCharacterEffect",
+    "ForwardSwapCharacterCheckEffect",
     "SpecificDamageEffect",
     "ReferredDamageEffect",
     "EnergyRechargeEffect",
     "EnergyDrainEffect",
     "RecoverHPEffect",
     "PublicAddCardEffect",
     "PublicRemoveCardEffect",
@@ -86,29 +88,30 @@
     "UpdateCombatStatusEffect",
     "OverrideCombatStatusEffect",
     "AddSummonEffect",
     "RemoveSummonEffect",
     "UpdateSummonEffect",
     "OverrideSummonEffect",
     "AllSummonIncreaseUsage",
+    "OneSummonDecreaseUsage",
     "OneSummonIncreaseUsage",
     "AddSupportEffect",
     "RemoveSupportEffect",
     "UpdateSupportEffect",
     "OverrideSupportEffect",
     "CastSkillEffect",
     "BroadCastSkillInfoEffect",
 ]
 
 ############################## base ##############################
 
 
 @dataclass(frozen=True, repr=False)
 class Effect:
-    def execute(self, game_state: GameState) -> GameState:
+    def execute(self, game_state: GameState) -> GameState:  # pragma: no cover
         raise Exception("Not Overriden or Implemented")
 
     def name(self) -> str:
         return self.__class__.__name__
 
     def dict_str(self) -> Union[dict, str]:
         return asdict(self)
@@ -154,31 +157,31 @@
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
 class TriggerStatusEffect(TriggerrbleEffect):
     target: StaticTarget
-    status: type[Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]]
+    status: type[Union[stt.HiddenStatus, stt.EquipmentStatus, stt.CharacterStatus]]
     signal: TriggeringSignal
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
-        if not isinstance(character, chr.Character):
+        if not isinstance(character, chr.Character):  # pragma: no cover
             return game_state
         effects: Iterable[Effect] = []
 
         statuses: Statuses
-        if issubclass(self.status, stt.CharacterTalentStatus):
-            statuses = character.get_talent_statuses()
+        if issubclass(self.status, stt.HiddenStatus):
+            statuses = character.get_hidden_statuses()
         elif issubclass(self.status, stt.EquipmentStatus):
             statuses = character.get_equipment_statuses()
         elif issubclass(self.status, stt.CharacterStatus):
             statuses = character.get_character_statuses()
-        else:
+        else:  # pragma: no cover
             raise Exception("Unexpected Status Type to Trigger", self.status)
         status = statuses.find(self.status)
         if status is None:
             return game_state
         effects = status.react_to_signal(game_state, self.target, self.signal)
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
@@ -382,15 +385,15 @@
         effects: list[Effect] = []
         if my_pid.is_player1():
             my_signal = TriggeringSignal.SWAP_EVENT_1
             oppo_signal = TriggeringSignal.SWAP_EVENT_2
         else:
             my_signal = TriggeringSignal.SWAP_EVENT_2
             oppo_signal = TriggeringSignal.SWAP_EVENT_1
-        if my_ac_id != self.my_active.id:
+        if my_ac_id != self.my_active.id:  # pragma: no cover
             effects += [
                 AllStatusTriggererEffect(
                     pid=my_pid,
                     signal=my_signal,
                 ),
             ]
         if oppo_ac_id != self.oppo_active.id:
@@ -420,15 +423,15 @@
             pid = Pid.P2
         else:  # if no one defeated, continue
             return game_state
         death_swap_player = game_state.get_player(pid)
         waiting_player = game_state.get_other_player(pid)
         # TODO: check if game ends
         if death_swap_player.defeated():
-            raise Exception("Not reached, should be caught by DefeatedCheckerEffect")
+            raise Exception("Not Reached! Should be caught by DefeatedCheckerEffect")
         effects: list[Effect] = []
         # TODO: trigger other death based effects
         effects.append(DeathSwapPhaseStartEffect())
         effects.append(DeathSwapPhaseEndEffect(
             pid,
             death_swap_player.get_phase(),
             waiting_player.get_phase(),
@@ -463,62 +466,105 @@
 class SwapCharacterEffect(DirectEffect):
     target: StaticTarget
 
     def execute(self, game_state: GameState) -> GameState:
         assert self.target.zone == Zone.CHARACTERS
         pid = self.target.pid
         player = game_state.get_player(pid)
-        if player.just_get_active_character().get_id() == self.target.id:
+        active_character = player.get_active_character()
+        if active_character is not None and active_character.get_id() == self.target.id:
             return game_state
 
         effects: list[Effect] = [
             AllStatusTriggererEffect(
                 pid,
-                case_val(
-                    pid.is_player1(),
-                    TriggeringSignal.SWAP_EVENT_1,
-                    TriggeringSignal.SWAP_EVENT_2,
-                ),
+                TriggeringSignal.swap_event(pid),
             ),
         ]
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().f_characters(
-                lambda cs: cs.factory().active_character_id(self.target.id).build()
+                lambda cs: cs.factory().active_character_id(cast(int, self.target.id)).build()
             ).build()
         ).f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
 class ForwardSwapCharacterEffect(DirectEffect):
+    """
+    Swap the to the next active character.
+
+    This effect doesn't auto-add swap checker.
+    """
     target_player: Pid
 
     def execute(self, game_state: GameState) -> GameState:
         characters = game_state.get_player(self.target_player).get_characters()
         ordered_chars = characters.get_character_in_activity_order()
-        next_char: Optional[chr.Character] = None
-        for char in ordered_chars[1:] + ordered_chars[:1]:
-            assert isinstance(char, chr.Character)
-            if char.alive():
-                next_char = char
-                break
+        next_char: Optional[chr.Character] = next(
+            (
+                char
+                for char in ordered_chars[1:]
+                if char.alive()
+            ),
+            None
+        )
         if next_char is None:
-            raise Exception("Not reached, there should be defeat checker before")
+            return game_state
         return game_state.factory().f_player(
             self.target_player,
             lambda p: p.factory().f_characters(
                 lambda cs: cs.factory().active_character_id(
                     next_char.get_id()  # type: ignore
                 ).build()
             ).build()
         ).build()
 
 
+@dataclass(frozen=True, repr=False)
+class ForwardSwapCharacterCheckEffect(DirectEffect):
+    """
+    Swap the to the next active character.
+
+    This effect auto-adds swap checker.
+    """
+    target_player: Pid
+
+    def execute(self, game_state: GameState) -> GameState:
+        characters = game_state.get_player(self.target_player).get_characters()
+        ordered_chars = characters.get_character_in_activity_order()
+        next_char: Optional[chr.Character] = next(
+            (
+                char
+                for char in ordered_chars[1:]
+                if char.alive()
+            ),
+            None
+        )
+        if next_char is None:
+            return game_state
+        return game_state.factory().f_player(
+            self.target_player,
+            lambda p: p.factory().f_characters(
+                lambda cs: cs.factory().active_character_id(
+                    next_char.get_id()  # type: ignore
+                ).build()
+            ).build()
+        ).f_effect_stack(
+            lambda es: es.push_one(
+                AllStatusTriggererEffect(
+                    self.target_player,
+                    TriggeringSignal.swap_event(self.target_player),
+                )
+            )
+        ).build()
+
+
 _DAMAGE_ELEMENTS: FrozenSet[Element] = frozenset({
     Element.PYRO,
     Element.HYDRO,
     Element.ANEMO,
     Element.ELECTRO,
     Element.DENDRO,
     Element.CRYO,
@@ -541,19 +587,19 @@
     def _damage_preprocess(
             game_state: GameState, damage: SpecificDamageEffect, pp_type: Preprocessables
     ) -> tuple[GameState, SpecificDamageEffect]:
         source_id = damage.source.pid
         game_state, item = StatusProcessing.preprocess_by_all_statuses(
             game_state,
             source_id,
-            damage,
-            pp_type
+            pp_type,
+            DmgPEvent(dmg=damage),
         )
-        assert type(item) == SpecificDamageEffect
-        damage = item
+        assert isinstance(item, DmgPEvent), item
+        damage = item.dmg
         return game_state, damage
 
     @classmethod
     def _element_confirmation(
             cls, game_state: GameState, damage: SpecificDamageEffect
     ) -> tuple[GameState, SpecificDamageEffect]:
         """ This is the pass to check final damage element """
@@ -618,28 +664,37 @@
         )
         if reaction is not None:
             reactioned_damage = replace(
                 reactioned_damage,
                 damage=reactioned_damage.damage + reaction.reaction_type.damage_boost(),
             )
         game_state, actual_damage = self._damage_confirmation(game_state, reactioned_damage)
+        # Update all statuses with this damage
+        game_state = StatusProcessing.inform_all_statuses(
+            game_state,
+            actual_damage.source.pid,
+            Informables.DMG_DELT,
+            DmgIEvent(dmg=actual_damage),
+        )
 
         # Get damage target
         target = game_state.get_character_target(actual_damage.target)
-        if target is None:
+        if target is None:  # pragma: no cover
             return game_state
 
         # Damage Calculation
         hp = target.get_hp()
         hp = max(0, hp - actual_damage.damage)
 
-        pid = self.target.pid
+        target_pid = self.target.pid
         effects: list[Effect] = [DefeatedCheckerEffect()]
 
-        # LATESET_TODO: use the reaction information to generate further effects
+        if hp != target.get_hp():
+            target = target.factory().hp(hp).build()
+
         if reaction is None:
             pass
 
         elif reaction.reaction_type is Reaction.VAPORIZE \
                 or reaction.reaction_type is Reaction.MELT:
             pass
 
@@ -647,15 +702,15 @@
             oppo_active_id = game_state \
                 .get_player(actual_damage.target.pid) \
                 .just_get_active_character() \
                 .get_id()
             assert actual_damage.target.zone is Zone.CHARACTERS
             if actual_damage.target.id is oppo_active_id:
                 effects.append(
-                    ForwardSwapCharacterEffect(pid)
+                    ForwardSwapCharacterEffect(target_pid)
                 )
 
         elif reaction.reaction_type is Reaction.SUPERCONDUCT \
                 or reaction.reaction_type is Reaction.ELECTRO_CHARGED:
             effects.append(
                 ReferredDamageEffect(
                     source=self.source,
@@ -715,30 +770,38 @@
             effects.append(
                 AddSummonEffect(
                     target_pid=actual_damage.source.pid,
                     summon=sm.BurningFlameSummon,
                 )
             )
 
-        else:
+        else:  # pragma: no cover
             # this exception shouldn't be reached by now, but leave it here just to be safe
             raise Exception(f"Reaction {reaction.reaction_type} not handled")
 
-        if hp != target.get_hp():
-            target = target.factory().hp(hp).build()
-
-        return game_state.factory().f_player(
-            pid,
+        # damaged game state
+        game_state = game_state.factory().f_player(
+            target_pid,
             lambda p: p.factory().f_characters(
                 lambda cs: cs.factory().character(target).build()  # type: ignore
             ).build()
         ).f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
+        if target.defeated():
+            game_state = StatusProcessing.inform_all_statuses(
+                game_state,
+                self.source.pid,
+                Informables.CHARACTER_DEATH,
+                CharacterDeathIEvent(target=self.target),
+            )
+
+        return game_state
+
 
 @dataclass(frozen=True, repr=False)
 class ReferredDamageEffect(DirectEffect):
     source: StaticTarget
     target: DynamicCharacterTarget
     element: Element
     damage: int
@@ -747,14 +810,15 @@
     # e.g. super-conduct caused by swirl
     target_ref: Optional[StaticTarget] = field(kw_only=True, default=None)
 
     def legal(self) -> bool:
         return self.element in _DAMAGE_ELEMENTS
 
     def execute(self, game_state: GameState) -> GameState:
+        assert self.legal()
         targets: list[Optional[chr.Character]] = []
         effects: list[Effect] = []
         char: Optional[chr.Character]
 
         if self.target is DynamicCharacterTarget.OPPO_ACTIVE:
             targets.append(
                 game_state.get_other_player(self.source.pid).get_characters().get_active_character()
@@ -763,26 +827,30 @@
             opponenet_characters = game_state.get_other_player(self.source.pid).get_characters()
             avoided_id: int
             if self.target_ref is None:
                 avoided_id = just(opponenet_characters.get_active_character_id())
             else:
                 assert self.target_ref.pid is self.source.pid.other()
                 assert self.target_ref.zone is Zone.CHARACTERS
-                avoided_id = self.target_ref.id
+                avoided_id = cast(int, self.target_ref.id)
             for char in opponenet_characters.get_characters():
                 if char.get_id() != avoided_id:
                     targets.append(char)
-        else:
+        elif self.target is DynamicCharacterTarget.SELF_SELF:
+            targets.append(
+                game_state.get_player(self.source.pid).get_characters().get_active_character()
+            )
+        else:  # pragma: no cover
             raise Exception("Not implemented yet")
 
         for char in targets:
-            if char is None:
+            if char is None:  # pragma: no cover
                 continue
             pid = game_state.belongs_to(char)
-            if pid is None:
+            if pid is None:  # pragma: no cover
                 continue
             effects.append(
                 SpecificDamageEffect(
                     source=self.source,
                     target=StaticTarget(
                         pid=pid,
                         zone=Zone.CHARACTERS,
@@ -803,15 +871,15 @@
 @dataclass(frozen=True, repr=False)
 class EnergyRechargeEffect(DirectEffect):
     target: StaticTarget
     recharge: int
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
-        if not isinstance(character, chr.Character):
+        if not isinstance(character, chr.Character):  # pragma: no cover
             return game_state
         energy = min(character.get_energy() + self.recharge, character.get_max_energy())
         if energy == character.get_energy():
             return game_state
         character = character.factory().energy(energy).build()
         player = game_state.get_player(self.target.pid)
         characters = player.get_characters().factory().character(character).build()
@@ -825,15 +893,15 @@
 @dataclass(frozen=True, repr=False)
 class EnergyDrainEffect(DirectEffect):
     target: StaticTarget
     drain: int
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
-        if not isinstance(character, chr.Character):
+        if not isinstance(character, chr.Character):  # pragma: no cover
             return game_state
         energy = max(character.get_energy() - self.drain, 0)
         if energy == character.get_energy():
             return game_state
         character = character.factory().energy(energy).build()
         player = game_state.get_player(self.target.pid)
         characters = player.get_characters().factory().character(character).build()
@@ -847,15 +915,15 @@
 @dataclass(frozen=True, repr=False)
 class RecoverHPEffect(DirectEffect):
     target: StaticTarget
     recovery: int
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
-        if not isinstance(character, chr.Character):
+        if not isinstance(character, chr.Character):  # pragma: no cover
             return game_state
         hp = min(character.get_hp() + self.recovery, character.get_max_hp())
         if hp == character.get_hp():
             return game_state
         return game_state.factory().f_player(
             self.target.pid,
             lambda p: p.factory().f_characters(
@@ -888,15 +956,15 @@
     pid: Pid
     card: type[Card]
 
     def execute(self, game_state: GameState) -> GameState:
         pid = self.pid
         card = self.card
         hand_cards = game_state.get_player(pid).get_hand_cards()
-        if not hand_cards.contains(card):
+        if not hand_cards.contains(card):  # pragma: no cover
             return game_state
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().f_hand_cards(
                 lambda cs: cs.remove(card)
             ).f_publicly_used_cards(
                 lambda cs: cs.add(card)
@@ -909,15 +977,15 @@
     pid: Pid
     card: type[Card]
 
     def execute(self, game_state: GameState) -> GameState:
         pid = self.pid
         card = self.card
         hand_cards = game_state.get_player(pid).get_hand_cards()
-        if not hand_cards.contains(card) or hand_cards[card] <= 0:
+        if not hand_cards.contains(card) or hand_cards[card] <= 0:  # pragma: no cover
             return game_state
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().f_hand_cards(
                 lambda cs: cs.remove_all(card)
             ).f_publicly_used_cards(
                 lambda cs: cs + {card: hand_cards[card]}
@@ -941,21 +1009,21 @@
             lambda p: p.factory().dices(new_dices).build()
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
 class AddCharacterStatusEffect(DirectEffect):
     target: StaticTarget
-    status: type[Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]]
+    status: type[Union[stt.HiddenStatus, stt.EquipmentStatus, stt.CharacterStatus]]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
-        if issubclass(self.status, stt.CharacterTalentStatus):
-            character = character.factory().f_talents(
+        if issubclass(self.status, stt.HiddenStatus):  # pragma: no cover
+            character = character.factory().f_hiddens(
                 lambda ts: ts.update_status(self.status())
             ).build()
         elif issubclass(self.status, stt.EquipmentStatus):
             character = character.factory().f_equipments(
                 lambda es: es.update_status(self.status())
             ).build()
         elif issubclass(self.status, stt.CharacterStatus):
@@ -969,23 +1037,23 @@
             ).build()
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
 class RemoveCharacterStatusEffect(DirectEffect):
     target: StaticTarget
-    status: type[Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]]
+    status: type[Union[stt.HiddenStatus, stt.EquipmentStatus, stt.CharacterStatus]]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_character_target(self.target)
-        if character is None:
+        if character is None:  # pragma: no cover
             return game_state
         new_character = character
-        if issubclass(self.status, stt.CharacterTalentStatus):
-            new_character = character.factory().f_talents(
+        if issubclass(self.status, stt.HiddenStatus):  # pragma: no cover
+            new_character = character.factory().f_hiddens(
                 lambda ts: ts.remove(self.status)
             ).build()
         elif issubclass(self.status, stt.EquipmentStatus):
             new_character = character.factory().f_equipments(
                 lambda es: es.remove(self.status)
             ).build()
         elif issubclass(self.status, stt.CharacterStatus):
@@ -999,21 +1067,21 @@
             ).build()
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
 class UpdateCharacterStatusEffect(DirectEffect):
     target: StaticTarget
-    status: Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]
+    status: Union[stt.HiddenStatus, stt.EquipmentStatus, stt.CharacterStatus]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
-        if isinstance(self.status, stt.CharacterTalentStatus):
-            character = character.factory().f_talents(
+        if isinstance(self.status, stt.HiddenStatus):  # pragma: no cover
+            character = character.factory().f_hiddens(
                 lambda ts: ts.update_status(self.status)
             ).build()
         elif isinstance(self.status, stt.EquipmentStatus):
             character = character.factory().f_equipments(
                 lambda es: es.update_status(self.status)
             ).build()
         elif isinstance(self.status, stt.CharacterStatus):
@@ -1027,21 +1095,21 @@
             ).build()
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
 class OverrideCharacterStatusEffect(DirectEffect):
     target: StaticTarget
-    status: Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]
+    status: Union[stt.HiddenStatus, stt.EquipmentStatus, stt.CharacterStatus]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
-        if isinstance(self.status, stt.CharacterTalentStatus):
-            character = character.factory().f_talents(
+        if isinstance(self.status, stt.HiddenStatus):
+            character = character.factory().f_hiddens(
                 lambda ts: ts.update_status(self.status, override=True)
             ).build()
         elif isinstance(self.status, stt.EquipmentStatus):
             character = character.factory().f_equipments(
                 lambda es: es.update_status(self.status, override=True)
             ).build()
         elif isinstance(self.status, stt.CharacterStatus):
@@ -1186,29 +1254,51 @@
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
 @dataclass(frozen=True, kw_only=True, repr=False)
 class OneSummonIncreaseUsage(DirectEffect):
-    target_pid: Pid
-    summon_type: type[sm.Summon]
+    target: StaticTarget
     d_usages: int = 1
 
     def execute(self, game_state: GameState) -> GameState:
         effects: list[Effect] = []
-        summons = game_state.get_player(self.target_pid).get_summons()
-        summon = summons.find(summon_type=self.summon_type)
-        if summon is None:
+        summons = game_state.get_player(self.target.pid).get_summons()
+        summon = summons.find(summon_type=cast(type[sm.Summon], self.target.id))
+        if summon is None:  # pragma: no cover
             return game_state
 
         effects.append(
             OverrideSummonEffect(
-                target_pid=self.target_pid,
-                summon=replace(summon, usages=summon.usages + 1),
+                target_pid=self.target.pid,
+                summon=replace(summon, usages=summon.usages + self.d_usages),
+            )
+        )
+        return game_state.factory().f_effect_stack(
+            lambda es: es.push_many_fl(effects)
+        ).build()
+
+
+@dataclass(frozen=True, kw_only=True, repr=False)
+class OneSummonDecreaseUsage(DirectEffect):
+    target: StaticTarget
+    d_usages: int = 1
+
+    def execute(self, game_state: GameState) -> GameState:
+        effects: list[Effect] = []
+        summons = game_state.get_player(self.target.pid).get_summons()
+        summon = summons.find(summon_type=cast(type[sm.Summon], self.target.id))
+        if summon is None:  # pragma: no cover
+            return game_state
+
+        effects.append(
+            UpdateSummonEffect(
+                target_pid=self.target.pid,
+                summon=replace(summon, usages=summon.usages + self.d_usages),
             )
         )
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
@@ -1272,18 +1362,18 @@
 class CastSkillEffect(DirectEffect):
     target: StaticTarget
     skill: CharacterSkill
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
-        if not character.can_cast_skill():
+        if not character.can_cast_skill():  # pragma: no cover
             return game_state
-        effects = character.skill(game_state, self.skill)
-        if not effects:
+        effects = character.skill(game_state, self.target, self.skill)
+        if not effects:  # pragma: no cover
             return game_state
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
 @dataclass(frozen=True, repr=False)
@@ -1291,10 +1381,13 @@
     source: StaticTarget
     skill: CharacterSkill
 
     def execute(self, game_state: GameState) -> GameState:
         return StatusProcessing.inform_all_statuses(
             game_state,
             self.source.pid,
-            self.skill,
-            source=self.source,
+            Informables.SKILL_USAGE,
+            SkillIEvent(
+                source=self.source,
+                skill_type=self.skill,
+            ),
         )
```

### Comparing `dgisim-0.2.dev2/dgisim/src/effect/effect_stack.py` & `dgisim-0.2.dev3/dgisim/src/effect/effect_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,19 @@
             if type(effect) == effect_type:
                 return True
         return False
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, EffectStack):
             return False
-        return self._effects == other._effects
+        return self is other or self._effects == other._effects
 
     def __hash__(self) -> int:
         return hash(self._effects)
 
-    def to_string(self, indent: int) -> str:
-        return str(self)
-
     def __str__(self) -> str:
         return str(self._effects)
 
     def dict_str(self) -> dict | str:
         content = {}
         for i, effect in enumerate(reversed(self._effects)):
             content[f"{str(i)}-{effect.name()}"] = effect.dict_str()
```

### Comparing `dgisim-0.2.dev2/dgisim/src/element.py` & `dgisim-0.2.dev3/dgisim/src/element.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     DENDRO = 5
     CRYO = 6
     GEO = 7
     PHYSICAL = 8
     PIERCING = 9
     ANY = 10
 
+    def __repr__(self) -> str:
+        return self.name
+
 
 AURA_ELEMENTS_ORDERED: tuple[Element, ...] = (
     Element.PYRO,
     Element.HYDRO,
     Element.ELECTRO,
     Element.CRYO,
     Element.DENDRO,
@@ -119,14 +122,24 @@
     def consult_reaction(cls, first: Element, second: Element) -> Optional[Reaction]:
         for reaction in cls:
             e1, e2 = reaction.value.reaction_elems
             if (first in e1 and second in e2) or (first in e2 and second in e1):
                 return reaction
         return None
 
+    @classmethod
+    def consult_reaction_with_aura(
+            cls, aura: ElementalAura, second: Element
+    ) -> None | ReactionDetail:
+        for elem in aura:
+            reaction = cls.consult_reaction(elem, second)
+            if reaction is not None:
+                return ReactionDetail(reaction, elem, second)
+        return None
+
     def damage_boost(self) -> int:
         return self.value.damage_boost
 
 
 @dataclass(frozen=True)
 class ReactionDetail:
     reaction_type: Reaction
@@ -183,14 +196,17 @@
             for e, aura in self._aura.items()
         ))
 
     def contains(self, elem: Element) -> bool:
         assert elem in AURA_ELEMENTS
         return self._aura[elem]
 
+    def __contains__(self, elem: Element) -> bool:
+        return self.contains(elem)
+
     def has_aura(self) -> bool:
         return any(self._aura.values())
 
     def elem_auras(self) -> tuple[Element, ...]:
         return tuple(iter(self))
 
     def __iter__(self) -> Iterator[Element]:
```

### Comparing `dgisim-0.2.dev2/dgisim/src/game_state_machine.py` & `dgisim-0.2.dev3/dgisim/src/game_state_machine.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev2/dgisim/src/helper/hashable_dict.py` & `dgisim-0.2.dev3/dgisim/src/helper/hashable_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
         A frozen HashableDict could be shared by multiple references thinking
         they have different HashableDicts, modifying this one may cause unexpected
         behaviour elsewhere.
         """
         # use a trick to bypass overriden __setattr__() avoiding exception
         object.__setattr__(self, "_frozen", False)
+        self._frozen_set = None
 
     def frozen(self) -> bool:
         if hasattr(self, "_frozen"):
             return self._frozen
         return False
 
     def __setattr__(self, *args, **kwargs):
@@ -100,26 +101,28 @@
                         for item in self.items()
                         if item[1] != 0
                     ),
                 )
             assert self._frozen_set is not None
             return self._frozen_set
         else:
-            self._frozen_set = None
             return frozenset(
                 item
                 for item in self.items()
                 if item[1] != 0
             )
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, HashableDict):
             return False
         return self is other or self._to_frozen_set() == other._to_frozen_set()
 
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
     def __hash__(self) -> int:  # type: ignore
         """ Exception is raised if the HashableDict is not frozen. """
         if not self.frozen():
             raise Exception("Calling __hash__() to a non-frozen HashableDict!")
         return hash(self._to_frozen_set())
 
     def all_val_non_negative(self) -> bool:
```

### Comparing `dgisim-0.2.dev2/dgisim/src/helper/level_print.py` & `dgisim-0.2.dev3/dgisim/src/helper/level_print.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,22 +103,22 @@
             board.insert_at_nextline(y, GamePrinter._pair(d, key))
 
     @staticmethod
     def _insert_character(name: str, character: dict) -> StrDrawer:
         board = StrDrawer()
         board.insert_at(0, 0, f"<{name}>")
         GamePrinter._insert_lines(board, 2, character, [
-            "id",
+            # "id",
             "Aura",
         ])
         board.insert_at_nextline(2, f"<HP: {character['HP']}/{character['Max HP']}>")
         board.insert_at_nextline(2, f"<Energy: {character['Energy']}/{character['Max Energy']}>")
         board.insert_board_at_nextline(
             2,
-            GamePrinter._insert_str_list("Talents", character["Talents"])
+            GamePrinter._insert_str_list("Hiddens", character["Hiddens"])
         )
         board.insert_board_at_nextline(
             2,
             GamePrinter._insert_str_list("Equipments", character["Equipments"])
         )
         board.insert_board_at_nextline(
             2,
```

### Comparing `dgisim-0.2.dev2/dgisim/src/helper/quality_of_life.py` & `dgisim-0.2.dev3/dgisim/src/helper/quality_of_life.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,15 @@
     "case_val",
     "dataclass_repr",
     "just",
 ]
 
 _T = TypeVar('_T')
 
-
-def just(optional_val: None | _T, backup: None | _T = None) -> _T:
-    """
-    Removes Optional and get value directly
-    Throws exception if it is indeed None
-    """
-    if optional_val is None:
-        if backup is None:
-            raise Exception("Trying to just None")
-        else:
-            return backup
-    return optional_val
+BIG_INT = 0x7fffffff
 
 
 def case_val(condition: bool, first: _T, second: _T) -> _T:
     """ if condition is True; then return first; else return second """
     return first if condition else second
 
 
@@ -44,8 +33,18 @@
     paired_fields = (
         f"{field.name}={field_val_to_str(self.__getattribute__(field.name))}"
         for field in cls_fields
     )
     return f"{self.__class__.__name__}({', '.join(paired_fields)})"
 
 
-BIG_INT = 0x7fffffff
+def just(optional_val: None | _T, backup: None | _T = None) -> _T:
+    """
+    Removes Optional and get value directly
+    Throws exception if it is indeed None
+    """
+    if optional_val is None:
+        if backup is None:
+            raise Exception("Trying to just None")
+        else:
+            return backup
+    return optional_val
```

### Comparing `dgisim-0.2.dev2/dgisim/src/mode.py` & `dgisim-0.2.dev3/dgisim/src/mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 from .dices import AbstractDices
 from .element import *
 from .event import *
 from .helper.level_print import level_print_single
 
@@ -13,15 +14,15 @@
 
 __all__ = [
     "Mode",
     "DefaultMode",
 ]
 
 
-class Mode:
+class Mode(ABC):
     """
     Base Mode for all modes.
 
     A mode is what that contains all configurations for a 'version' of a game.
 
     e.g. It contains how many cards a player can have, how many summons can a
     player have...
@@ -60,37 +61,45 @@
 
     def swap_cost(self) -> AbstractDices:
         return self._SWAP_COST
 
     def swap_speed(self) -> EventSpeed:
         return self._SWAP_SPEED
 
+    @abstractmethod
     def all_cards(self) -> frozenset[type[Card]]:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def all_chars(self) -> frozenset[type[Character]]:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def card_select_phase(self) -> Phase:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def starting_hand_select_phase(self) -> Phase:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def roll_phase(self) -> Phase:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def action_phase(self) -> Phase:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def end_phase(self) -> Phase:
-        raise Exception("Not Overridden")
+        pass
 
+    @abstractmethod
     def game_end_phase(self) -> Phase:
-        raise Exception("Not Overridden")
+        pass
 
     def __eq__(self, other: object) -> bool:
         return type(self) == type(other)
 
     def __hash__(self) -> int:
         return hash(type(self))
 
@@ -132,9 +141,14 @@
         from .phase.default.end_phase import EndPhase
         return EndPhase()
 
     def game_end_phase(self) -> Phase:
         from .phase.default.game_end_phase import GameEndPhase
         return GameEndPhase()
 
-    def __hash__(self) -> int:
-        return hash(self.__class__.__name__)
+
+class AllOmniMode(DefaultMode):
+    _DICE_REROLL_CHANCES = 0
+
+    def roll_phase(self) -> Phase:
+        from .phase.all_omni.roll_phase import RollPhase
+        return RollPhase()
```

### Comparing `dgisim-0.2.dev2/dgisim/src/phase/default/action_phase.py` & `dgisim-0.2.dev3/dgisim/src/phase/default/action_phase.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,36 +50,32 @@
                 Act.PASSIVE_WAIT_PHASE
             ).build()
         ).build()
 
     def _execute_effect(self, game_state: GameState) -> GameState:
         effect_stack, effect = game_state.get_effect_stack().pop()
         new_game_state = game_state.factory().effect_stack(effect_stack).build()
-        if isinstance(effect, DeathSwapPhaseStartEffect):
-            print("AFTER DEATH:", new_game_state)
         return effect.execute(new_game_state)
 
     def _is_executing_effects(self, game_state: GameState) -> bool:
         effect_stack = game_state.get_effect_stack()
         return not effect_stack.is_empty() \
             and not isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect)
 
     def step(self, game_state: GameState) -> GameState:
         p1 = game_state.get_player1()
         p2 = game_state.get_player2()
-        p1p = p1.get_phase()
-        p2p = p2.get_phase()
-        if p1p is Act.ACTION_PHASE or p2p is Act.ACTION_PHASE:
+        if p1.is_action_phase() or p2.is_action_phase():
             assert self._is_executing_effects(game_state)
             return self._execute_effect(game_state)
-        elif p1p is Act.PASSIVE_WAIT_PHASE and p2p is Act.PASSIVE_WAIT_PHASE:
+        elif p1.is_passive_wait_phase() and p2.is_passive_wait_phase():
             return self._start_up_phase(game_state)
-        elif p1p is Act.END_PHASE and p2p is Act.END_PHASE:
+        elif p1.is_end_phase() and p2.is_end_phase():
             return self._to_end_phase(game_state)
-        raise Exception("Unknown Game State to process")
+        raise Exception("Not Reached! Unknown Game State to process")
 
     def _handle_end_round(
             self,
             game_state: GameState,
             pid: Pid,
             action: EndRoundAction
     ) -> GameState:
@@ -87,19 +83,17 @@
         assert active_player_id == pid
         active_player = game_state.get_player(active_player_id)
         other_player = game_state.get_other_player(active_player_id)
         if other_player.get_phase() is Act.END_PHASE:
             other_player_new_phase = Act.END_PHASE
         elif other_player.get_phase() is Act.PASSIVE_WAIT_PHASE:
             other_player_new_phase = Act.ACTION_PHASE
-        else:
+        else:  # pragma: no cover
             print(f"ERROR pid={pid}\n {game_state}")
             raise Exception(f"Unknown Game State to process {other_player.get_phase()}")
-        if pid is not active_player_id:
-            raise Exception("Unknown Game State to process")
         return game_state.factory().active_player_id(
             active_player_id.other()
         ).player(
             active_player_id,
             active_player.factory().phase(
                 Act.END_PHASE
             ).build()
@@ -119,31 +113,31 @@
         # Check action validity
         result = game_state.skill_checker().valid_action(pid, action)
         if result is None:
             raise Exception(f"{action} from {pid} is invalid for gamestate:\n{game_state}")
         game_state = result
 
         player = game_state.get_player(pid)
-        # TODO: check validity of the action
         instruction = action.instruction
         new_effects: list[Effect] = []
-        # TODO: put pre checks
         # Costs
         dices = player.get_dices()
-        new_dices = dices - action.instruction.dices
-        if new_dices is None:
-            return None
+        new_dices = dices - instruction.dices
+        assert new_dices.is_legal()
         # Skill Effect
         active_character = player.get_characters().get_active_character()
-        if active_character is None:
-            return None
+        assert active_character is not None
         assert active_character.can_cast_skill()
         # note: it's important to cast skill before new_dices are putted into the game_state
         #       so that normal_attacks can correctly be marked as charged attack
-        new_effects += active_character.skill(game_state, action.skill)
+        new_effects += active_character.skill(
+            game_state,
+            StaticTarget(pid, Zone.CHARACTERS, active_character.get_id()),
+            action.skill
+        )
         new_effects.append(AllStatusTriggererEffect(
             pid,
             TriggeringSignal.COMBAT_ACTION,
         ))
         new_effects.append(TurnEndEffect())
         # Afterwards
         return game_state.factory().f_effect_stack(
@@ -221,18 +215,15 @@
         #  setup
         player = game_state.get_player(pid)
         new_effects: list[Effect] = []
 
         # Costs
         dices = player.get_dices()
         new_dices = dices - paid_dices
-        if not new_dices.is_legal():
-            print(f"Fail with new dices: <{new_dices}> for card: {card.name()}")
-            assert False
-            return None
+        assert new_dices.is_legal()
 
         # Card
         new_effects.append(PublicRemoveCardEffect(pid, card))
         new_effects += card.effects(game_state, pid, action.instruction)
         if card.is_combat_action():
             new_effects.append(AllStatusTriggererEffect(
                 pid,
@@ -315,15 +306,15 @@
             return self._handle_swap_action(game_state, pid, action)
         elif isinstance(action, CardAction):
             return self._handle_card_action(game_state, pid, action)
         elif isinstance(action, ElementalTuningAction):
             return self._handle_elemental_tuning_action(game_state, pid, action)
         elif isinstance(action, DeathSwapAction):
             return self._handle_death_swap_action(game_state, pid, action)
-        raise Exception("Unhandld action", action)
+        raise Exception("Unhandld action", action)  # pragma: no cover
 
     def step_action(
             self,
             game_state: GameState,
             pid: Pid,
             action: PlayerAction
     ) -> Optional[GameState]:
@@ -337,15 +328,15 @@
                 raise Exception(f"Trying to execute {action} when a death swap is expected")
             # game_state = game_state.factory().effect_stack(effect_stack.pop()[0]).build()
 
         if isinstance(action, GameAction):
             return self._handle_game_action(game_state, pid, action)
         elif isinstance(action, EndRoundAction):
             return self._handle_end_round(game_state, pid, action)
-        raise Exception("Unknown Game State to process")
+        raise Exception("Not Reached! Unknown Game State to process")
 
     def waiting_for(self, game_state: GameState) -> Optional[Pid]:
         effect_stack = game_state.get_effect_stack()
         # if no effects are to be executed or death swap phase is inserted
         if effect_stack.is_empty() or game_state.death_swapping():
             return super().waiting_for(game_state)
         else:
@@ -410,15 +401,15 @@
             return just(SkillActGenGenerator.action_generator(game_state, pid))
         elif player_choice is ActionType.ELEMENTAL_TUNING:
             assert game_state.elem_tuning_checker().usable(pid)
             from ...action.action_generator_generator import ElemTuningActGenGenerator
             return just(ElemTuningActGenGenerator.action_generator(game_state, pid))
         elif player_choice is ActionType.END_ROUND:
             return ActionGenerator(game_state=game_state, pid=pid, action=EndRoundAction())
-        else:
+        else:  # pragma: no cover
             action_type_name = ActionType.__name__
             if isinstance(player_choice, ActionType):
                 raise Exception(f"Unhandled player {action_type_name} {player_choice}")
             else:
                 raise TypeError(f"Unexpected player choice {player_choice} where"
                                 + f"where {action_type_name} is expected")
 
@@ -427,13 +418,7 @@
             return None
         return ActionGenerator(
             game_state=game_state,
             pid=pid,
             _choices_helper=self._choices_helper,
             _fill_helper=self._fill_helper,
         )
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, ActionPhase)
-
-    def __hash__(self) -> int:
-        return hash(self.__class__.__name__)
```

### Comparing `dgisim-0.2.dev2/dgisim/src/phase/default/card_select_phase.py` & `dgisim-0.2.dev3/dgisim/src/phase/default/card_select_phase.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         elif p1.get_phase() is Act.END_PHASE and p2.get_phase() is Act.END_PHASE:
             return self._to_starting_hand_select_phase(game_state)
         else:
             raise Exception("Unknown Game State to process")
 
     def _handle_card_drawing(self, game_state: GameState, pid: Pid, action: CardsSelectAction) -> GameState:
         player: PlayerState = game_state.get_player(pid)
-        new_deck, new_cards = player.get_deck_cards().pick_random_cards(action.num_cards())
+        new_deck, new_cards = player.get_deck_cards().pick_random_cards(action.selected_cards.num_cards())
         new_deck = new_deck + action.selected_cards
         new_hand = player.get_hand_cards() - action.selected_cards
         new_hand = new_hand + new_cards
         new_redraw_chances: int = player.get_card_redraw_chances() - 1
         new_player_phase: Act
         if new_redraw_chances > 0:
             new_player_phase = player.get_phase()
@@ -128,15 +128,15 @@
         pid = action_generator.pid
 
         if player_choice is ActionType.SELECT_CARDS:
             from ...action.action_generator_generator import CardsSelectionActGenGenerator
             return just(CardsSelectionActGenGenerator.action_generator(game_state, pid))
         elif player_choice is ActionType.END_ROUND:
             return ActionGenerator(game_state=game_state, pid=pid, action=EndRoundAction())
-        else:
+        else:  # pragma: no cover
             action_type_name = ActionType.__name__
             if isinstance(player_choice, ActionType):
                 raise Exception(f"Unhandled player {action_type_name} {player_choice}")
             else:
                 raise TypeError(f"Unexpected player choice {player_choice} where"
                                 + f"where {action_type_name} is expected")
 
@@ -145,13 +145,7 @@
             return None
         return ActionGenerator(
             game_state=game_state,
             pid=pid,
             _choices_helper=self._choices_helper,
             _fill_helper=self._fill_helper,
         )
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, CardSelectPhase)
-
-    def __hash__(self) -> int:
-        return hash(self.__class__.__name__)
```

### Comparing `dgisim-0.2.dev2/dgisim/src/phase/default/end_phase.py` & `dgisim-0.2.dev3/dgisim/src/phase/default/end_phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,62 +75,51 @@
             ).hand_cards(
                 other_player_hand
             ).deck_cards(
                 other_player_deck
             ).build()
         ).build()
 
-    def _end_both_players(self, game_state: GameState) -> GameState:
-        return game_state.factory().f_player1(
-            lambda p: p.factory().phase(
-                Act.END_PHASE
-            ).build()
-        ).f_player2(
-            lambda p: p.factory().phase(
-                Act.END_PHASE
-            ).build()
-        ).build()
-
     def _end_game(self, game_state: GameState) -> GameState:
         return game_state.factory().phase(
             game_state.get_mode().game_end_phase()
         ).build()
 
     def _execute_effect(self, game_state: GameState) -> GameState:
         effect_stack, effect = game_state.get_effect_stack().pop()
         new_game_state = game_state.factory().effect_stack(effect_stack).build()
         if isinstance(effect, DeathSwapPhaseStartEffect):
-            print("AFTER DEATH:", new_game_state)
+            raise Exception("Not Reached!")
         return effect.execute(new_game_state)
 
     def _is_executing_effects(self, game_state: GameState) -> bool:
         effect_stack = game_state.get_effect_stack()
         return not effect_stack.is_empty() \
             and not isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect)
 
     def step(self, game_state: GameState) -> GameState:
         p1 = game_state.get_player1()
         p2 = game_state.get_player2()
         active_player_id = game_state.get_active_player_id()
-        if p1.get_phase() is Act.PASSIVE_WAIT_PHASE and p2.get_phase() is Act.PASSIVE_WAIT_PHASE:
+        if p1.is_passive_wait_phase() and p2.is_passive_wait_phase():
             return self._initialize_end_phase(game_state)
-        elif p1.get_phase() is Act.ACTIVE_WAIT_PHASE or p2.get_phase() is Act.ACTIVE_WAIT_PHASE:
+        elif p1.is_active_wait_phase() or p2.is_active_wait_phase():
             assert self._is_executing_effects(game_state)
             return self._execute_effect(game_state)
-        elif p1.get_phase().is_action_phase() or p2.get_phase().is_action_phase():
+        elif p1.is_action_phase() or p2.is_action_phase():
             # handling death swap
             assert self._is_executing_effects(game_state)
             return self._execute_effect(game_state)
-        elif p1.get_phase() is Act.END_PHASE and p2.get_phase() is Act.END_PHASE:
+        elif p1.is_end_phase() and p2.is_end_phase():
             new_round = game_state.get_round() + 1
             if new_round > game_state.get_mode().round_limit():
                 return self._end_game(game_state)
             else:
                 return self._to_roll_phase(game_state, new_round)
-        raise Exception("Unknown Game State to process")
+        raise Exception("Unknown Game State to process")  # pragma: no cover
 
     def _handle_death_swap_action(
             self,
             game_state: GameState,
             pid: Pid,
             action: DeathSwapAction
     ) -> Optional[GameState]:
@@ -167,18 +156,12 @@
         if effect_stack.is_not_empty() \
                 and isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect):
             return super().waiting_for(game_state)
         else:
             return None
 
     def action_generator(self, game_state: GameState, pid: Pid) -> ActionGenerator | None:
-        if pid is not self.waiting_for(game_state):
+        if pid is not self.waiting_for(game_state):  # pragma: no cover
             return None
         assert game_state.death_swapping(pid)
         from ...action.action_generator_generator import SwapActGenGenerator
         return SwapActGenGenerator.action_generator(game_state, pid)
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, EndPhase)
-
-    def __hash__(self) -> int:
-        return hash(self.__class__.__name__)
```

### Comparing `dgisim-0.2.dev2/dgisim/src/phase/default/game_end_phase.py` & `dgisim-0.2.dev3/dgisim/src/phase/phase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,50 @@
 from __future__ import annotations
+from abc import abstractmethod
 from typing import TYPE_CHECKING
 
-from .. import phase as ph
+from ..helper.level_print import level_print_single
 
 if TYPE_CHECKING:
-    from ...action.action import PlayerAction
-    from ...action.action_generator import ActionGenerator
-    from ...state.game_state import GameState
-    from ...state.enums import Pid
+    from ..state.game_state import GameState
+    from ..action.action import PlayerAction
+    from ..action.action_generator import ActionGenerator
+    from ..state.enums import Pid
 
 __all__ = [
-    "GameEndPhase",
+    "Phase",
 ]
 
 
-class GameEndPhase(ph.Phase):
+class Phase:
+    @abstractmethod
     def step(self, game_state: GameState) -> GameState:
-        raise Exception("Not Reached")
+        raise NotImplementedError
 
-    def step_action(self, game_state: GameState, pid: Pid, action: PlayerAction) -> None | GameState:
-        raise Exception("Not Reached")
+    @abstractmethod
+    def step_action(
+        self,
+        game_state: GameState,
+        pid: Pid,
+        action: PlayerAction
+    ) -> None | GameState:
+        raise NotImplementedError
+
+    def waiting_for(self, game_state: GameState) -> None | Pid:
+        players = [game_state.get_player1(), game_state.get_player2()]
+        for player in players:
+            if player.get_phase().is_action_phase():
+                return game_state.get_pid(player)
+        return None
 
+    @abstractmethod
     def action_generator(self, game_state: GameState, pid: Pid) -> None | ActionGenerator:
-        raise Exception("Not Reached")
+        raise NotImplementedError
 
     def __eq__(self, other: object) -> bool:
-        return isinstance(other, GameEndPhase)
+        return type(self) is type(other)
 
     def __hash__(self) -> int:
-        return hash(self.__class__.__name__)
+        return hash(type(self))
+
+    def dict_str(self) -> dict | str:
+        return self.__class__.__name__
```

### Comparing `dgisim-0.2.dev2/dgisim/src/phase/default/roll_phase.py` & `dgisim-0.2.dev3/dgisim/src/phase/default/roll_phase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
-from dataclasses import replace
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from .. import phase as ph
 
 from ...action.action import DicesSelectAction, EndRoundAction, PlayerAction
 from ...action.action_generator import ActionGenerator
 from ...action.enums import ActionType
 from ...dices import ActualDices
-from ...element import Element
 from ...helper.quality_of_life import just
 from ...state.enums import Act, Pid
 
 if TYPE_CHECKING:
     from ...action.types import DecidedChoiceType, GivenChoiceType
     from ...state.game_state import GameState
 
@@ -20,27 +18,25 @@
     "RollPhase",
 ]
 
 
 class RollPhase(ph.Phase):
     _NUM_DICES = 8
 
-    def _get_all_omni_and_activate(self, game_state: GameState) -> GameState:
+    def _get_all_dices_and_activate(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player1(
             lambda p1: p1.factory()
             .phase(Act.ACTION_PHASE)
             .dice_reroll_chances(game_state.get_mode().dice_reroll_chances())
-            # .dices(ActualDices.from_all(RollPhase._NUM_DICES, Element.OMNI))
             .dices(ActualDices.from_random(RollPhase._NUM_DICES))
             .build()
         ).f_player2(
             lambda p2: p2.factory()
             .phase(Act.ACTION_PHASE)
             .dice_reroll_chances(game_state.get_mode().dice_reroll_chances())
-            # .dices(ActualDices.from_all(RollPhase._NUM_DICES, Element.OMNI))
             .dices(ActualDices.from_random(RollPhase._NUM_DICES))
             .build()
         ).build()
 
     def _to_action_phase(self, game_state: GameState) -> GameState:
         return game_state.factory().f_phase(
             lambda mode: mode.action_phase()
@@ -50,15 +46,15 @@
             lambda p2: p2.factory().phase(Act.PASSIVE_WAIT_PHASE).build()
         ).build()
 
     def step(self, game_state: GameState) -> GameState:
         p1 = game_state.get_player1()
         p2 = game_state.get_player2()
         if p1.get_phase().is_passive_wait_phase() and p2.get_phase().is_passive_wait_phase():
-            return self._get_all_omni_and_activate(game_state)
+            return self._get_all_dices_and_activate(game_state)
         elif p1.get_phase().is_end_phase() and p2.get_phase().is_end_phase():
             return self._to_action_phase(game_state)
         else:
             raise ValueError(f"Given game_state has undefined next state for"
                              + f"{self.__class__.__name__}:\n{game_state}")
 
     def _handle_dices_selection(
@@ -129,15 +125,15 @@
         pid = action_generator.pid
 
         if player_choice is ActionType.SELECT_DICES:
             from ...action.action_generator_generator import DicesSelectionActGenGenerator
             return just(DicesSelectionActGenGenerator.action_generator(game_state, pid))
         elif player_choice is ActionType.END_ROUND:
             return ActionGenerator(game_state=game_state, pid=pid, action=EndRoundAction())
-        else:
+        else:  # pragma: no cover
             action_type_name = ActionType.__name__
             if isinstance(player_choice, ActionType):
                 raise Exception(f"Unhandled player {action_type_name} {player_choice}")
             else:
                 raise TypeError(f"Unexpected player choice {player_choice} where"
                                 + f"where {action_type_name} is expected")
 
@@ -146,13 +142,7 @@
             return None
         return ActionGenerator(
             game_state=game_state,
             pid=pid,
             _choices_helper=self._choices_helper,
             _fill_helper=self._fill_helper,
         )
-
-    def __eq__(self, other: object) -> bool:
-        return isinstance(other, RollPhase)
-
-    def __hash__(self) -> int:
-        return hash(self.__class__.__name__)
```

### Comparing `dgisim-0.2.dev2/dgisim/src/player_agent.py` & `dgisim-0.2.dev3/dgisim/src/player_agent.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev2/dgisim/src/state/enums.py` & `dgisim-0.2.dev3/dgisim/src/state/enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return self is Pid.P2
 
     def other(self) -> Pid:
         if self is Pid.P1:
             return Pid.P2
         elif self is Pid.P2:
             return Pid.P1
-        else:
+        else:  # pragma: no cover
             raise Exception("Unknown situation of pid")
 
 
 class Act(Enum):
     ACTION_PHASE = "Action Phase"
     PASSIVE_WAIT_PHASE = "Passive Wait Phase"
     ACTIVE_WAIT_PHASE = "Aggressive Wait Phase"
```

### Comparing `dgisim-0.2.dev2/dgisim/src/state/player_state.py` & `dgisim-0.2.dev3/dgisim/src/state/player_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,27 +128,30 @@
             lambda dcs: dcs.hide_all()
         ).build()
 
     @classmethod
     def example_player(cls, mode: Mode) -> Self:
         cards = mode.all_cards()
         chars = mode.all_chars()
+        import random
+        selected_cards = random.sample(list(cards), k=15)
+        selected_chars = random.sample(list(chars), k=3)
         return cls(
             phase=Act.PASSIVE_WAIT_PHASE,
             card_redraw_chances=0,
             dice_reroll_chances=0,
             characters=Characters.from_default(
-                tuple([char.from_default(i + 1) for i, char in enumerate(chars)][:3])
+                tuple(char.from_default(i + 1) for i, char in enumerate(selected_chars))
             ),
             combat_statuses=sts.Statuses(()),
             summons=Summons((), mode.summons_limit()),
             supports=Supports((), mode.supports_limit()),
             dices=ActualDices({}),
             hand_cards=Cards({}),
-            deck_cards=Cards(dict([(card, mode.max_cards_per_kind()) for card in cards])),
+            deck_cards=Cards(dict([(card, mode.max_cards_per_kind()) for card in selected_cards])),
             publicly_used_cards=Cards({}),
             publicly_gained_cards=Cards({}),
         )
 
     @classmethod
     def from_deck(cls, mode: Mode, characters: Characters, cards: Cards) -> Self:
         return cls(
@@ -166,21 +169,24 @@
             publicly_gained_cards=Cards({}),
         )
 
     def _all_unique_data(self) -> tuple:
         return (
             self._phase,
             self._card_redraw_chances,
+            self._dice_reroll_chances,
             self._characters,
-            self._dices,
+            self._combat_statuses,
             self._summons,
             self._supports,
+            self._dices,
             self._hand_cards,
             self._deck_cards,
             self._publicly_used_cards,
+            self._publicly_gained_cards,
         )
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, PlayerState):
             return False
         return self._all_unique_data() == other._all_unique_data()
 
@@ -222,22 +228,22 @@
         self._phase = phase
         return self
 
     def card_redraw_chances(self, chances: int) -> PlayerStateFactory:
         self._card_redraw_chances = chances
         return self
 
-    def f_card_redraw_chances(self, f: Callable[[int], int]) -> PlayerStateFactory:
+    def f_card_redraw_chances(self, f: Callable[[int], int]) -> PlayerStateFactory:  # pragma: no cover
         return self.card_redraw_chances(f(self._card_redraw_chances))
 
     def dice_reroll_chances(self, chances: int) -> PlayerStateFactory:
         self._dice_reroll_chances = chances
         return self
 
-    def f_dice_reroll_chances(self, f: Callable[[int], int]) -> PlayerStateFactory:
+    def f_dice_reroll_chances(self, f: Callable[[int], int]) -> PlayerStateFactory:  # pragma: no cover
         return self.dice_reroll_chances(f(self._dice_reroll_chances))
 
     def characters(self, characters: Characters) -> PlayerStateFactory:
         self._characters = characters
         return self
 
     def f_characters(self, f: Callable[[Characters], Characters]) -> PlayerStateFactory:
```

### Comparing `dgisim-0.2.dev2/dgisim/src/status/enums.py` & `dgisim-0.2.dev3/dgisim/src/status/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from enum import Enum
 
 __all__ = [
     "Preprocessables",
+    "Informables",
 ]
 
 
 class Preprocessables(Enum):
     """ PreProcessType """
     # Swap
     SWAP = "Swap"                 # To determine if swap needs to cost more or less,
@@ -15,7 +16,12 @@
     SKILL = "Skill"               # same as SWAP but for skill
     # Card
     CARD = "Card"                 # same as SWAP but for card
     # Damages
     DMG_ELEMENT = "DmgElement"    # To determine the element
     DMG_REACTION = "DmgReaction"  # To determine the reaction
     DMG_AMOUNT = "DmgNumber"      # To determine final amount of damage
+
+class Informables(Enum):
+    DMG_DELT = "DmgDelt"
+    SKILL_USAGE = "SkillUsage"
+    CHARACTER_DEATH = "CharacterDeath"
```

### Comparing `dgisim-0.2.dev2/dgisim/src/status/status.py` & `dgisim-0.2.dev3/dgisim/src/status/status.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,46 +10,65 @@
 - template classes, starting with an '_', are templates for other classes
 - concrete classes, the implementation of statuses that are actually in the game
 """
 from __future__ import annotations
 from dataclasses import dataclass, replace
 from enum import Enum
 from math import ceil
-from typing import ClassVar, Optional, TYPE_CHECKING
+from typing import ClassVar, cast, Optional, TYPE_CHECKING
 from typing_extensions import override, Self
 
 from ..effect import effect as eft
 
-from ..character.enums import CharacterSkill
+from ..character.enums import CharacterSkill, WeaponType
 from ..effect.enums import Zone, TriggeringSignal, DynamicCharacterTarget
 from ..effect.structs import StaticTarget, DamageType
-from ..element import Element
-from ..event import EventSpeed, EventType, GameEvent
+from ..element import Element, Reaction
+from ..event import *
+from ..helper.hashable_dict import HashableDict
 from ..helper.quality_of_life import just, BIG_INT, case_val
-from .enums import Preprocessables
+from .enums import Preprocessables, Informables
 
 if TYPE_CHECKING:
     from ..card.card import Card
+    from ..character.character import Character
     from ..state.game_state import GameState
-    from .types import Preprocessable
 
 __all__ = [
     # base
     "Status",
 
     # type
-    "CharacterTalentStatus",  # it should be statuses used to record character-talent related data
+    "HiddenStatus",  # it should be statuses used to record character-talent related data
     "EquipmentStatus",  # talent / weapon / artifact
+    "TalentEquipmentStatus",
+    "WeaponEquipmentStatus",
+    "ArtifactEquipmentStatus",
     "CharacterStatus",  # statues that belongs to one character only
     "CombatStatus",  # statues that buffs the active character
 
     # templates
     "StackedShieldStatus",
     "FixedShieldStatus",
 
+    # hidden status
+    "PlungeAttackStatus",
+
+    # equipment status
+    ## bow ##
+    "RavenBowStatus",
+    ## catalyst ##
+    "MagicGuideStatus",
+    ## claymore ##
+    "WhiteIronGreatswordStatus",
+    ## polearm ##
+    "WhiteTasselStatus",
+    ## sword ##
+    "TravelersHandySwordStatus",
+
     # combat status
     "CatalyzingFieldStatus",
     "ChangingShiftsStatus",
     "CrystallizeStatus",
     "DendroCoreStatus",
     "FrozenStatus",
     "LeaveItToMeStatus",
@@ -59,43 +78,66 @@
     "LotusFlowerCrispStatus",
     "MintyMeatRollsStatus",
     "MushroomPizzaStatus",
     "NorthernSmokedChickenStatus",
     "SatiatedStatus",
 
     # character specific status
+    ## Arataki Itto ##
+    "AratakiIchibanStatus",
+    "RagingOniKing",
+    "SuperlativeSuperstrengthStatus",
+    ## Kaedehara Kazuha ##
+    "MidareRanzanStatus",
+    "MidareRanzanCryoStatus",
+    "MidareRanzanElectroStatus",
+    "MidareRanzanHydroStatus",
+    "MidareRanzanPyroStatus",
+    "PoeticsOfFuubutsuStatus",
+    "PoeticsOfFuubutsuCryoStatus",
+    "PoeticsOfFuubutsuElectroStatus",
+    "PoeticsOfFuubutsuHydroStatus",
+    "PoeticsOfFuubutsuPyroStatus",
     ## Kaeya ##
     "ColdBloodedStrikeStatus",
     "IcicleStatus",
     ## Keqing ##
     "KeqingElectroInfusionStatus",
     "KeqingTalentStatus",
     "ThunderingPenanceStatus",
+    ## Klee ##
+    "ExplosiveSparkStatus",
+    "PoundingSurpriseStatus",
+    "SparksnSplash",
     ## Rhodeia of Loch ##
     "StreamingSurgeStatus",
+    ## Tighnari ##
+    "KeenSightStatus",
+    "VijnanaSuffusionStatus",
 ]
 
 
 ############################## base ##############################
 @dataclass(frozen=True)
 class Status:
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset()
 
     def __init__(self) -> None:
         if type(self) is Status:  # pragma: no cover
             raise Exception("class Status is not instantiable")
 
     def preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         """
-        Returns the processed Preprocessable and possibly updated or deleted self
+        Returns the processed PreprocessableEvent and possibly updated or deleted self
         """
         new_item, new_self = self._preprocess(game_state, status_source, item, signal)
         return self._post_preprocess(
             game_state,
             status_source,
             item,
             signal,
@@ -103,44 +145,44 @@
             new_self,
         )
 
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         return item, self
 
     def _post_preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-            new_item: Preprocessable,
+            new_item: PreprocessableEvent,
             new_self: Optional[Self],
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         return (new_item, new_self)
 
     def inform(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            information: eft.SpecificDamageEffect | CharacterSkill | Card,
-            info_source: Optional[StaticTarget] = None,
+            info_type: Informables,
+            information: InformableEvent,
     ) -> GameState:
-        new_self = self._inform(game_state, status_source, information, info_source)
+        new_self = self._inform(game_state, status_source, info_type, information)
         if new_self == self:
             return game_state
 
         from ..summon import summon as sm
         from ..support import support as sp
-        if isinstance(new_self, CharacterTalentStatus) \
+        if isinstance(new_self, HiddenStatus) \
                 or isinstance(new_self, EquipmentStatus) \
                 or isinstance(new_self, CharacterStatus):
             return eft.OverrideCharacterStatusEffect(
                 target=status_source,
                 status=new_self,
             ).execute(game_state)
 
@@ -165,32 +207,29 @@
         else:
             raise NotImplementedError
 
     def _inform(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            information: eft.SpecificDamageEffect | CharacterSkill | Card,
-            info_source: Optional[StaticTarget],
+            info_type: Informables,
+            information: InformableEvent,
     ) -> Self:
         return self
 
-    # def react_to_event(self, game_state: gs.GameState, event: TriggerringEvent) -> gs.GameState:
-    #     raise Exception("TODO")
-
     def react_to_signal(
             self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> list[eft.Effect]:
-        es, new_status = self._react_to_signal(source, signal)
-        es, new_status = self._post_react_to_signal(es, new_status, signal)
+        es, new_status = self._react_to_signal(game_state, source, signal)
+        es, new_status = self._post_react_to_signal(es, new_status, source, signal)
 
         from ..summon import summon as sm
         from ..support import support as sp
         # do the removal or update of the status
-        if isinstance(self, CharacterTalentStatus) \
+        if isinstance(self, HiddenStatus) \
                 or isinstance(self, EquipmentStatus) \
                 or isinstance(self, CharacterStatus):
             if new_status is None:
                 es.append(eft.RemoveCharacterStatusEffect(
                     source,
                     type(self),
                 ))
@@ -271,32 +310,42 @@
 
         return es
 
     def _post_react_to_signal(
             self,
             effects: list[eft.Effect],
             new_status: Optional[Self],
+            source: StaticTarget,
             signal: TriggeringSignal,
     ) -> tuple[list[eft.Effect], Optional[Self]]:
-        if new_status != self:
-            return effects, new_status
-        return effects, self
+        if effects:
+            if any(isinstance(effect, eft.ReferredDamageEffect) for effect in effects):
+                effects.append(eft.AllStatusTriggererEffect(
+                    pid=source.pid,
+                    signal=TriggeringSignal.POST_DMG,
+                ))
+        return effects, case_val(new_status == self, self, new_status)
 
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         """
         Returns a tuple, containg the effects and how to update self
         * if the returned new self is the same object as myself, then it is taken as no change
           requested
         * if the returned new self is none, then it is taken as a removal request
         * if the returned new self is different object than myself, then it is taken as an update
         """
         return [], self
 
+    def _is_swapping_source(self, source: StaticTarget, signal: TriggeringSignal) -> bool:
+        """ Returns True if characters of the source player is swapping """
+        return source.pid.is_player1() and signal is TriggeringSignal.SWAP_EVENT_1 \
+            or source.pid.is_player2() and signal is TriggeringSignal.SWAP_EVENT_2
+
     def same_type_as(self, status: Status) -> bool:
         return type(self) == type(status)
 
     def update(self, other: Self) -> None | Self:
         new_self = self._update(other)
         return self._post_update(new_self)
 
@@ -308,29 +357,69 @@
 
     def __str__(self) -> str:
         return self.__class__.__name__.removesuffix("Status")  # pragma: no cover
 
 
 ############################## type ##############################
 @dataclass(frozen=True)
-class CharacterTalentStatus(Status):
+class HiddenStatus(Status):
     """
     Basic status, describing character talents
     """
     pass
 
 
 @dataclass(frozen=True)
 class EquipmentStatus(Status):
     """
     Basic status, describing weapon, artifact and character unique talents
     """
 
 
 @dataclass(frozen=True)
+class TalentEquipmentStatus(EquipmentStatus):
+    pass
+
+
+@dataclass(frozen=True)
+class WeaponEquipmentStatus(EquipmentStatus):
+    WEAPON_TYPE: ClassVar[WeaponType]
+    BASE_DAMAGE_BOOST: ClassVar[int] = 1
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        if signal is Preprocessables.DMG_AMOUNT:
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if (
+                dmg.source == status_source
+                and (
+                    dmg.damage_type.normal_attack
+                    or dmg.damage_type.elemental_skill
+                    or dmg.damage_type.elemental_burst
+                )
+                and dmg.element is not Element.PIERCING
+            ):
+                new_damage = replace(dmg, damage=dmg.damage + self.BASE_DAMAGE_BOOST)
+                return DmgPEvent(dmg=new_damage), self
+        return super()._preprocess(game_state, status_source, item, signal)
+
+
+@dataclass(frozen=True)
+class ArtifactEquipmentStatus(EquipmentStatus):
+    pass
+
+
+@dataclass(frozen=True)
 class CharacterStatus(Status):
     """
     Basic status, private status to each character
     """
     pass
 
 
@@ -353,19 +442,19 @@
         return True
 
     @override
     def _post_preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-            new_item: Preprocessable,
+            new_item: PreprocessableEvent,
             new_self: Optional[Self],
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if new_self is not None:
             if self._auto_destroy() and new_self.usages <= 0:
                 new_self = None
             elif new_self.usages < 0:
                 new_self = replace(new_self, usages=0)
         return super()._post_preprocess(game_state, status_source, item, signal, new_item, new_self)
 
@@ -378,32 +467,30 @@
             elif new_self.usages < 0:
                 new_self = replace(new_self, usages=0)
         return super()._post_update(new_self)
 
     @override
     def _update(self, other: Self) -> Optional[Self]:
         new_usages = min(self.usages + other.usages, self.MAX_USAGES)
-        return replace(self, usages=new_usages)
+        return replace(other, usages=new_usages)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True)
 class _ShieldStatus(Status):
     def _is_target(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
-            signal: Preprocessables,
+            item: eft.SpecificDamageEffect,
     ) -> bool:
         from ..summon import summon as sm
-        assert isinstance(item, eft.SpecificDamageEffect)
-        if isinstance(self, CharacterTalentStatus) \
+        if isinstance(self, HiddenStatus) \
                 or isinstance(self, EquipmentStatus) \
                 or isinstance(self, CharacterStatus):
             return item.target == status_source
 
         elif isinstance(self, CombatStatus):
             attached_active_character = StaticTarget(
                 status_source.pid,
@@ -435,26 +522,28 @@
         return True
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         cls = type(self)
         if signal is Preprocessables.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
-            if item.damage > 0 and self.usages > 0 \
-                    and item.element != Element.PIERCING \
-                    and self._is_target(game_state, status_source, item, signal) \
-                    and self._trigerring_condition(item):
-                new_dmg = max(0, item.damage - cls.SHIELD_AMOUNT)
-                new_item = replace(item, damage=new_dmg)
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if dmg.damage > 0 and self.usages > 0 \
+                    and dmg.element != Element.PIERCING \
+                    and self._is_target(game_state, status_source, dmg) \
+                    and self._trigerring_condition(dmg):
+                new_dmg_amount = max(0, dmg.damage - cls.SHIELD_AMOUNT)
+                new_dmg = replace(dmg, damage=new_dmg_amount)
+                new_item = DmgPEvent(dmg=new_dmg)
                 new_usages = self.usages - 1
                 if self._auto_destroy() and new_usages == 0:
                     return new_item, None
                 else:
                     return new_item, replace(self, usages=new_usages)
 
         return super()._preprocess(game_state, status_source, item, signal)
@@ -468,63 +557,69 @@
     SHIELD_AMOUNT: ClassVar[int] = 1  # shield amount per usage
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         cls = type(self)
         if signal is Preprocessables.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
             assert self.usages <= type(self).MAX_USAGES
-            if item.damage > 0 and self.usages > 0 \
-                    and item.element != Element.PIERCING \
-                    and self._is_target(game_state, status_source, item, signal):
-                usages_consumed = min(ceil(item.damage / cls.SHIELD_AMOUNT), self.usages)
-                new_dmg = max(0, item.damage - usages_consumed * cls.SHIELD_AMOUNT)
-                new_item = replace(item, damage=new_dmg)
+            if dmg.damage > 0 and self.usages > 0 \
+                    and dmg.element != Element.PIERCING \
+                    and self._is_target(game_state, status_source, dmg):
+                usages_consumed = min(ceil(dmg.damage / cls.SHIELD_AMOUNT), self.usages)
+                new_dmg_amount = max(0, dmg.damage - usages_consumed * cls.SHIELD_AMOUNT)
+                new_dmg = replace(dmg, damage=new_dmg_amount)
+                new_item = DmgPEvent(dmg=new_dmg)
                 new_usages = self.usages - usages_consumed
                 if new_usages == 0:
                     return new_item, None
                 else:
                     return new_item, replace(self, usages=new_usages)
 
         return super()._preprocess(game_state, status_source, item, signal)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True, kw_only=True)
-class _InfusionStatus(CharacterStatus, _UsageStatus):
+class _InfusionStatus(_UsageStatus):
     MAX_USAGES: ClassVar[int] = BIG_INT
-    ELEMENT: ClassVar[Optional[Element]] = None
+    ELEMENT: ClassVar[Element]
     damage_boost: int = 0
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
-        assert self.ELEMENT is not None
-        new_item: Optional[eft.SpecificDamageEffect] = None
-        if isinstance(item, eft.SpecificDamageEffect):
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        new_item: Optional[DmgPEvent] = None
+        if isinstance(item, DmgPEvent):
+            dmg = item.dmg
             if signal is Preprocessables.DMG_ELEMENT:
-                if self._dmg_element_condition(game_state, status_source, item):
-                    new_item = replace(item, element=self.ELEMENT)
+                if self._dmg_element_condition(game_state, status_source, dmg):
+                    new_item = replace(item, dmg=replace(dmg, element=self.ELEMENT))
             if signal is Preprocessables.DMG_AMOUNT:
                 if self.damage_boost != 0  \
-                        and self._dmg_boost_condition(game_state, status_source, item):
-                    new_item = replace(item, damage=item.damage + self.damage_boost)
+                        and self._dmg_boost_condition(game_state, status_source, dmg):
+                    new_item = replace(item, dmg=replace(
+                        dmg, damage=dmg.damage + self.damage_boost))
         if new_item is not None:
             return new_item, self
         else:
             return item, self
 
     def _dmg_element_condition(
             self,
@@ -543,56 +638,142 @@
             status_source: StaticTarget,
             item: eft.SpecificDamageEffect,
     ) -> bool:
         return item.element is self.ELEMENT and status_source == item.source
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         d_usages = 0
         if signal is TriggeringSignal.ROUND_END:
             d_usages = -1
         return [], replace(self, usages=d_usages)
 
 
+############################## Hidden Status ##############################
+
+
+@dataclass(frozen=True, kw_only=True)
+class PlungeAttackStatus(HiddenStatus):
+    can_plunge: bool = False
+    invalidate: bool = False
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+        TriggeringSignal.ROUND_END,
+        TriggeringSignal.SWAP_EVENT_1,
+        TriggeringSignal.SWAP_EVENT_2,
+    ))
+
+    @override
+    def _inform(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
+        if info_type is Informables.SKILL_USAGE:
+            assert isinstance(information, SkillIEvent)
+            if information.source == status_source \
+                    and self.can_plunge:
+                return replace(self, invalidate=True)
+        return self
+
+    @override
+    def _react_to_signal(
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
+    ) -> tuple[list[eft.Effect], None | Self]:
+        if signal is TriggeringSignal.COMBAT_ACTION and self.invalidate:
+            return [], replace(self, can_plunge=False, invalidate=False)
+        elif signal is TriggeringSignal.ROUND_END and self.can_plunge:
+            assert not self.invalidate
+            return [], replace(self, can_plunge=False)
+        elif self._is_swapping_source(source, signal):
+            characters = game_state.get_player(source.pid).get_characters()
+            active_char_id = characters.get_active_character_id()
+            if source.id == active_char_id and not self.can_plunge:
+                return [], replace(self, can_plunge=True)
+        return [], self
+
+    @override
+    def __str__(self) -> str:
+        return super().__str__() + f"({case_val(self.can_plunge, '*', '')})"
+
+############################## Equipment Status ##############################
+
+########## Weapon Status ##########
+
+#### Bow ####
+
+
 @dataclass(frozen=True, kw_only=True)
-class ElectroInfusionStatus(_InfusionStatus):
-    ELEMENT: ClassVar[Optional[Element]] = Element.ELECTRO
+class RavenBowStatus(WeaponEquipmentStatus):
+    WEAPON_TYPE: ClassVar[WeaponType] = WeaponType.BOW
+
+#### Catalyst ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class MagicGuideStatus(WeaponEquipmentStatus):
+    WEAPON_TYPE: ClassVar[WeaponType] = WeaponType.CATALYST
+
+#### Claymore ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class WhiteIronGreatswordStatus(WeaponEquipmentStatus):
+    WEAPON_TYPE: ClassVar[WeaponType] = WeaponType.CLAYMORE
+
+#### Polearm ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class WhiteTasselStatus(WeaponEquipmentStatus):
+    WEAPON_TYPE: ClassVar[WeaponType] = WeaponType.POLEARM
+
+#### Sword ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class TravelersHandySwordStatus(WeaponEquipmentStatus):
+    WEAPON_TYPE: ClassVar[WeaponType] = WeaponType.SWORD
 
 ############################## Combat Status ##############################
 
 
 @dataclass(frozen=True)
 class CatalyzingFieldStatus(CombatStatus):
     damage_boost: ClassVar[int] = 1
     usages: int = 2
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[CatalyzingFieldStatus]]:
+    ) -> tuple[PreprocessableEvent, Optional[CatalyzingFieldStatus]]:
         if signal is Preprocessables.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
+            assert isinstance(item, eft.DmgPEvent)
+            dmg = item.dmg
             assert self.usages >= 1
-            elem_can_boost = item.element is Element.ELECTRO or item.element is Element.DENDRO
-            legal_to_boost = status_source.pid is item.source.pid
-            target_is_active = item.target.id == game_state.get_player(
-                item.target.pid
+            elem_can_boost = dmg.element is Element.ELECTRO or dmg.element is Element.DENDRO
+            legal_to_boost = status_source.pid is dmg.source.pid
+            target_is_active = dmg.target.id == game_state.get_player(
+                dmg.target.pid
             ).just_get_active_character().get_id()
             if elem_can_boost and legal_to_boost and target_is_active:
-                new_damage = replace(item, damage=item.damage + CatalyzingFieldStatus.damage_boost)
+                new_damage = replace(dmg, damage=dmg.damage + CatalyzingFieldStatus.damage_boost)
+                new_item = DmgPEvent(dmg=new_damage)
                 if self.usages == 1:
-                    return new_damage, None
+                    return new_item, None
                 else:
-                    return new_damage, CatalyzingFieldStatus(self.usages - 1)
+                    return new_item, CatalyzingFieldStatus(self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True)
@@ -600,20 +781,20 @@
     COST_DEDUCTION: ClassVar[int] = 1
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if signal is Preprocessables.SWAP:
-            assert isinstance(item, GameEvent) and item.event_type is EventType.SWAP
-            if item.target.pid is status_source.pid \
+            assert isinstance(item, ActionPEvent) and item.event_type is EventType.SWAP
+            if item.source.pid is status_source.pid \
                     and item.dices_cost.num_dices() >= self.COST_DEDUCTION:
                 assert item.dices_cost.num_dices() == item.dices_cost[Element.ANY]
                 new_cost = (item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
                 return replace(item, dices_cost=new_cost), None
         return super()._preprocess(game_state, status_source, item, signal)
 
 
@@ -641,185 +822,209 @@
     usages: int = 1
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[DendroCoreStatus]]:
+    ) -> tuple[PreprocessableEvent, Optional[DendroCoreStatus]]:
         if signal is Preprocessables.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
             assert self.usages >= 1
-            elem_can_boost = item.element is Element.ELECTRO or item.element is Element.PYRO
-            legal_to_boost = status_source.pid is item.source.pid
-            target_is_active = item.target.id == game_state.get_player(
-                item.target.pid
+            elem_can_boost = dmg.element is Element.ELECTRO or dmg.element is Element.PYRO
+            legal_to_boost = status_source.pid is dmg.source.pid
+            target_is_active = dmg.target.id == game_state.get_player(
+                dmg.target.pid
             ).just_get_active_character().get_id()
             if elem_can_boost and legal_to_boost and target_is_active:
-                new_damage = replace(item, damage=item.damage + DendroCoreStatus.damage_boost)
+                new_damage = replace(dmg, damage=dmg.damage + DendroCoreStatus.damage_boost)
+                new_item = DmgPEvent(dmg=new_damage)
                 if self.usages == 1:
-                    return new_damage, None
+                    return new_item, None
                 else:
-                    return new_damage, DendroCoreStatus(self.usages - 1)
+                    return new_item, DendroCoreStatus(self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
 
     # @override
     # def update(self, other: DendroCoreStatus) -> DendroCoreStatus:
     #     total_count = min(self.count + other.count, 2)
     #     return DendroCoreStatus(total_count)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True)
 class FrozenStatus(CharacterStatus):
     damage_boost: ClassVar[int] = 2
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if signal is Preprocessables.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
-            can_reaction = item.element is Element.PYRO or item.element is Element.PHYSICAL
-            is_damage_target = item.target == status_source
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            can_reaction = dmg.element is Element.PYRO or dmg.element is Element.PHYSICAL
+            is_damage_target = dmg.target == status_source
             if is_damage_target and can_reaction:
-                return replace(item, damage=item.damage + FrozenStatus.damage_boost), None
+                return (
+                    DmgPEvent(dmg=replace(dmg, damage=dmg.damage + FrozenStatus.damage_boost)),
+                    None
+                )
         return super()._preprocess(game_state, status_source, item, signal)
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[FrozenStatus]]:
         if signal is TriggeringSignal.ROUND_END:
             return [], None
         return [], self
 
 
 @dataclass(frozen=True)
 class LeaveItToMeStatus(CombatStatus):
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if signal is Preprocessables.SWAP:
-            assert isinstance(item, GameEvent) and item.event_type is EventType.SWAP
-            if item.target.pid is status_source.pid \
+            assert isinstance(item, ActionPEvent) and item.event_type is EventType.SWAP
+            if item.source.pid is status_source.pid \
                     and item.event_speed is EventSpeed.COMBAT_ACTION:
                 return replace(item, event_speed=EventSpeed.FAST_ACTION), None
         return super()._preprocess(game_state, status_source, item, signal)
 
 
 ############################## Character Status ##############################
 
 
 @dataclass(frozen=True)
 class JueyunGuobaStatus(CharacterStatus, _UsageStatus):
     usages: int = 1
     MAX_USAGES: ClassVar[int] = 1
     damage_boost: ClassVar[int] = 1
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if signal is Preprocessables.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
-            if item.source == status_source and item.damage_type.normal_attack:
-                item = replace(item, damage=item.damage + JueyunGuobaStatus.damage_boost)
-                return item, replace(self, usages=self.usages - 1)
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if dmg.source == status_source and dmg.damage_type.normal_attack:
+                dmg = replace(dmg, damage=dmg.damage + JueyunGuobaStatus.damage_boost)
+                return DmgPEvent(dmg=dmg), replace(self, usages=self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         d_usages = 0
         if signal is TriggeringSignal.ROUND_END:
             d_usages = -1
         return [], replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
 class LotusFlowerCrispStatus(CharacterStatus, FixedShieldStatus):
     usages: int = 1
     MAX_USAGES: ClassVar[int] = 1
     SHIELD_AMOUNT: ClassVar[int] = 3
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _react_to_signal(
             self,
+            game_state: GameState,
             source: StaticTarget,
             signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         d_usages = 0
         if signal is TriggeringSignal.ROUND_END:
             d_usages = -BIG_INT
         return [], replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
 class MintyMeatRollsStatus(CharacterStatus, _UsageStatus):
     usages: int = 3
     MAX_USAGES: ClassVar[int] = 3
     COST_DEDUCTION: ClassVar[int] = 1
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if signal is Preprocessables.SKILL:
-            assert isinstance(item, GameEvent)
-            if status_source == item.target \
+            assert isinstance(item, ActionPEvent)
+            if status_source == item.source \
                     and item.event_type is EventType.NORMAL_ATTACK \
                     and item.dices_cost[Element.ANY] >= self.COST_DEDUCTION:
                 item = replace(
                     item,
                     dices_cost=(item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
                 )
                 return item, replace(self, usages=self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         d_usages = 0
         if signal is TriggeringSignal.ROUND_END:
             d_usages = -BIG_INT
         return [], replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
 class MushroomPizzaStatus(CharacterStatus, _UsageStatus):
     usages: int = 2
     MAX_USAGES: ClassVar[int] = 2
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.END_ROUND_CHECK_OUT,
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         es: list[eft.Effect] = []
         d_usages = 0
         if signal is TriggeringSignal.END_ROUND_CHECK_OUT:
             es.append(
                 eft.RecoverHPEffect(
                     source,
@@ -833,122 +1038,444 @@
 
 
 @dataclass(frozen=True)
 class NorthernSmokedChickenStatus(CharacterStatus, _UsageStatus):
     usages: int = 1
     MAX_USAGES: ClassVar[int] = 1
     COST_DEDUCTION: ClassVar[int] = 1
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, Optional[Self]]:
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
         if signal is Preprocessables.SKILL:
-            assert isinstance(item, GameEvent)
-            if status_source == item.target \
+            assert isinstance(item, ActionPEvent)
+            if status_source == item.source \
                     and item.event_type is EventType.NORMAL_ATTACK \
                     and item.dices_cost[Element.ANY] >= self.COST_DEDUCTION:
                 item = replace(
                     item,
                     dices_cost=(item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
                 )
                 return item, replace(self, usages=self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         d_usages = 0
         if signal is TriggeringSignal.ROUND_END:
             d_usages = -BIG_INT
         return [], replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
 class SatiatedStatus(CharacterStatus):
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         if signal is TriggeringSignal.ROUND_END:
             return [], None
         return [], self
 
 
 ############################## Character Specific Status ##############################
 """
 Group statues by characters, characters ordered alphabetically
 """
 
+#### Arataki Itto ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class AratakiIchibanStatus(TalentEquipmentStatus, _UsageStatus):
+    usages: int = 0  # here means num of normal attacks in the past
+    ACTIVATION_THRESHOLD: ClassVar[int] = 2
+    DAMAGE_BOOST: ClassVar[int] = 1
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
+
+    @staticmethod
+    def _auto_destroy() -> bool:
+        return False
+
+    def activated(self) -> bool:
+        return self.usages + 1 >= self.ACTIVATION_THRESHOLD
+
+    @property
+    def dmg_boost(self) -> int:
+        return self.DAMAGE_BOOST
+
+    @override
+    def _inform(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
+        if self.activated() \
+                or info_type is not Informables.SKILL_USAGE:
+            return self
+
+        assert isinstance(information, SkillIEvent)
+        if status_source != information.source \
+                or information.skill_type != CharacterSkill.NORMAL_ATTACK:
+            return self
+
+        return replace(self, usages=self.usages+1)
+
+    @override
+    def _react_to_signal(
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
+    ) -> tuple[list[eft.Effect], None | Self]:
+        if signal is TriggeringSignal.ROUND_END:
+            return [], replace(self, usages=-self.usages)
+        return [], self
+
+
+@dataclass(frozen=True, kw_only=True)
+class RagingOniKing(CharacterStatus, _InfusionStatus):
+    usages: int = 2  # duration
+    ELEMENT: ClassVar[Element] = Element.GEO
+    damage_boost: int = 2
+    status_gaining_usages: int = 1
+    status_gaining_available: bool = False
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+        TriggeringSignal.ROUND_END,
+    ))
+
+    @override
+    def _inform(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
+        if info_type is Informables.SKILL_USAGE:
+            assert isinstance(information, SkillIEvent)
+            if information.source == status_source \
+                    and information.skill_type is CharacterSkill.NORMAL_ATTACK \
+                    and not self.status_gaining_available:
+                return replace(self, status_gaining_available=True)
+        return self
+
+    @override
+    def _react_to_signal(
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
+    ) -> tuple[list[eft.Effect], None | Self]:
+        if signal is TriggeringSignal.ROUND_END:
+            return [], replace(self, usages=-1)
+        elif signal is TriggeringSignal.COMBAT_ACTION:
+            if self.status_gaining_available:
+                return [
+                    eft.AddCharacterStatusEffect(
+                        target=source,
+                        status=SuperlativeSuperstrengthStatus,
+                    ),
+                ], replace(self, usages=0, status_gaining_usages=0, status_gaining_available=False)
+        return [], self
+
+
+@dataclass(frozen=True, kw_only=True)
+class SuperlativeSuperstrengthStatus(CharacterStatus, _UsageStatus):
+    usages: int = 1
+    MAX_USAGES: ClassVar[int] = 3
+    DAMAGE_BOOST: ClassVar[int] = 1
+    TALENT_DAMAGE_BOOST: ClassVar[int] = 1
+    COST_DEDUCTION: ClassVar[int] = 1
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        if signal is Preprocessables.DMG_AMOUNT:
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if status_source != dmg.source:
+                return item, self
+            if dmg.damage_type.charged_attack:
+                character = game_state.get_character_target(status_source)
+                assert character is not None, f"source {status_source} in {game_state}"
+                dmg_boost = self.DAMAGE_BOOST
+                if character.talent_equiped():
+                    talent = character.get_equipment_statuses().just_find(AratakiIchibanStatus)
+                    if talent.activated():
+                        dmg_boost += talent.dmg_boost
+                new_item = DmgPEvent(dmg=replace(dmg, damage=dmg.damage + dmg_boost))
+                new_self = replace(self, usages=self.usages - 1)
+                return new_item, new_self
+        elif signal is Preprocessables.SKILL:
+            assert isinstance(item, ActionPEvent)
+            player = game_state.get_player(status_source.pid)
+            if (
+                    self.usages >= 2
+                    and status_source == item.source
+                    and item.event_type is EventType.NORMAL_ATTACK
+                    and player.get_dices().is_even()
+                    and item.dices_cost[Element.ANY] > 0
+            ):
+                item = replace(
+                    item,
+                    dices_cost=(item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
+                )
+                return item, self
+        return item, self
+
+#### Kaedehara Kazuha ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class MidareRanzanStatus(CharacterStatus):
+    _protected: bool = True
+    _needs_removal: bool = False
+    _ELEMENT: ClassVar[Element] = Element.ANEMO
+    _DMG_BOOST: ClassVar[int] = 1
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+    ))
+
+    @override
+    def _inform(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
+        if info_type is Informables.SKILL_USAGE:
+            assert isinstance(information, SkillIEvent)
+            if information.source == status_source \
+                    and not self._protected \
+                    and not self._needs_removal:
+                return replace(self, _needs_removal=True)
+        return self
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        if isinstance(item, DmgPEvent):
+            dmg = item.dmg
+            if status_source != dmg.source:
+                return item, self
+
+            if signal is Preprocessables.DMG_ELEMENT:
+                if dmg.damage_type.plunge_attack:
+                    new_item = DmgPEvent(dmg=replace(dmg, element=self._ELEMENT))
+                    return new_item, self
+            elif signal is Preprocessables.DMG_AMOUNT:
+                if dmg.damage_type.plunge_attack:
+                    new_item = DmgPEvent(dmg=replace(dmg, damage=dmg.damage + self._DMG_BOOST))
+                    return new_item, None
+        return item, self
+
+    @override
+    def _react_to_signal(
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
+    ) -> tuple[list[eft.Effect], None | Self]:
+        if signal is TriggeringSignal.COMBAT_ACTION:
+            if self._protected:
+                return [], replace(self, _protected=False)
+            elif self._needs_removal:
+                return [], None
+        return [], self
+
+    def __str__(self) -> str:
+        return super().__str__() + f"({self._protected}, {self._needs_removal})"
+
+
+@dataclass(frozen=True, kw_only=True)
+class MidareRanzanCryoStatus(MidareRanzanStatus):
+    _ELEMENT: ClassVar[Element] = Element.CRYO
+
+
+@dataclass(frozen=True, kw_only=True)
+class MidareRanzanElectroStatus(MidareRanzanStatus):
+    _ELEMENT: ClassVar[Element] = Element.ELECTRO
+
+
+@dataclass(frozen=True, kw_only=True)
+class MidareRanzanHydroStatus(MidareRanzanStatus):
+    _ELEMENT: ClassVar[Element] = Element.HYDRO
+
+
+@dataclass(frozen=True, kw_only=True)
+class MidareRanzanPyroStatus(MidareRanzanStatus):
+    _ELEMENT: ClassVar[Element] = Element.PYRO
+
+
+_MIDARE_RANZAN_MAP: dict[Element, type[MidareRanzanStatus]] = HashableDict({
+    Element.ANEMO: MidareRanzanStatus,
+    Element.CRYO: MidareRanzanCryoStatus,
+    Element.ELECTRO: MidareRanzanElectroStatus,
+    Element.HYDRO: MidareRanzanHydroStatus,
+    Element.PYRO: MidareRanzanPyroStatus,
+})
+
+
+@dataclass(frozen=True, kw_only=True)
+class PoeticsOfFuubutsuStatus(TalentEquipmentStatus):
+    pass
+
+
+@dataclass(frozen=True, kw_only=True)
+class _PoeticsOfFuubutsuElementStatus(CombatStatus, _UsageStatus):
+    usages: int = 2
+    MAX_USAGES: ClassVar[int] = 2
+    _ELEM: Element
+    _DMG_BOOST: ClassVar[int] = 1
+    _BOOSTABLE_ELEMS: ClassVar[frozenset[Element]] = Reaction.SWIRL.value.reaction_elems[0]
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        if signal is Preprocessables.DMG_AMOUNT:
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if (
+                    status_source.pid != dmg.source.pid
+                    or not (
+                        dmg.damage_type.from_character()
+                        or dmg.damage_type.from_summon()
+                    )
+                    or dmg.element is not self._ELEM
+            ):
+                return item, self
+
+            assert self.usages > 0
+            new_item = DmgPEvent(dmg=replace(dmg, damage=dmg.damage + self._DMG_BOOST))
+            return new_item, replace(self, usages=self.usages - 1)
+        return item, self
+
+
+@dataclass(frozen=True, kw_only=True)
+class PoeticsOfFuubutsuCryoStatus(_PoeticsOfFuubutsuElementStatus):
+    _ELEM: Element = Element.CRYO
+
+
+@dataclass(frozen=True, kw_only=True)
+class PoeticsOfFuubutsuElectroStatus(_PoeticsOfFuubutsuElementStatus):
+    _ELEM: Element = Element.ELECTRO
+
+
+@dataclass(frozen=True, kw_only=True)
+class PoeticsOfFuubutsuHydroStatus(_PoeticsOfFuubutsuElementStatus):
+    _ELEM: Element = Element.HYDRO
+
+
+@dataclass(frozen=True, kw_only=True)
+class PoeticsOfFuubutsuPyroStatus(_PoeticsOfFuubutsuElementStatus):
+    _ELEM: Element = Element.PYRO
+
+
+_POETICS_OF_FUUBUTSU_MAP: dict[Element, type[_PoeticsOfFuubutsuElementStatus]] = HashableDict({
+    Element.CRYO: PoeticsOfFuubutsuCryoStatus,
+    Element.ELECTRO: PoeticsOfFuubutsuElectroStatus,
+    Element.HYDRO: PoeticsOfFuubutsuHydroStatus,
+    Element.PYRO: PoeticsOfFuubutsuPyroStatus,
+})
 
 #### Kaeya ####
 
 
 @dataclass(frozen=True, kw_only=True)
 class IcicleStatus(CombatStatus, _UsageStatus):
     usages: int = 3
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.SWAP_EVENT_1,
+        TriggeringSignal.SWAP_EVENT_2,
+    ))
 
     def _react_to_signal(
             self,
+            game_state: GameState,
             source: StaticTarget,
             signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[IcicleStatus]]:
-        if source.pid.is_player1() and signal is TriggeringSignal.SWAP_EVENT_1 \
-                or source.pid.is_player2() and signal is TriggeringSignal.SWAP_EVENT_2:
+        if self._is_swapping_source(source, signal):
             effects: list[eft.Effect] = [
                 eft.ReferredDamageEffect(
                     source=source,
                     target=DynamicCharacterTarget.OPPO_ACTIVE,
                     element=Element.CRYO,
                     damage=2,
                     damage_type=DamageType(status=True),
                 ),
             ]
             return effects, replace(self, usages=-1)
         return [], self
 
 
 @dataclass(frozen=True, kw_only=True)
-class ColdBloodedStrikeStatus(EquipmentStatus):
+class ColdBloodedStrikeStatus(TalentEquipmentStatus):
     """
     Equipping this status implies the equipped character is Kaeya
     """
     usages: int = 1
     activated: bool = False
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _inform(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            information: eft.SpecificDamageEffect | CharacterSkill | Card,
-            info_source: Optional[StaticTarget],
-    ) -> ColdBloodedStrikeStatus:
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
         if self.activated or self.usages == 0:
             return self
 
-        if not isinstance(information, CharacterSkill):
+        if info_type is not Informables.SKILL_USAGE:
             return self
 
-        assert info_source != None
-        if status_source != info_source \
-                or information != CharacterSkill.ELEMENTAL_SKILL1:
+        assert isinstance(information, SkillIEvent)
+        if status_source != information.source \
+                or information.skill_type != CharacterSkill.ELEMENTAL_SKILL1:
             return self
 
         return replace(self, activated=True)
 
     @override
     def _react_to_signal(
             self,
+            game_state: GameState,
             source: StaticTarget,
             signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[ColdBloodedStrikeStatus]]:
         es: list[eft.Effect] = []
         new_self = self
 
         if signal is TriggeringSignal.COMBAT_ACTION and self.activated:
@@ -969,41 +1496,276 @@
     def __str__(self) -> str:
         return super().__str__() + case_val(self.activated, "(*)", '')
 
 #### Keqing ####
 
 
 @dataclass(frozen=True, kw_only=True)
-class KeqingTalentStatus(CharacterTalentStatus):
+class KeqingTalentStatus(HiddenStatus):
     can_infuse: bool
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+    ))
 
     def _react_to_signal(
             self,
+            game_state: GameState,
             source: StaticTarget,
             signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], Optional[KeqingTalentStatus]]:
         if signal is TriggeringSignal.COMBAT_ACTION:
             return [], type(self)(can_infuse=False)
         return [], self
 
     def __str__(self) -> str:
         return super().__str__() + f"({case_val(self.can_infuse, 1, 0)})"  # pragma: no cover
 
 
 @dataclass(frozen=True, kw_only=True)
-class ThunderingPenanceStatus(EquipmentStatus):
+class ThunderingPenanceStatus(TalentEquipmentStatus):
     pass
 
 
 @dataclass(frozen=True, kw_only=True)
-class KeqingElectroInfusionStatus(ElectroInfusionStatus):
-    pass
+class KeqingElectroInfusionStatus(CharacterStatus, _InfusionStatus):
+    ELEMENT: ClassVar[Element] = Element.ELECTRO
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.damage_boost})"
 
+#### Klee ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class ExplosiveSparkStatus(CharacterStatus, _UsageStatus):
+    usages: int = 1
+    MAX_USAGES: ClassVar[int] = 2
+    DAMAGE_BOOST: ClassVar[int] = 1
+    COST_DEDUCTION: ClassVar[int] = 1
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        if signal is Preprocessables.DMG_AMOUNT:
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if status_source != dmg.source:
+                return item, self
+            if dmg.damage_type.charged_attack:
+                new_item = DmgPEvent(dmg=replace(dmg, damage=dmg.damage + self.DAMAGE_BOOST))
+                new_self = replace(self, usages=self.usages - 1)
+                return new_item, new_self
+        elif signal is Preprocessables.SKILL:
+            assert isinstance(item, ActionPEvent)
+            player = game_state.get_player(status_source.pid)
+            if (
+                    status_source == item.source
+                    and item.event_type is EventType.NORMAL_ATTACK
+                    and player.get_dices().is_even()
+                    and item.dices_cost[Element.ANY] + item.dices_cost[Element.PYRO] > 0
+            ):
+                elems = [Element.PYRO, Element.ANY]
+                cost_deduction_left = self.COST_DEDUCTION
+                deduction: dict[Element, int] = {}
+                for elem in elems:
+                    deduction[elem] = cost_deduction_left
+                    cost_deduction_left -= item.dices_cost[elem]
+                    if cost_deduction_left <= 0:
+                        break
+                if item.dices_cost[Element.PYRO] > 0:
+                    item = replace(
+                        item,
+                        dices_cost=(item.dices_cost - deduction).validify()
+                    )
+                return item, self
+        return item, self
+
+
+@dataclass(frozen=True, kw_only=True)
+class PoundingSurpriseStatus(TalentEquipmentStatus):
+    pass
+
+
+@dataclass(frozen=True, kw_only=True)
+class SparksnSplash(CombatStatus, _UsageStatus):
+    usages: int = 2
+    activated: bool = False
+    MAX_USAGES: ClassVar[int] = 2
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+    ))
+
+    @override
+    def _inform(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
+        if self.activated or self.usages == 0:
+            return self
+
+        if info_type is not Informables.SKILL_USAGE:
+            return self
+
+        assert isinstance(information, SkillIEvent), information
+        if status_source.pid is not information.source.pid:
+            return self
+
+        return replace(self, activated=True)
+
+    @override
+    def _react_to_signal(
+            self,
+            game_state: GameState,
+            source: StaticTarget,
+            signal: TriggeringSignal
+    ) -> tuple[list[eft.Effect], Optional[Self]]:
+        es: list[eft.Effect] = []
+        new_self = self
+
+        if signal is TriggeringSignal.COMBAT_ACTION and self.activated:
+            assert self.usages >= 1
+            es.append(
+                eft.ReferredDamageEffect(
+                    source=source,
+                    target=DynamicCharacterTarget.SELF_SELF,
+                    element=Element.PYRO,
+                    damage=2,
+                    damage_type=DamageType(status=True, no_boost=True)
+                )
+            )
+            new_self = replace(new_self, usages=-1, activated=False)
+
+        return es, new_self
 
 #### Rhodeia of Loch ####
 
+
 @dataclass(frozen=True, kw_only=True)
-class StreamingSurgeStatus(EquipmentStatus):
+class StreamingSurgeStatus(TalentEquipmentStatus):
     pass
+
+#### Tighnari ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class KeenSightStatus(TalentEquipmentStatus):
+    COST_DEDUCTION: ClassVar[int] = 1
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        if signal is Preprocessables.SKILL:
+            assert isinstance(item, ActionPEvent)
+            player = game_state.get_player(status_source.pid)
+            characters = player.get_characters()
+            if (
+                    status_source == item.source
+                    and item.event_type is EventType.NORMAL_ATTACK
+                    and player.get_dices().is_even()
+                    and characters.just_get_character(
+                        cast(int, status_source.id)
+                    ).get_character_statuses().contains(VijnanaSuffusionStatus)
+                    and item.dices_cost[Element.ANY] > 0
+            ):
+                item = replace(
+                    item,
+                    dices_cost=(item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
+                )
+                return item, self
+        return super()._preprocess(game_state, status_source, item, signal)
+
+
+@dataclass(frozen=True, kw_only=True)
+class VijnanaSuffusionStatus(CharacterStatus, _UsageStatus):
+    usages: int = 2
+    activated: bool = False
+    MAX_USAGES: ClassVar[int] = 2
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.COMBAT_ACTION,
+    ))
+
+    @override
+    def _inform(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            info_type: Informables,
+            information: InformableEvent,
+    ) -> Self:
+        if (
+                self.activated
+                or self.usages == 0
+                or not isinstance(information, DmgIEvent)
+                or status_source != information.dmg.source
+                or not information.dmg.damage_type.charged_attack
+        ):
+            return self
+
+        return replace(self, activated=True)
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: PreprocessableEvent,
+            signal: Preprocessables,
+    ) -> tuple[PreprocessableEvent, Optional[Self]]:
+        new_item: None | DmgPEvent = None
+        if signal is Preprocessables.DMG_ELEMENT:
+            assert isinstance(item, DmgPEvent)
+            dmg = item.dmg
+            if status_source != dmg.source:
+                return item, self
+            if dmg.damage_type.charged_attack:
+                new_item = DmgPEvent(dmg=replace(dmg, element=Element.DENDRO))
+        if new_item is not None:
+            return new_item, self
+        else:
+            return item, self
+
+    @override
+    def _react_to_signal(
+            self,
+            game_state: GameState,
+            source: StaticTarget,
+            signal: TriggeringSignal
+    ) -> tuple[list[eft.Effect], Optional[Self]]:
+        es: list[eft.Effect] = []
+        new_self = self
+
+        if signal is TriggeringSignal.COMBAT_ACTION and self.activated:
+            from ..summon.summon import ClusterbloomArrowSummon
+            assert self.usages >= 1
+            es.append(
+                eft.AddSummonEffect(
+                    target_pid=source.pid,
+                    summon=ClusterbloomArrowSummon,
+                )
+            )
+            new_self = replace(new_self, usages=-1, activated=False)
+
+        return es, new_self
+
+    @override
+    def _update(self, other: Self) -> None | Self:
+        new_usages = min(self.usages + other.usages, self.MAX_USAGES)
+        return type(self)(
+            usages=new_usages,
+            activated=other.activated,
+        )
+
+    def __str__(self) -> str:
+        return super().__str__() + f"({self.usages}{case_val(self.activated, '*', '')})"
```

### Comparing `dgisim-0.2.dev2/dgisim/src/status/status_processing.py` & `dgisim-0.2.dev3/dgisim/src/status/status_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 from ..summon import summon as sm
 from ..support import support as sp
 
 from ..character.enums import CharacterSkill
 from ..state.enums import Pid
 from ..effect.enums import Zone, TriggeringSignal
 from ..effect.structs import StaticTarget
-from .enums import Preprocessables
+from ..event import *
+from .enums import Preprocessables, Informables
 
 if TYPE_CHECKING:
     from ..card.card import Card
     from ..state.game_state import GameState
 
-    from .types import Preprocessable
-
 __all__ = [
     "StatusProcessing",
 ]
 
 class StatusProcessing:
     """
     This class holds static methods that facilitate the preprocessing of items by
@@ -111,15 +110,18 @@
         Takes the current game_state, trigger all statuses in order of player pid
         Returns the triggering effects in order (first to last)
         """
         effects: list[eft.Effect] = []
 
         def f(game_state: GameState, status: stt.Status, target: StaticTarget) -> GameState:
             nonlocal effects
-            if isinstance(status, stt.CharacterTalentStatus) \
+            if signal not in status.REACTABLE_SIGNALS:
+                return game_state
+
+            if isinstance(status, stt.HiddenStatus) \
                     or isinstance(status, stt.EquipmentStatus) \
                     or isinstance(status, stt.CharacterStatus):
                 effects.append(eft.TriggerStatusEffect(target, type(status), signal))
 
             elif isinstance(status, stt.CombatStatus):
                 effects.append(eft.TriggerCombatStatusEffect(target.pid, type(status), signal))
 
@@ -135,22 +137,22 @@
         StatusProcessing.loop_all_statuses(game_state, pid, f)
         return effects
 
     @staticmethod
     def preprocess_by_all_statuses(
             game_state: GameState,
             pid: Pid,
-            item: Preprocessable,
             pp_type: Preprocessables,
-    ) -> tuple[GameState, Preprocessable]:
+            item: PreprocessableEvent,
+    ) -> tuple[GameState, PreprocessableEvent]:
         def f(game_state: GameState, status: stt.Status, status_source: StaticTarget) -> GameState:
             nonlocal item
             item, new_status = status.preprocess(game_state, status_source, item, pp_type)
 
-            if isinstance(status, stt.CharacterTalentStatus) \
+            if isinstance(status, stt.HiddenStatus) \
                     or isinstance(status, stt.EquipmentStatus) \
                     or isinstance(status, stt.CharacterStatus):
                 if new_status is None:
                     game_state = eft.RemoveCharacterStatusEffect(
                         status_source, type(status)).execute(game_state)
                 elif new_status != status:
                     assert type(status) == type(new_status)
@@ -209,20 +211,20 @@
         game_state = StatusProcessing.loop_all_statuses(game_state, pid, f)
         return game_state, item
 
     @staticmethod
     def inform_all_statuses(
             game_state: GameState,
             pid: Pid,
-            info: eft.SpecificDamageEffect | CharacterSkill | Card,
-            source: None | StaticTarget = None,
+            info_type: Informables,
+            info: InformableEvent,
     ) -> GameState:
         def f(game_state: GameState, status: stt.Status, status_source: StaticTarget) -> GameState:
             return status.inform(
                 game_state,
                 status_source,
+                info_type,
                 info,
-                info_source=source,
             )
 
         game_state = StatusProcessing.loop_all_statuses(game_state, pid, f)
         return game_state
```

### Comparing `dgisim-0.2.dev2/dgisim/src/status/statuses.py` & `dgisim-0.2.dev3/dgisim/src/status/statuses.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 _U = TypeVar('_U')
 
 
 class Statuses:
     """
     A container for easy statuses managing.
     """
+
     def __init__(self, statuses: tuple[stt.Status, ...]):
         self._statuses = statuses
 
     def update_status(self, incoming_status: stt.Status, override: bool = False) -> Self:
         """
         Replaces existing status of the same type with the new_status,
         or append the new_status to the end of current statuses
@@ -43,14 +44,17 @@
             return cls(tuple(statuses))
         statuses.append(incoming_status)
         return cls(tuple(statuses))
 
     def contains(self, status: type[stt.Status]) -> bool:
         return any(type(b) is status for b in self._statuses)
 
+    def __contains__(self, status: type[stt.Status]) -> bool:
+        return self.contains(status)
+
     def find(self, status: type[stt.Status]) -> None | stt.Status:
         return next((bf for bf in self._statuses if type(bf) is status), None)
 
     def just_find(self, status: type[_U]) -> _U:
         """ _U should be a subclass of type[Status] """
         assert issubclass(status, stt.Status)
         found_status = just(self.find(status))
@@ -67,15 +71,15 @@
 
     def __iter__(self) -> Iterator[stt.Status]:
         return iter(self._statuses)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Statuses):
             return False
-        return self is other or self == other
+        return self is other or self._statuses == other._statuses
 
     def __hash__(self) -> int:
         return hash(self._statuses)
 
     def __str__(self) -> str:
         return '[' + ', '.join(map(str, self._statuses)) + ']'
 
@@ -83,16 +87,41 @@
         return [
             str(status)
             for status in self._statuses
         ]
 
 
 class EquipmentStatuses(Statuses):
-    pass
-
-
-class OrderedStatuses(Statuses):
-    pass
+    _CATEGORIES = (stt.TalentEquipmentStatus, stt.WeaponEquipmentStatus,
+                   stt.ArtifactEquipmentStatus)
 
-
-class TalentStatuses(Statuses):
-    pass
+    def update_status(self, incoming_status: stt.Status, override: bool = False) -> Self:
+        """
+        Replaces existing status of the same type with the new_status,
+        or append the new_status to the end of current statuses
+        """
+        cls = type(self)
+        statuses = list(self._statuses)
+        for i, status in enumerate(statuses):
+            same_category = False
+            for category in self._CATEGORIES:
+                if isinstance(incoming_status, category) and isinstance(status, category):
+                    same_category = True
+                    break
+            if not same_category:
+                continue
+            if type(status) is not type(incoming_status):
+                return self.remove(type(status)).update_status(incoming_status)
+            new_status: Optional[stt.Status]
+            if override:
+                new_status = incoming_status
+            else:
+                assert type(status) is type(incoming_status)
+                new_status = status.update(incoming_status)  # type: ignore
+            if status == new_status:
+                return self
+            if new_status is None:
+                return self.remove(type(status))
+            statuses[i] = new_status
+            return cls(tuple(statuses))
+        statuses.append(incoming_status)
+        return cls(tuple(statuses))
```

### Comparing `dgisim-0.2.dev2/dgisim/src/summon/summons.py` & `dgisim-0.2.dev3/dgisim/src/summon/summons.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,18 +65,35 @@
 
     def __iter__(self) -> Iterator[Summon]:
         return iter(self._summons)
 
     def __str__(self) -> str:  # pragma: no cover
         return f"[{', '.join(map(str, self._summons))}]"
 
+    def empty(self) -> bool:
+        return not bool(self._summons)
+
     def len(self) -> int:
         return len(self)
 
     def __len__(self) -> int:
         return len(self._summons)
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self is other or (
+            self._summons == other._summons
+            and self._max_num == other._max_num
+        )
+
+    def __hash__(self) -> int:
+        return hash((
+            self._summons,
+            self._max_num,
+        ))
+
     def dict_str(self) -> dict:
         return dict(
-            (summon.__class__.__name__.removesuffix("Summon"), str(summon.usages))
+            (summon.__class__.__name__.removesuffix("Summon"), str(summon.content_repr()))
             for summon in self
         )
```

### Comparing `dgisim-0.2.dev2/dgisim/src/support/support.py` & `dgisim-0.2.dev3/dgisim/src/support/support.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 from __future__ import annotations
 from dataclasses import dataclass, replace
 from typing import ClassVar, TYPE_CHECKING
 from typing_extensions import Self, override
 
 from ..card import card as cd
 from ..effect import effect as eft
-from ..event import CardEvent
+from ..event import *
 from ..status import status as stt
 
 from ..effect.enums import TriggeringSignal
 from ..element import Element
 from ..helper.quality_of_life import BIG_INT
 from ..status.enums import Preprocessables
 
 if TYPE_CHECKING:
     from ..state.game_state import GameState
     from ..effect.structs import StaticTarget
-    from ..status.types import Preprocessable
 
 __all__ = [
     # base
     "Support",
 
     # concrete implementations
     "XudongSupport",
@@ -53,25 +52,28 @@
         return ""
 
 
 @dataclass(frozen=True, kw_only=True)
 class XudongSupport(Support):
     usages: int = 1
     COST_DEDUCTION: ClassVar[int] = 2
+    REACTABLE_SIGNALS: ClassVar[frozenset[TriggeringSignal]] = frozenset((
+        TriggeringSignal.ROUND_END,
+    ))
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
-            item: Preprocessable,
+            item: PreprocessableEvent,
             signal: Preprocessables,
-    ) -> tuple[Preprocessable, None | Self]:
+    ) -> tuple[PreprocessableEvent, None | Self]:
         if signal is Preprocessables.CARD:
-            assert isinstance(item, CardEvent)
+            assert isinstance(item, CardPEvent)
             if item.pid is status_source.pid \
                     and issubclass(item.card_type, cd.FoodCard) \
                     and item.dices_cost.num_dices() > 0 \
                     and self.usages > 0:
                 # note that this only handle cases when food requires only one kind of dices
                 major_elem: Element
                 if item.dices_cost[Element.OMNI] == item.dices_cost.num_dices():
@@ -82,15 +84,15 @@
                     raise NotImplementedError
                 new_cost = (item.dices_cost - {major_elem: self.COST_DEDUCTION}).validify()
                 return replace(item, dices_cost=new_cost), replace(self, usages=self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
 
     @override
     def _react_to_signal(
-            self, source: StaticTarget, signal: TriggeringSignal
+            self, game_state: GameState, source: StaticTarget, signal: TriggeringSignal
     ) -> tuple[list[eft.Effect], None | Self]:
         if signal is TriggeringSignal.ROUND_END:
             return [], type(self)(sid=self.sid)
         return [], self
 
     @override
     def content_str(self) -> str:
```

### Comparing `dgisim-0.2.dev2/dgisim/src/support/supports.py` & `dgisim-0.2.dev3/dgisim/src/support/supports.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def find_by_sid(self, sid: int) -> None | Support:
         return next((
             s
             for s in self._supports
             if s.sid == sid
         ), None)
 
-    def just_find_by_sid(self, sid: int) -> None | Support:
+    def just_find_by_sid(self, sid: int) -> None | Support:  # pragma: no cover
         return just(self.find_by_sid(sid))
 
     def update_support(self, incoming_support: Support, override: bool = False) -> Supports:
         supports = list(self._supports)
         for i, support in enumerate(supports):
             sid = support.sid
             if type(support) != type(incoming_support) \
@@ -55,15 +55,15 @@
             if support == new_support:
                 return self
             if new_support is None:
                 return self.remove_support(type(support), support.sid)
             supports[i] = new_support
             return Supports(tuple(supports), self._max_num)
         if len(supports) >= self._max_num:
-            raise Exception("Should not be reached. "
+            raise Exception("Not Reached. "
                             + "Handle support destruction before updating when supports are full.")
         if any(s.sid == incoming_support.sid for s in supports):
             raise Exception("Incoming support cannot be added when support with same sid exists.")
         supports.append(incoming_support)
         return Supports(tuple(supports), self._max_num)
 
     def new_sid(self, support_type: type[Support]) -> int:
@@ -73,22 +73,22 @@
             i += 1
         return i
 
     def remove_support(self, support_type: type[Support], sid: int) -> Supports:
         return Supports(tuple(
             s
             for s in self._supports
-            if type(s) is support_type and s.sid == sid
+            if not(type(s) is support_type and s.sid == sid)
         ), self._max_num)
 
     def remove_by_sid(self, sid: int) -> Supports:
         return Supports(tuple(
             s
             for s in self._supports
-            if s.sid == sid
+            if s.sid != sid
         ), self._max_num)
 
     def full(self) -> bool:
         return len(self) == self._max_num
 
     def contains_exactly(self, support_type: type[Support], sid: int) -> bool:
         return any(
@@ -113,14 +113,28 @@
 
     def len(self) -> int:
         return len(self)
 
     def __len__(self) -> int:
         return len(self._supports)
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self is other or (
+            self._supports == other._supports
+            and self._max_num == other._max_num
+        )
+
+    def __hash__(self) -> int:
+        return hash((
+            self._supports,
+            self._max_num,
+        ))
+
     def dict_str(self) -> dict:
         return dict(
             (
                 support.__class__.__name__.removesuffix("Support") + f"<{support.sid}>",
                 support.content_str()
             )
             for support in self
```

### Comparing `dgisim-0.2.dev2/dgisim.egg-info/PKG-INFO` & `dgisim-0.2.dev3/dgisim.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgisim
-Version: 0.2.dev2
+Version: 0.2.dev3
 Summary: A highly customizable Genius Invokation TCG Simulator for AI training
 Author: Jarvis Yu
 License: MIT License
         
         Copyright (c) 2023 Leyang Yu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,29 +65,35 @@
 ```
 pip install dgisim
 ```
 
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
 
-## [Documentation](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
+## [Wiki](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
 
-## Simple Guide
+- [v0.2.dev2 documentation](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev2-Documentation)
+- [state machine design](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/state_machine_design.md)
+- [run cloned repository locally](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/dev_readme.md)
+
+## Simple Start With CLI
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
 
 You might want to run a simple python program like this:
 
 ```py
 from dgisim import CLISession
 
 session = CLISession()
 session.run()
 ```
 
+Or try the CLI online on [Google Colab](https://colab.research.google.com/drive/1h6ckw4LQ2jMEnZAs9QQo6tHjCwWnR8KD?usp=sharing)
+
 See CLI's [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/cli_readme.md)
 for showcase and explanations of the CLI.
 
 ## Features of This Simulator
 
 First of all, it is modeled as a finite state machine, which means any intermediate state can be
 standalone and be used to proceed to other states.
@@ -100,59 +106,41 @@
 branches of possibilities in the future are not error-prone. Do not worry about memory efficiency,
 everything is immutable, so only the modified part between neighbouring game states are added to the
 memory.
 
 `GameState` implements `__eq__` and `__hash__`, enabling you to use any game state as a key in a
 dictionary, and discover game states on different 'game branches' being actually the same.
 
+## [State Machine Design](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/state_machine_design.md)
+
 ## Development Milestones
 
 - [x] Set up the framework for maintaining game states
 - [x] Implement game phase of Card Selection (card selection at the start of the game)
 - [x] Implement game phase of Starting Hand Select Phase (select active character)
 - [x] Implement game phase of Roll (Dice) Phase (roll dices between rounds)
 - [x] Implement game phase of Action Phase (players beat each other)
-  - [ ] Implement all cards (15/184 implemented)
-    - [x] Changing Shifts,
-          ColdBlooded Strike,
-          Jueyun Guoba,
-          Leave It to Me!,
-          Lightning Stiletto,
-          Lotus Flower Crisp,
-          Minty Meat Rolls,
-          Mondstadt Hash Brown,
-          Mushroom Pizza,
-          Nothern Smoked Chicken,
-          Starsigns,
-          Streaming Surge,
-          Sweet Madame,
-          Thundering Penance,
-          Xudong,
-  - [ ] Implement all characters with their talent cards (3/48 implemented)
-    - [x] Kaeya,
-          Keqing,
-          Rhodeia of Loch,
+  - [ ] Implement all cards (26/192 implemented) ([details](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/progress.md))
+  - [ ] Implement all characters with their talent cards (7/51 implemented) ([details](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/progress.md))
   - [x] Implement all reactions
+  - [x] Implement all logics to support the implemented cards and characters
 - [x] Implement game phase of End Phase (summons and some support card or statuses take action)
 - [x] Implement game phase of Game End Phase (one player wins or draw)
 - [x] Implement CLI for better debugging experience
 - [x] Implement interactive active CLI that accepts user input as action
 - [x] Implement lazy player agent for minimal testing purposes
 - [x] Implement random player agent for testing purposes
 - [x] Implement player action validity checker
 - [x] Implement player action choices provider
-- [ ] Implement greedy player agent for testing purposes
-
-> Just in case you don't know, **_WIP_** means "work in progress".
 
 ## Future Plans
 
 I have the plan to implement a simple cross-platform GUI interface for the simulator. But that will
 be in a separate repo.
 
 Once this project is done, I'll be reading relative papers and develop an AI for this game. The AI
 is supposed to be used for learning strategies and making decks, but not against another player
 directly.
 
-## Interested in the Project?
+## Wants To Contribute?
 
-Please read this [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/dev_readme.md).
+Please read [this](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/dev_readme.md).
```

### Comparing `dgisim-0.2.dev2/dgisim.egg-info/SOURCES.txt` & `dgisim-0.2.dev3/dgisim.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 dgisim/src/effect/structs.py
 dgisim/src/helper/__init__.py
 dgisim/src/helper/hashable_dict.py
 dgisim/src/helper/level_print.py
 dgisim/src/helper/quality_of_life.py
 dgisim/src/phase/__init__.py
 dgisim/src/phase/phase.py
+dgisim/src/phase/all_omni/__init__.py
+dgisim/src/phase/all_omni/roll_phase.py
 dgisim/src/phase/default/__init__.py
 dgisim/src/phase/default/action_phase.py
 dgisim/src/phase/default/card_select_phase.py
 dgisim/src/phase/default/end_phase.py
 dgisim/src/phase/default/game_end_phase.py
 dgisim/src/phase/default/roll_phase.py
 dgisim/src/phase/default/starting_hand_select_phase.py
@@ -54,14 +56,13 @@
 dgisim/src/state/game_state.py
 dgisim/src/state/player_state.py
 dgisim/src/status/__init__.py
 dgisim/src/status/enums.py
 dgisim/src/status/status.py
 dgisim/src/status/status_processing.py
 dgisim/src/status/statuses.py
-dgisim/src/status/types.py
 dgisim/src/summon/__init__.py
 dgisim/src/summon/summon.py
 dgisim/src/summon/summons.py
 dgisim/src/support/__init__.py
 dgisim/src/support/support.py
 dgisim/src/support/supports.py
```

### Comparing `dgisim-0.2.dev2/pyproject.toml` & `dgisim-0.2.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dgisim"
-version = "0.2.dev2"
+version = "0.2.dev3"
 license = {file = "LICENSE"}
 
 description = "A highly customizable Genius Invokation TCG Simulator for AI training"
 authors = [{ name="Jarvis Yu" }]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
```

