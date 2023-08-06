# Comparing `tmp/perceval_mozilla-0.3.8rc2.tar.gz` & `tmp/perceval_mozilla-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_mozilla-0.3.8rc2.tar", max compression
+gzip compressed data, was "perceval_mozilla-0.3.9.tar", max compression
```

## Comparing `perceval_mozilla-0.3.8rc2.tar` & `perceval_mozilla-0.3.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      180 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/LICENSE
--rw-r--r--   0        0        0     1379 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/NEWS
--rw-r--r--   0        0        0     2373 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/README.md
--rw-r--r--   0        0        0        0 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/__init__.py
--rw-r--r--   0        0        0       91 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/_version.py
--rw-r--r--   0        0        0    10890 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/crates.py
--rw-r--r--   0        0        0    10821 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/kitsune.py
--rw-r--r--   0        0        0    11469 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/mozillaclub.py
--rw-r--r--   0        0        0    10907 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/remo.py
--rw-r--r--   0        0        0     1401 2023-04-21 09:53:17.006550 perceval_mozilla-0.3.8rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/__init__.py
--rw-r--r--   0        0        0     1889 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/base.py
--rw-r--r--   0        0        0        0 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/__init__.py
--rw-r--r--   0        0        0     1637 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_1
--rw-r--r--   0        0        0     2797 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_2
--rw-r--r--   0        0        0     1840 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_3
--rw-r--r--   0        0        0     6506 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_4
--rw-r--r--   0        0        0       19 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_team_1
--rw-r--r--   0        0        0      312 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_team_2
--rw-r--r--   0        0        0      295 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_team_3
--rw-r--r--   0        0        0      298 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_team_4
--rw-r--r--   0        0        0      324 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_1
--rw-r--r--   0        0        0      555 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_2
--rw-r--r--   0        0        0      555 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_3
--rw-r--r--   0        0        0      823 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_4
--rw-r--r--   0        0        0      369 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_version_downloads_1
--rw-r--r--   0        0        0        2 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_version_downloads_empty
--rw-r--r--   0        0        0      724 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_1
--rw-r--r--   0        0        0     3641 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_2
--rw-r--r--   0        0        0      748 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_3
--rw-r--r--   0        0        0     5010 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_4
--rw-r--r--   0        0        0     2181 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crates_page_1
--rw-r--r--   0        0        0     2352 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crates_page_2
--rw-r--r--   0        0        0       59 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crates_page_empty
--rw-r--r--   0        0        0    39923 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/crates/crates_summary
--rw-r--r--   0        0        0        0 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_answers_empty.json
--rw-r--r--   0        0        0     3693 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_question_answers.json
--rw-r--r--   0        0        0       78 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_question_answers_empy.json
--rw-r--r--   0        0        0     5730 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_questions_1_2.json
--rw-r--r--   0        0        0     8148 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_questions_2_2.json
--rw-r--r--   0        0        0       78 2023-04-21 09:53:17.010550 perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_questions_empty.json
--rw-r--r--   0        0        0  2047401 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/mozillaclub/feed.json
--rw-r--r--   0        0        0     1141 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities.json
--rw-r--r--   0        0        0     2893 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities_page_1_2.json
--rw-r--r--   0        0        0     2888 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities_page_2_2.json
--rw-r--r--   0        0        0       78 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities_page_empty.json
--rw-r--r--   0        0        0     1263 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events.json
--rw-r--r--   0        0        0     3463 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_1_2.json
--rw-r--r--   0        0        0     3784 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_2_2.json
--rw-r--r--   0        0        0      158 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_empty.json
--rw-r--r--   0        0        0     2904 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_page_1_2.json
--rw-r--r--   0        0        0     2889 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_page_2_2.json
--rw-r--r--   0        0        0       78 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_page_empty.json
--rw-r--r--   0        0        0    28055 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_reps.json
--rw-r--r--   0        0        0     2263 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users.json
--rw-r--r--   0        0        0     4143 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users_page_1_2.json
--rw-r--r--   0        0        0     4123 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users_page_2_2.json
--rw-r--r--   0        0        0       78 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users_page_empty.json
--rwxr-xr-x   0        0        0     1017 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/run_tests.py
--rw-r--r--   0        0        0    20404 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/test_crates.py
--rw-r--r--   0        0        0    14955 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/test_kitsune.py
--rw-r--r--   0        0        0    12118 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/test_mozillaclub.py
--rw-r--r--   0        0        0    17239 2023-04-21 09:53:17.014550 perceval_mozilla-0.3.8rc2/tests/test_remo.py
--rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 perceval_mozilla-0.3.8rc2/PKG-INFO
+-rw-r--r--   0        0        0      180 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1555 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/NEWS
+-rw-r--r--   0        0        0     2373 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/perceval/backends/mozilla/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/perceval/backends/mozilla/_version.py
+-rw-r--r--   0        0        0    10890 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/perceval/backends/mozilla/crates.py
+-rw-r--r--   0        0        0    10821 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/perceval/backends/mozilla/kitsune.py
+-rw-r--r--   0        0        0    11469 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/perceval/backends/mozilla/mozillaclub.py
+-rw-r--r--   0        0        0    10907 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/perceval/backends/mozilla/remo.py
+-rw-r--r--   0        0        0     1396 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0     1889 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/base.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/__init__.py
+-rw-r--r--   0        0        0     1637 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_example_1
+-rw-r--r--   0        0        0     2797 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_example_2
+-rw-r--r--   0        0        0     1840 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_example_3
+-rw-r--r--   0        0        0     6506 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_example_4
+-rw-r--r--   0        0        0       19 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_team_1
+-rw-r--r--   0        0        0      312 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_team_2
+-rw-r--r--   0        0        0      295 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_team_3
+-rw-r--r--   0        0        0      298 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_team_4
+-rw-r--r--   0        0        0      324 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_1
+-rw-r--r--   0        0        0      555 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_2
+-rw-r--r--   0        0        0      555 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_3
+-rw-r--r--   0        0        0      823 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_4
+-rw-r--r--   0        0        0      369 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_version_downloads_1
+-rw-r--r--   0        0        0        2 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_version_downloads_empty
+-rw-r--r--   0        0        0      724 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_versions_1
+-rw-r--r--   0        0        0     3641 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_versions_2
+-rw-r--r--   0        0        0      748 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_versions_3
+-rw-r--r--   0        0        0     5010 2023-04-26 14:45:52.062925 perceval_mozilla-0.3.9/tests/data/crates/crate_versions_4
+-rw-r--r--   0        0        0     2181 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/crates/crates_page_1
+-rw-r--r--   0        0        0     2352 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/crates/crates_page_2
+-rw-r--r--   0        0        0       59 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/crates/crates_page_empty
+-rw-r--r--   0        0        0    39923 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/crates/crates_summary
+-rw-r--r--   0        0        0        0 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_answers_empty.json
+-rw-r--r--   0        0        0     3693 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_question_answers.json
+-rw-r--r--   0        0        0       78 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_question_answers_empy.json
+-rw-r--r--   0        0        0     5730 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_questions_1_2.json
+-rw-r--r--   0        0        0     8148 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_questions_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-26 14:45:52.066925 perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_questions_empty.json
+-rw-r--r--   0        0        0  2047401 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/mozillaclub/feed.json
+-rw-r--r--   0        0        0     1141 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_activities.json
+-rw-r--r--   0        0        0     2893 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_activities_page_1_2.json
+-rw-r--r--   0        0        0     2888 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_activities_page_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_activities_page_empty.json
+-rw-r--r--   0        0        0     1263 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events.json
+-rw-r--r--   0        0        0     3463 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events_1_2.json
+-rw-r--r--   0        0        0     3784 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events_2_2.json
+-rw-r--r--   0        0        0      158 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events_empty.json
+-rw-r--r--   0        0        0     2904 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events_page_1_2.json
+-rw-r--r--   0        0        0     2889 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events_page_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_events_page_empty.json
+-rw-r--r--   0        0        0    28055 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_reps.json
+-rw-r--r--   0        0        0     2263 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_users.json
+-rw-r--r--   0        0        0     4143 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_users_page_1_2.json
+-rw-r--r--   0        0        0     4123 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_users_page_2_2.json
+-rw-r--r--   0        0        0       78 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/data/remo/remo_users_page_empty.json
+-rwxr-xr-x   0        0        0     1017 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/run_tests.py
+-rw-r--r--   0        0        0    20404 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/test_crates.py
+-rw-r--r--   0        0        0    14955 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/test_kitsune.py
+-rw-r--r--   0        0        0    12118 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/test_mozillaclub.py
+-rw-r--r--   0        0        0    17239 2023-04-26 14:45:52.070925 perceval_mozilla-0.3.9/tests/test_remo.py
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 perceval_mozilla-0.3.9/PKG-INFO
```

### Comparing `perceval_mozilla-0.3.8rc2/LICENSE` & `perceval_mozilla-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/NEWS` & `perceval_mozilla-0.3.9/NEWS`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+  ## perceval-mozilla 0.3.9 - (2023-04-26)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-mozilla 0.3.8 - (2023-04-21)
+  
+  * Update Poetry's package dependencies
+
   ## perceval-mozilla 0.3.7 - (2023-02-03)
   
   * Update Poetry's package dependencies
 
   ## perceval-mozilla 0.3.6 - (2023-02-01)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_mozilla-0.3.8rc2/README.md` & `perceval_mozilla-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/crates.py` & `perceval_mozilla-0.3.9/perceval/backends/mozilla/crates.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/kitsune.py` & `perceval_mozilla-0.3.9/perceval/backends/mozilla/kitsune.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/mozillaclub.py` & `perceval_mozilla-0.3.9/perceval/backends/mozilla/mozillaclub.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/perceval/backends/mozilla/remo.py` & `perceval_mozilla-0.3.9/perceval/backends/mozilla/remo.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/pyproject.toml` & `perceval_mozilla-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-mozilla"
-version = "0.3.8-rc.2"
+version = "0.3.9"
 description = "Bundle of Perceval backends for Mozilla ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_mozilla-0.3.8rc2/tests/base.py` & `perceval_mozilla-0.3.9/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_1` & `perceval_mozilla-0.3.9/tests/data/crates/crate_example_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_2` & `perceval_mozilla-0.3.9/tests/data/crates/crate_example_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_3` & `perceval_mozilla-0.3.9/tests/data/crates/crate_example_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_example_4` & `perceval_mozilla-0.3.9/tests/data/crates/crate_example_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_2` & `perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_3` & `perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_owner_user_4` & `perceval_mozilla-0.3.9/tests/data/crates/crate_owner_user_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_1` & `perceval_mozilla-0.3.9/tests/data/crates/crate_versions_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_2` & `perceval_mozilla-0.3.9/tests/data/crates/crate_versions_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_3` & `perceval_mozilla-0.3.9/tests/data/crates/crate_versions_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crate_versions_4` & `perceval_mozilla-0.3.9/tests/data/crates/crate_versions_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crates_page_1` & `perceval_mozilla-0.3.9/tests/data/crates/crates_page_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crates_page_2` & `perceval_mozilla-0.3.9/tests/data/crates/crates_page_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/crates/crates_summary` & `perceval_mozilla-0.3.9/tests/data/crates/crates_summary`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_question_answers.json` & `perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_question_answers.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_questions_1_2.json` & `perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_questions_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/kitsune/kitsune_questions_2_2.json` & `perceval_mozilla-0.3.9/tests/data/kitsune/kitsune_questions_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/mozillaclub/feed.json` & `perceval_mozilla-0.3.9/tests/data/mozillaclub/feed.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_activities.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities_page_1_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_activities_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_activities_page_2_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_activities_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_events.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_1_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_events_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_2_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_events_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_page_1_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_events_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_events_page_2_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_events_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_reps.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_reps.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_users.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users_page_1_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_users_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/data/remo/remo_users_page_2_2.json` & `perceval_mozilla-0.3.9/tests/data/remo/remo_users_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/run_tests.py` & `perceval_mozilla-0.3.9/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/test_crates.py` & `perceval_mozilla-0.3.9/tests/test_crates.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/test_kitsune.py` & `perceval_mozilla-0.3.9/tests/test_kitsune.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/test_mozillaclub.py` & `perceval_mozilla-0.3.9/tests/test_mozillaclub.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/tests/test_remo.py` & `perceval_mozilla-0.3.9/tests/test_remo.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-0.3.8rc2/PKG-INFO` & `perceval_mozilla-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-mozilla
-Version: 0.3.8rc2
+Version: 0.3.9
 Summary: Bundle of Perceval backends for Mozilla ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

