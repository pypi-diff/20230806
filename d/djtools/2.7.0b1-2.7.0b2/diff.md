# Comparing `tmp/djtools-2.7.0b1.tar.gz` & `tmp/djtools-2.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djtools-2.7.0b1.tar", last modified: Tue Aug  1 16:32:28 2023, max compression
+gzip compressed data, was "djtools-2.7.0b2.tar", last modified: Sun Aug  6 00:41:13 2023, max compression
```

## Comparing `djtools-2.7.0b1.tar` & `djtools-2.7.0b2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.806547 djtools-2.7.0b1/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.7.0b1/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.7.0b1/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-08-01 16:32:28.806641 djtools-2.7.0b1/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1632 2023-07-29 18:53:45.000000 djtools-2.7.0b1/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.767990 djtools-2.7.0b1/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2621 2023-07-29 19:17:36.000000 djtools-2.7.0b1/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-29 19:17:36.000000 djtools-2.7.0b1/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.786082 djtools-2.7.0b1/djtools/collection/
--rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.7.0b1/djtools/collection/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27429 2023-07-26 18:56:00.000000 djtools-2.7.0b1/djtools/collection/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.7.0b1/djtools/collection/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/collection/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.793626 djtools-2.7.0b1/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-26 18:24:13.000000 djtools-2.7.0b1/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1485 2023-08-01 16:23:50.000000 djtools-2.7.0b1/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    22278 2023-08-01 15:46:44.000000 djtools-2.7.0b1/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:30.000000 djtools-2.7.0b1/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.794478 djtools-2.7.0b1/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.797211 djtools-2.7.0b1/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.799890 djtools-2.7.0b1/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.7.0b1/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5343 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.806016 djtools-2.7.0b1/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)     1441 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4233 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2120 2023-08-01 15:47:39.000000 djtools-2.7.0b1/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9264 2023-07-29 18:53:45.000000 djtools-2.7.0b1/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1859 2023-08-01 16:20:25.000000 djtools-2.7.0b1/djtools/utils/normalize_audio.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5098 2023-08-01 15:47:27.000000 djtools-2.7.0b1/djtools/utils/process_recording.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.7.0b1/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-08-01 16:15:23.000000 djtools-2.7.0b1/djtools/version.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-01 16:32:28.775431 djtools-2.7.0b1/djtools.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2864 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1277 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      278 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-08-01 16:32:28.000000 djtools-2.7.0b1/djtools.egg-info/top_level.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.7.0b1/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-08-01 16:32:28.807159 djtools-2.7.0b1/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2361 2023-07-29 19:17:36.000000 djtools-2.7.0b1/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.399328 djtools-2.7.0b2/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.7.0b2/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.7.0b2/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2964 2023-08-06 00:41:13.399459 djtools-2.7.0b2/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1732 2023-08-06 00:40:41.000000 djtools-2.7.0b2/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.370531 djtools-2.7.0b2/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2621 2023-07-29 19:17:36.000000 djtools-2.7.0b2/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-29 19:17:36.000000 djtools-2.7.0b2/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.379896 djtools-2.7.0b2/djtools/collection/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/collection/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13140 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/collection/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.7.0b2/djtools/collection/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/collection/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    31479 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/collection/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.7.0b2/djtools/collection/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16104 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/collection/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/collection/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15806 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/collection/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.384641 djtools-2.7.0b2/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.7.0b2/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1302 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1485 2023-08-05 23:50:51.000000 djtools-2.7.0b2/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    22330 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.7.0b2/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-07-29 19:28:30.000000 djtools-2.7.0b2/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.385019 djtools-2.7.0b2/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.7.0b2/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.387766 djtools-2.7.0b2/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.390831 djtools-2.7.0b2/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.7.0b2/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5343 2023-07-29 18:53:45.000000 djtools-2.7.0b2/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.398021 djtools-2.7.0b2/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1441 2023-07-29 18:53:45.000000 djtools-2.7.0b2/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4233 2023-07-29 18:53:45.000000 djtools-2.7.0b2/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2120 2023-08-05 14:56:47.000000 djtools-2.7.0b2/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9264 2023-07-29 18:53:45.000000 djtools-2.7.0b2/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1859 2023-08-05 14:56:47.000000 djtools-2.7.0b2/djtools/utils/normalize_audio.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5098 2023-08-05 14:56:47.000000 djtools-2.7.0b2/djtools/utils/process_recording.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.7.0b2/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-08-06 00:40:41.000000 djtools-2.7.0b2/djtools/version.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-08-06 00:41:13.374606 djtools-2.7.0b2/djtools.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2964 2023-08-06 00:41:13.000000 djtools-2.7.0b2/djtools.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1277 2023-08-06 00:41:13.000000 djtools-2.7.0b2/djtools.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-08-06 00:41:13.000000 djtools-2.7.0b2/djtools.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-08-06 00:41:13.000000 djtools-2.7.0b2/djtools.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      278 2023-08-06 00:41:13.000000 djtools-2.7.0b2/djtools.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-08-06 00:41:13.000000 djtools-2.7.0b2/djtools.egg-info/top_level.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.7.0b2/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-08-06 00:41:13.399889 djtools-2.7.0b2/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2361 2023-07-29 19:17:36.000000 djtools-2.7.0b2/setup.py
```

### Comparing `djtools-2.7.0b1/LICENSE` & `djtools-2.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/PKG-INFO` & `djtools-2.7.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.7.0b1
+Version: 2.7.0b2
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -41,13 +41,14 @@
     - [x] Script for removing situation tags and resolving album, label, and year for tracks
     - [x] Allow `build_config` to accept an override for the path to `config.yaml`
     - [x] Fix missing typehints for the `NonEmptyListElementAction` class
     - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
     - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
     - [x] [Standardize audio files](https://github.com/a-rich/DJ-Tools/issues/126)
     - [x] [Process recorded file using Spotify playlist](https://github.com/a-rich/DJ-Tools/issues/127)
+    - [x] [Improve selectors for Combiner playlists](https://github.com/a-rich/DJ-Tools/issues/131)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
     - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
     - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
 
 # Contribution
 Please see the [CONTRIBUTING](CONTRIBUTING.md)
```

### Comparing `djtools-2.7.0b1/README.md` & `djtools-2.7.0b2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,13 +11,14 @@
     - [x] Script for removing situation tags and resolving album, label, and year for tracks
     - [x] Allow `build_config` to accept an override for the path to `config.yaml`
     - [x] Fix missing typehints for the `NonEmptyListElementAction` class
     - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
     - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
     - [x] [Standardize audio files](https://github.com/a-rich/DJ-Tools/issues/126)
     - [x] [Process recorded file using Spotify playlist](https://github.com/a-rich/DJ-Tools/issues/127)
+    - [x] [Improve selectors for Combiner playlists](https://github.com/a-rich/DJ-Tools/issues/131)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
     - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
     - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
 
 # Contribution
 Please see the [CONTRIBUTING](CONTRIBUTING.md)
```

### Comparing `djtools-2.7.0b1/djtools/__init__.py` & `djtools-2.7.0b2/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/__main__.py` & `djtools-2.7.0b2/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/collection/__init__.py` & `djtools-2.7.0b2/djtools/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/collection/collections.py` & `djtools-2.7.0b2/djtools/collection/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,36 +41,41 @@
 
         Args:
             playlist: Playlist to append to the collection.
         """
         self._playlists.add_playlist(playlist)  # pylint:disable=no-member
 
     def get_playlists(
-        self, name: Optional[str] = None
+        self, name: Optional[str] = None, glob: Optional[bool] = False
     ) -> Union[Playlist, List[Playlist]]:
         """Returns Playlists with a matching name.
 
         If no playlist name is provided, then the root playlist is returned.
 
         Args:
             name: Name of the Playlists to return.
+            glob: Glob on playlist name containing "*".
 
         Returns:
             The Playlists with the same name.
         """
         if not name:
             return self._playlists  # pylint:disable=no-member
 
+        exp = re.compile(r".*".join(name.split("*")))
         playlists = []
         for playlist in self._playlists:  # pylint:disable=no-member
-            if playlist.get_name() == name:
+            if (
+                (glob and re.search(exp, playlist.get_name())) or
+                (not glob and playlist.get_name() == name)
+            ):
                 playlists.append(playlist)
             if playlist.is_folder():
                 for playlist in playlist:
-                    playlists.extend(playlist.get_playlists(name))
+                    playlists.extend(playlist.get_playlists(name, glob=glob))
 
         return [playlist for playlist in playlists if playlist is not None]
 
     def get_tracks(self) -> Dict[str, Track]:
         """Returns the tracks in the collection.
 
         Returns:
```

### Comparing `djtools-2.7.0b1/djtools/collection/config.py` & `djtools-2.7.0b2/djtools/collection/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/collection/copy_playlists.py` & `djtools-2.7.0b2/djtools/collection/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/collection/helpers.py` & `djtools-2.7.0b2/djtools/collection/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module contains helpers for the collection package."""
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from collections import defaultdict
+from datetime import datetime
 import logging
 from operator import itemgetter
 from pathlib import Path
 import re
 import shutil
 from typing import Dict, List, Optional, Set, Tuple, Union
 
@@ -49,17 +50,18 @@
 #       tracks that have hip hop influences
 #   - MinimalDeepTechFilter: used to distinguish between minimal deep tech
 #       tracks with predominately house and techno influences
 #   - filter_tag_playlists: applies PlaylistFilter implementations to built tag
 #       playlists
 #   - aggregate_playlists: aggregates tracks from playlists in folders to
 #       create an "All <folder name>" playlist in each folder
-#   - add_selectors_to_tags: parses combiner playlist names and finds BPM,
-#       rating, and playlist selectors to update the tag -> track lookup
-#   - parse_bpms_and_ratings: used to parse BPM and rating selectors
+#   - add_selectors_to_tags: parses combiner playlist names and finds numerical
+#       and string selectors to update the tag -> track lookup
+#   - parse_numerical_selectors: used to parse numerical selectors like
+#       ratings, BPMs, and years
 #   - build_combiner_playlists: builds collection playlists using "combiner"
 #       component of the PlaylistConfig
 #   - parse_expression: evaluates the boolean algebra logic in combiner
 #       playlists names to populate them with the appropriate tracks
 #   - BooleanNode: used to build and evaluate the boolean algebra parse tree
 #   - print_playlist_tag_statistics: prints ASCII histograms showing tag
 #       frequencies in combiner playlists split by genre and other tag types
@@ -402,112 +404,221 @@
 
     Args:
         playlist_config: PlaylistConfig object.
         tags_tracks: Dict of tags to tracks.
         collection: Collection object.
         auto_playlists: Tag playlists built in this same run.
     """
+    numerical_selector_regex = re.compile(r"(?<=\[)[^\[\]]*(?=\])")
+    numerical_value_lookup = {}
+    numerical_value_set = set()
+    string_selector_regex = re.compile(r"(?<={)[^{}]+:[^{}]+(?=})")
+    string_selector_type_map = {
+        "artist": "get_artists",
+        "comment": "get_comments",
+        "date": "get_date_added",
+        "key": "get_key",
+        "label": "get_label",
+    }
+    string_value_lookup = {}
     playlists = set()
-    values_set = set()
-    bpm_rating_lookup = {}
-    playlist_selector_regex = r"(?<={)[^{}]*(?=})"
-    bpm_rating_selector_regex = r"(?<=\[)[^\[\]]*(?=\])"
 
     # Grab selectors from Combiner playlists' names.
     for playlist in playlist_config.combiner.playlists:
-        playlists.update(re.findall(playlist_selector_regex, playlist))
-        bpm_rating_matches = re.findall(bpm_rating_selector_regex, playlist)
-        if not bpm_rating_matches:
-            continue
-        parsed_bpms, parsed_ratings = parse_bpms_and_ratings(
-            bpm_rating_matches, bpm_rating_lookup
+        numerical_value_set.update(
+            parse_numerical_selectors(
+                re.findall(numerical_selector_regex, playlist),
+                numerical_value_lookup,
+            )
+        )
+        parse_string_selectors(
+            re.findall(string_selector_regex, playlist),
+            string_value_lookup,
+            string_selector_type_map,
+            playlists,
         )
-        values_set.update(parsed_bpms)
-        values_set.update(parsed_ratings)
 
-    # Add keys for BPM and rating selectors for tracks having those values.
-    for track_id, track in collection.get_tracks().items():
-        values = map(str, [round(track.get_bpm()), track.get_rating()])
-        for val in values:
-            if val not in values_set:
-                continue
-            for value, tag in bpm_rating_lookup.items():
+    # Add keys for numerical selectors for tracks having those values.
+    for value, tag in numerical_value_lookup.items():
+        for track_id, track in collection.get_tracks().items():
+            values = map(
+                str, [round(track.get_bpm()), track.get_rating(), track.get_year()]
+            )
+            for val in values:
                 if (
                     (isinstance(value, str) and value == val) or
                     (isinstance(value, tuple) and val in value)
                 ):
                     tags_tracks[tag][track_id] = track
 
+    # Add keys for string selectors for tracks having those values.
+    for selector, tag in string_value_lookup.items():
+        selector_type, selector_value = selector
+        for track_id, track in collection.get_tracks().items():
+            value = getattr(track, string_selector_type_map[selector_type])()
+            if not value:
+                continue
+            if selector_type == "date":
+                inequality, date, date_format = selector_value
+                if not inequality:
+                    if value.strftime(date_format) == date.strftime(date_format):
+                        tags_tracks[tag][track_id] = track
+                    continue
+                if not inequality(value, date):
+                    continue
+                tags_tracks[tag][track_id] = track
+                continue
+            if "*" in selector_value:
+                exp = re.compile(r".*".join(selector_value.lower().split("*")))
+                if re.search(exp, value.lower()):
+                    tags_tracks[tag][track_id] = track
+                    continue
+            if value.lower() == selector_value.lower():
+                tags_tracks[tag][track_id] = track
+
     # Get playlists for the identified playlist selectors. Not only must we get
     # playlists from the collection, but we must also get playlists from the
     # auto playlists constructed in the very same run of the playlist_builder.
     # This is because the playlists being selected may include those generated
     # by the playlist_builder.
     for playlist_name in playlists:
         for playlist_object in [collection, *auto_playlists]:
             for playlist in playlist_object.get_playlists(playlist_name):
-                tags_tracks[f"{{{playlist_name}}}"].update(
+                tags_tracks[f"{{playlist:{playlist_name}}}"].update(
                     playlist.get_tracks()
                 )
 
 
-def parse_bpms_and_ratings(
-    bpm_rating_match: List[str],
-    bpm_rating_lookup: Dict[Union[str, Tuple], str],
-) -> List[Tuple]:
-    """Parses a string match of one or more BPM and / or rating selectors.
+def parse_numerical_selectors(
+    numerical_matches: List[str],
+    numerical_value_lookup: Dict[Union[str, Tuple], str],
+) -> Set[str]:
+    """Parses a string match of one or more numerical selectors.
 
     Args:
-        bpm_rating_match: List of BPM or rating strings.
-        bpm_rating_lookup: Empty dict to populate with tuples or strings
-            mapping bpm or rating ranges or values to their "tag"
-            representation.
+        numerical_matches: List of numerical strings.
+        numerical_value_lookup: Empty dict to populate with tuples or strings
+            mapping numerical ranges or values to their "tag" representation.
 
     Returns:
-        Tuple of BPM and rating lists.
+        Set of numerical selector values.
     """
-    bpms, ratings = [], []
-    for bpm_rating in bpm_rating_match:
-        parts = map(str.strip, bpm_rating.split(","))
-        for part in parts:
-            number = _range = None
-            # If "part" is a digit, then it's an explicit BPM or rating to
-            # filter for.
-            if part.isdigit():
-                number = int(part)
-                if 0 <= number <= 5:
-                    ratings.append(str(number))
-                elif number > 5:
-                    bpms.append(str(number))
-            # If "part" is two digits separated by a "-", then it's a range
-            # of BPMs or ratings to filter for.
-            elif (
-                len(part.split("-")) == 2 and
-                all(x.isdigit() for x in part.split("-"))
+    numerical_values = set()
+    for match in numerical_matches:
+        _range = None
+        # If "match" is a digit, then it's an explicit numerical value.
+        if match.isdigit():
+            numerical_values.add(match)
+        # If "match" is two digits separated by a "-", then it's a range.
+        elif (
+            len(match.split("-")) == 2 and
+            all(x.isdigit() for x in match.split("-"))
+        ):
+            _range = list(map(int, match.split("-")))
+            _range = range(min(_range), max(_range) + 1)
+            if not (
+                all(0 <= x <= 5 for x in _range) or    # range for ratings
+                all(6 <= x <= 999 for x in _range) or  # range for BPMs
+                all(x >= 1000 for x in _range)         # range for years
             ):
-                _range = list(map(int, part.split("-")))
-                _range = range(min(_range), max(_range) + 1)
-                if all(0 <= x <= 5 for x in _range):
-                    ratings.extend(map(str, _range))
-                elif all(x > 5 for x in _range):
-                    bpms.extend(map(str, _range))
-                else:
-                    logger.error(f"Bad BPM or rating number range: {part}")
-                    continue
-            else:
-                logger.error(
-                    f"Malformed BPM or rating filter part: {part}"
-                )
+                logger.error(f"Bad numerical range selector: {match}")
+                continue
+            numerical_values.update(map(str, _range))
+        else:
+            logger.error(
+                f"Malformed numerical selector: {match}"
+            )
+            continue
+
+        numerical_value_lookup[
+            tuple(map(str, _range or [])) or match
+        ] = f"[{match}]"
+
+    return numerical_values
+
+
+def parse_string_selectors(
+    string_matches: List[str],
+    string_value_lookup:  Dict[Union[str, Tuple], str],
+    string_selector_type_map: Dict[str],
+    playlists: Set(str),
+):
+    """_summary_
+
+    Args:
+        string_matches: List of strings for string selectors.
+        string_value_lookup: Empty dict to populate with strings mapping string
+            selectors to their "tag" representation.
+        string_selector_type_map: Maps a selector type to a Track method name.
+        playlists: Set for storing playlist names.
+    """
+    date_selector_regex = re.compile(r"(>=|>|<=|<)")
+    date_formats = ["%Y-%m-%d", "%Y-%m", "%Y"]
+    inequality_map = {
+        ">": lambda x, y: x > y,
+        "<": lambda x, y: x < y,
+        ">=": lambda x, y: x >= y,
+        "<=": lambda x, y: x <= y,
+    }
+
+    for match in string_matches:
+        selector_type, selector_value = map(str.strip, match.split(":"))
+        if selector_type == "playlist":
+            playlists.add(selector_value)
+            continue
+        if not string_selector_type_map.get(selector_type):
+            logger.warning(f"{selector_type} is not a supported selector!")
+            continue
+        if selector_type != "date":
+            string_value_lookup[(selector_type, selector_value)] = (
+                f"{{{match}}}"
+            )
+            continue
+
+        dates, formats, inequalities = [], [], []
+        skip_date_selector = False
+        for part in filter(
+            None, re.split(date_selector_regex, selector_value)
+        ):
+            if re.search(date_selector_regex, part):
+                inequalities.append(inequality_map[part])
                 continue
 
-            bpm_rating_lookup[
-                tuple(map(str, _range or [])) or str(number)
-            ] = f"[{part}]"
+            date = None
+            for date_format in date_formats:
+                try:
+                    date = datetime.strptime(part, date_format)
+                except ValueError:
+                    continue
+                break
+            if not date:
+                skip_date_selector = True
+                break
+            dates.append(date)
+            formats.append(date_format)
 
-    return bpms, ratings
+        if (
+            skip_date_selector or
+            len(dates) != 1  or
+            (len(inequalities) not in [0, 1])
+        ):
+            logger.warning(f"Date selector {selector_value} is invalid!")
+            continue
+
+
+        string_value_lookup[
+            (
+                selector_type,
+                (
+                    None if not inequalities else inequalities[0],
+                    dates[0],
+                    formats[0]
+                )
+            )
+        ] = f"{{{match}}}"
 
 
 def build_combiner_playlists(
     playlist_config: PlaylistConfig,
     tags_tracks: Dict[str, Dict[str, Track]],
     playlist_class: Playlist,
 ) -> Playlist:
@@ -585,29 +696,34 @@
             "~": set.difference,
         }
         self._parent = parent
         self._operators = []
         self._tags = []
         self._tracks = []
         self._tags_tracks = tags_tracks
+        self._numerical_selector_regex = re.compile(r"(?<=\[)[^\[\]]*(?=\])")
+        self._string_selector_regex = re.compile(r"(?<={)[^{}]+:[^{}]+(?=})")
 
     def _get_tracks(self, tag: str) -> Set[str]:
         """Gets set of track IDs for the provided tag.
 
         If the tag contains a wildcard, denoted with "*", then the union of
         track IDs with a tag containing the provided tag as a sub-string is
         returned.
 
         Args:
             tag: Tag for indexing tracks.
 
         Returns:
             Set of track IDs for the provided tag.
         """
-        if "*" in tag:
+        if "*" in tag and not (
+            re.search(self._numerical_selector_regex, tag) or
+            re.search(self._string_selector_regex, tag)
+        ):
             exp = re.compile(r".*".join(tag.split("*")))
             tracks = {}
             for key in self._tags_tracks:
                 if re.search(exp, key):
                     tracks.update(self._tags_tracks[key])
             return tracks
```

### Comparing `djtools-2.7.0b1/djtools/collection/playlist_builder.py` & `djtools-2.7.0b2/djtools/collection/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/collection/playlists.py` & `djtools-2.7.0b2/djtools/collection/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 RekordboxPlaylist is an implementation of Playlist which operates on the XML
 format that Rekordbox exports.
 """
 from __future__ import annotations
 from abc import ABC, abstractmethod
 import inspect
 from pathlib import Path
+import re
 from typing import Any, Dict, List, Optional
 
 import bs4
 
 from djtools.collection.tracks import RekordboxTrack, Track
 
 
@@ -88,37 +89,44 @@
         """Returns the folder this playlist is in.
 
         Returns:
             A Playlist folder or None (if no parent).
         """
         return self._parent
 
-    def get_playlists(self, name: Optional[str] = None) -> List[Playlist]:
+    def get_playlists(
+        self, name: Optional[str] = None, glob: Optional[bool] = False
+    ) -> List[Playlist]:
         """Returns Playlists with a matching name.
 
         Args:
             name: Name of the Playlists to return.
+            glob: Glob on playlist name containing "*".
 
         Returns:
             The Playlists with the same name.
         """
         if not name:
             if not self.is_folder():
                 raise RuntimeError(
                     f'Playlist "{self.get_name()}" is not a folder so you '
                     f"cannot call get_playlists on it."
                 )
             return list(self)
 
+        exp = re.compile(r".*".join(name.split("*")))
         playlists = []
-        if self.get_name() == name:
+        if (
+            (glob and re.search(exp, self.get_name())) or
+            (not glob and self.get_name() == name)
+        ):
             playlists.append(self)
         if self.is_folder():
             for playlist in self:
-                playlists.extend(playlist.get_playlists(name))
+                playlists.extend(playlist.get_playlists(name, glob=glob))
 
         return [playlist for playlist in playlists if playlist is not None]
 
     def get_tracks(self) -> Dict[str, Track]:
         """Returns a dict of track IDs and tracks.
 
         Returns:
```

### Comparing `djtools-2.7.0b1/djtools/collection/shuffle_playlists.py` & `djtools-2.7.0b2/djtools/collection/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/collection/tracks.py` & `djtools-2.7.0b2/djtools/collection/tracks.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,30 +15,57 @@
 import re
 from typing import Any, List, Union, Set
 from urllib.parse import quote, unquote
 
 import bs4
 
 
+# pylint: disable=no-member
+
+
 class Track(ABC):
     "Abstract base class for a track."
 
     @abstractmethod
     def __init__(self, *args, **kwargs):
         "Deserializes a track from the native format of a DJ software."
 
     @abstractmethod
+    def get_artists(self) -> str:
+        """Gets the track artists.
+
+        Returns:
+            A string representing the track's artists.
+        """
+
+    @abstractmethod
     def get_bpm(self) -> float:
         """Gets the track BPM.
 
         Returns:
             A float representing BPM.
         """
 
     @abstractmethod
+    def get_comments(self) -> str:
+        """Gets the track comments.
+
+        Returns:
+            A string representing the track's comments.
+        """
+
+    @abstractmethod
+    def get_date_added(self) -> str:
+        """Gets the track's date added.
+
+        Returns:
+            A datetime representing the track's date added.
+        """
+
+    @abstractmethod
     def get_genre_tags(self) -> List[str]:
         """Gets the genre tags of the track.
 
         Returns:
             A list of the track's genre tags.            
         """
 
@@ -47,14 +74,30 @@
         """Gets the track ID.
 
         Returns:
             The ID of this track.
         """
 
     @abstractmethod
+    def get_key(self) -> Any:
+        """Gets the track key.
+
+        Returns:
+            The key of this track.
+        """
+
+    @abstractmethod
+    def get_label(self) -> Any:
+        """Gets the track label.
+
+        Returns:
+            The label of this track.
+        """
+
+    @abstractmethod
     def get_location(self) -> Path:
         """Gets the location of the track.
 
         Returns:
             The Path for the location of the track.
         """
 
@@ -71,14 +114,22 @@
         """Gets the tags of the track.
 
         Returns:
             A set of the track's tags.
         """
 
     @abstractmethod
+    def get_year(self) -> str:
+        """Gets the year of the track.
+
+        Returns:
+            The year of the track.
+        """
+
+    @abstractmethod
     def serialize(self, *args, **kwargs) -> Any:
         """Serializes a track into the native format of a DJ software.
 
         Returns:
             A serialized track of the same type used to initialize Track.
         """
 
@@ -141,21 +192,21 @@
             if key == "Rating":
                 value = {
                     "0": 0, "51": 1, "102": 2, "153": 3, "204": 4, "255": 5
                 }.get(value)
             setattr(self, f"_{key}", value)
 
         # Parse MyTag data from Comments attribute.
-        my_tags = re.search(r"(?<=\/\*).*(?=\*\/)", self._Comments)  # pylint: disable=no-member
+        my_tags = re.search(r"(?<=\/\*).*(?=\*\/)", self._Comments)
         self._MyTags = (  # pylint: disable=invalid-name
             [x.strip() for x in my_tags.group().split("/")] if my_tags else []
         )
 
         # Merge Genre and MyTag data into a new attribute.
-        self._Tags = set(self._Genre + self._MyTags)  # pylint: disable=no-member, invalid-name
+        self._Tags = set(self._Genre + self._MyTags)  # pylint: disable=invalid-name
 
         # Parse TEMPO Tags as the beat grid attribute.
         self._beat_grid = track.find_all("TEMPO")
         if self._beat_grid:
             self._beat_grid = [point.attrs for point in self._beat_grid]
 
         # Parse POSITION_MARK Tags as the hot cues attribute.
@@ -217,37 +268,77 @@
         """Produces a string representation of this track.
 
         Returns:
             Track represented as a string.
         """
         return str(self.serialize())
 
+    def get_artists(self) -> str:
+        """Gets the track artists.
+
+        Returns:
+            A string representing the track's artists.
+        """
+        return self._Artist
+
     def get_bpm(self) -> float:
         """Gets the track BPM.
 
         Returns:
             A float representing BPM.
         """
-        return self._AverageBpm  # pylint: disable=no-member
+        return self._AverageBpm
+
+    def get_comments(self) -> str:
+        """Gets the track comments.
+
+        Returns:
+            A string representing the track's comments.
+        """
+        return self._Comments
+
+    def get_date_added(self) -> str:
+        """Gets the track's date added.
+
+        Returns:
+            A datetime representing the track's date added.
+        """
+        return self._DateAdded
 
     def get_genre_tags(self) -> List[str]:
         """Gets the genre tags of the track.
 
         Returns:
             A list of the track's genre tags.            
         """
-        return self._Genre  # pylint: disable=no-member
+        return self._Genre
 
     def get_id(self) -> str:
         """Get the track ID.
 
         Returns:
             The ID of this track.
         """
-        return self._TrackID  # pylint: disable=no-member
+        return self._TrackID
+
+    def get_key(self) -> Any:
+        """Gets the track key.
+
+        Returns:
+            The key of this track.
+        """
+        return self._Tonality
+
+    def get_label(self) -> Any:
+        """Gets the track label.
+
+        Returns:
+            The label of this track.
+        """
+        return self._Label
 
     def get_location(self) -> Path:
         """Gets the location of the track.
 
         Returns:
             The Path for the location of the track.
         """
@@ -255,24 +346,32 @@
 
     def get_rating(self) -> int:
         """Gets the rating of the track.
 
         Returns:
             The rating of the track.
         """
-        return self._Rating  # pylint: disable=no-member
+        return self._Rating
 
     def get_tags(self) -> Set[str]:
         """Gets the tags of the track.
 
         Returns:
             A set of the track's tags.
         """
         return self._Tags
 
+    def get_year(self) -> str:
+        """Gets the year of the track.
+
+        Returns:
+            The year of the track.
+        """
+        return self._Year
+
     def serialize(
         self, *args, playlist: bool = False, **kwargs
     ) -> bs4.element.Tag:
         """Serializes this track as a BeautifulSoup TRACK Tag.
 
         Args:
             playlist: Whether or not to serialize this track as a member of a
@@ -396,15 +495,15 @@
 
     def set_track_number(self, number: int):
         """Sets the track number of a track.
 
         Args:
             number: Number to set for TrackNumber.
         """
-        self._TrackNumber = number  # pylint: disable=invalid-name,attribute-defined-outside-init
+        self._TrackNumber = number  # pylint: disable=attribute-defined-outside-init,invalid-name
 
     @classmethod
     def validate(cls, original: bs4.element.Tag, serializable: RekordboxTrack):
         """Validate the serialized track matches the original. 
 
         Args:
             original: BeautifulSoup Tag representing a track.
```

### Comparing `djtools-2.7.0b1/djtools/configs/collection_playlists.yaml` & `djtools-2.7.0b2/djtools/configs/collection_playlists.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 combiner:
   name: Combinations
   playlists:
+    - "{artist:*Tribe*} | {comment:*Dark*} | {date:2022} | {date:<2022} | {key:7A} | {label:Some Label}"
     - "(Dubstep | Hip Hop) | (Dubstep | Hip Hop)"
-    - "{Hip Hop} & [85-87]"
-    - "{Hip Hop} & [86]"
+    - "{playlist:Hip Hop} & [85-87]"
+    - "{playlist:Hip Hop} & [86]"
     - Dark & [2-5]
     - Dark & [5]
 tags:
   name: "Tags"
   playlists:
     - name: _ignore
       playlists:
```

### Comparing `djtools-2.7.0b1/djtools/configs/config.py` & `djtools-2.7.0b2/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/configs/config.yaml` & `djtools-2.7.0b2/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/configs/helpers.py` & `djtools-2.7.0b2/djtools/configs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,14 +519,16 @@
     if args.log_level:
         logger.setLevel(args.log_level)
 
     if args.version:
         print(__version__)
         sys.exit()
 
+    logger.info(f"djtools version: {__version__}")
+
     if args.link_configs:
         args.link_configs = Path(args.link_configs)
         if args.link_configs.exists():
             msg = (
                 f"{args.link_configs} must be a directory that does not "
                 "already exist"
             )
```

### Comparing `djtools-2.7.0b1/djtools/spotify/__init__.py` & `djtools-2.7.0b2/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/spotify/config.py` & `djtools-2.7.0b2/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/spotify/helpers.py` & `djtools-2.7.0b2/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/spotify/playlist_builder.py` & `djtools-2.7.0b2/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/sync/__init__.py` & `djtools-2.7.0b2/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/sync/config.py` & `djtools-2.7.0b2/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/sync/helpers.py` & `djtools-2.7.0b2/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/sync/sync_operations.py` & `djtools-2.7.0b2/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/__init__.py` & `djtools-2.7.0b2/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/check_tracks.py` & `djtools-2.7.0b2/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/config.py` & `djtools-2.7.0b2/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/helpers.py` & `djtools-2.7.0b2/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/normalize_audio.py` & `djtools-2.7.0b2/djtools/utils/normalize_audio.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/process_recording.py` & `djtools-2.7.0b2/djtools/utils/process_recording.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools/utils/url_download.py` & `djtools-2.7.0b2/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/djtools.egg-info/PKG-INFO` & `djtools-2.7.0b2/djtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.7.0b1
+Version: 2.7.0b2
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -41,13 +41,14 @@
     - [x] Script for removing situation tags and resolving album, label, and year for tracks
     - [x] Allow `build_config` to accept an override for the path to `config.yaml`
     - [x] Fix missing typehints for the `NonEmptyListElementAction` class
     - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
     - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
     - [x] [Standardize audio files](https://github.com/a-rich/DJ-Tools/issues/126)
     - [x] [Process recorded file using Spotify playlist](https://github.com/a-rich/DJ-Tools/issues/127)
+    - [x] [Improve selectors for Combiner playlists](https://github.com/a-rich/DJ-Tools/issues/131)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
     - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
     - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
 
 # Contribution
 Please see the [CONTRIBUTING](CONTRIBUTING.md)
```

### Comparing `djtools-2.7.0b1/djtools.egg-info/SOURCES.txt` & `djtools-2.7.0b2/djtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djtools-2.7.0b1/setup.py` & `djtools-2.7.0b2/setup.py`

 * *Files identical despite different names*

