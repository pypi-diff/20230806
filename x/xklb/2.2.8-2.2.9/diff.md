# Comparing `tmp/xklb-2.2.8.tar.gz` & `tmp/xklb-2.2.9.tar.gz`

## Comparing `xklb-2.2.8.tar` & `xklb-2.2.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.8/.gitattributes
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.8/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.8/Windows.md
--rw-r--r--   0        0        0   529549 2020-02-02 00:00:00.000000 xklb-2.2.8/pdm.lock
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.8/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.8/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.8/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.8/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/books.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/consts.py
--rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/dl_config.py
--rw-r--r--   0        0        0    10993 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/fs_extract.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/gdl_backend.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/hn_extract.py
--rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/lb.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/media.py
--rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/play_actions.py
--rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/playlists.py
--rw-r--r--   0        0        0    13480 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/praw_extract.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/subtitle.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/tube_backend.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/tube_extract.py
--rw-r--r--   0        0        0    85452 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/usage.py
--rw-r--r--   0        0        0    41680 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.8/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.8/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.8/LICENSE
--rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.8/README.md
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.8/pyproject.toml
--rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.9/.gitattributes
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.9/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.9/Windows.md
+-rw-r--r--   0        0        0   529549 2020-02-02 00:00:00.000000 xklb-2.2.9/pdm.lock
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.9/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/av.py
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/books.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/consts.py
+-rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/dl_config.py
+-rw-r--r--   0        0        0    10993 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/lb.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/media.py
+-rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/play_actions.py
+-rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/playlists.py
+-rw-r--r--   0        0        0    13480 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/subtitle.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/tube_backend.py
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/tube_extract.py
+-rw-r--r--   0        0        0    85452 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/usage.py
+-rw-r--r--   0        0        0    41680 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.9/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.9/LICENSE
+-rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.9/README.md
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.9/PKG-INFO
```

### Comparing `xklb-2.2.8/TODO` & `xklb-2.2.9/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/Windows.md` & `xklb-2.2.9/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/pdm.lock` & `xklb-2.2.9/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/readme.py` & `xklb-2.2.9/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/.github/workflows/push.yaml` & `xklb-2.2.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/av.py` & `xklb-2.2.9/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/books.py` & `xklb-2.2.9/xklb/books.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,11 +225,10 @@
         assert m["path"] == e.pop("SourceFile")
 
         try:
             m = munge_image_tags(m, e)
         except Exception as e:
             log.error("[%s]: %s", m["path"], e)
             # continue ?
-
         exif_enriched.append(m)
 
-    return metadata
+    return exif_enriched
```

### Comparing `xklb-2.2.8/xklb/consts.py` & `xklb-2.2.9/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/db.py` & `xklb-2.2.9/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/dl_config.py` & `xklb-2.2.9/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/dl_extract.py` & `xklb-2.2.9/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/fs_extract.py` & `xklb-2.2.9/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/gdl_backend.py` & `xklb-2.2.9/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/gdl_extract.py` & `xklb-2.2.9/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/gui.py` & `xklb-2.2.9/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/history.py` & `xklb-2.2.9/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/hn_extract.py` & `xklb-2.2.9/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/lb.py` & `xklb-2.2.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/media.py` & `xklb-2.2.9/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/play_actions.py` & `xklb-2.2.9/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/player.py` & `xklb-2.2.9/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/playlists.py` & `xklb-2.2.9/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/praw_extract.py` & `xklb-2.2.9/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/search.py` & `xklb-2.2.9/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/subtitle.py` & `xklb-2.2.9/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/tabs_actions.py` & `xklb-2.2.9/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/tabs_extract.py` & `xklb-2.2.9/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/tube_backend.py` & `xklb-2.2.9/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/tube_extract.py` & `xklb-2.2.9/xklb/tube_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
+    parser.add_argument("--no-optimize", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Fetch metadata for paths even if they are already in the media table",
     )
@@ -108,15 +109,15 @@
 
             tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
 
             if args.extra:
                 log.warning("[%s]: Getting extra metadata", path)
                 tube_backend.get_extra_metadata(args, path)
 
-    if not args.db["media"].detect_fts():
+    if not args.no_optimize and not args.db["media"].detect_fts():
         db.optimize(args)
 
 
 def tube_update(args=None) -> None:
     if args:
         sys.argv = ["tubeupdate", *args]
```

### Comparing `xklb-2.2.8/xklb/usage.py` & `xklb-2.2.9/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/utils.py` & `xklb-2.2.9/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/bigdirs.py` & `xklb-2.2.9/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/block.py` & `xklb-2.2.9/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/christen.py` & `xklb-2.2.9/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/cluster_sort.py` & `xklb-2.2.9/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/copy_play_counts.py` & `xklb-2.2.9/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/dedupe.py` & `xklb-2.2.9/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/dedupe_db.py` & `xklb-2.2.9/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/disk_usage.py` & `xklb-2.2.9/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/download_status.py` & `xklb-2.2.9/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/history.py` & `xklb-2.2.9/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/merge_dbs.py` & `xklb-2.2.9/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/merge_online_local.py` & `xklb-2.2.9/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/move_list.py` & `xklb-2.2.9/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/optimize_db.py` & `xklb-2.2.9/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/places_import.py` & `xklb-2.2.9/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/playback_control.py` & `xklb-2.2.9/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/playlists.py` & `xklb-2.2.9/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/redownload.py` & `xklb-2.2.9/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/relmv.py` & `xklb-2.2.9/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/scatter.py` & `xklb-2.2.9/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/streaming_tab_loader.py` & `xklb-2.2.9/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/mining/data.py` & `xklb-2.2.9/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/mining/extract_links.py` & `xklb-2.2.9/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.2.9/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/mining/nouns.py` & `xklb-2.2.9/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/mining/pushshift.py` & `xklb-2.2.9/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.2.9/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/xklb/assets/kotobago.png` & `xklb-2.2.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/.gitignore` & `xklb-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/LICENSE` & `xklb-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/README.md` & `xklb-2.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.2.008)
+    xk media library subcommands (v2.2.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-2.2.8/pyproject.toml` & `xklb-2.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.2.8/PKG-INFO` & `xklb-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.2.8
+Version: 2.2.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.2.008)
+    xk media library subcommands (v2.2.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

