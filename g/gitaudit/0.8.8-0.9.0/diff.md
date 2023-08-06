# Comparing `tmp/gitaudit-0.8.8.tar.gz` & `tmp/gitaudit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitaudit-0.8.8.tar", last modified: Wed Mar 15 20:38:43 2023, max compression
+gzip compressed data, was "gitaudit-0.9.0.tar", last modified: Sun Apr 16 21:15:50 2023, max compression
```

## Comparing `gitaudit-0.8.8.tar` & `gitaudit-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.165259 gitaudit-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-15 20:38:29.000000 gitaudit-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-15 20:38:43.161259 gitaudit-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-15 20:38:29.000000 gitaudit-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.157258 gitaudit-0.8.8/gitaudit/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-15 20:38:42.000000 gitaudit-0.8.8/gitaudit/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-15 20:38:42.000000 gitaudit-0.8.8/gitaudit/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.157258 gitaudit-0.8.8/gitaudit/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.157258 gitaudit-0.8.8/gitaudit/analysis/merge_debt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/merge_debt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/pruners.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/combined_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/css/adapted.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/macros/change_log_entry.html
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/match_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/prune_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/single_report.html
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/statistics_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/unmatched_table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/gitaudit/branch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/branch/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/branch/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/branch/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/branch/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/branch/tree_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/gitaudit/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/git/change_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/git/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/gitaudit/github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/github/graphql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/github/graphql_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-03-15 20:38:29.000000 gitaudit-0.8.8/gitaudit/github/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.157258 gitaudit-0.8.8/gitaudit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-15 20:38:43.000000 gitaudit-0.8.8/gitaudit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-15 20:38:43.000000 gitaudit-0.8.8/gitaudit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 20:38:43.000000 gitaudit-0.8.8/gitaudit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-15 20:38:43.000000 gitaudit-0.8.8/gitaudit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-15 20:38:43.000000 gitaudit-0.8.8/gitaudit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 20:38:43.165259 gitaudit-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-15 20:38:29.000000 gitaudit-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 20:38:43.161259 gitaudit-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-15 20:38:29.000000 gitaudit-0.8.8/tests/test_custom_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.024141 gitaudit-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 21:15:36.000000 gitaudit-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-16 21:15:50.024141 gitaudit-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 21:15:36.000000 gitaudit-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.016141 gitaudit-0.9.0/gitaudit/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 21:15:49.000000 gitaudit-0.9.0/gitaudit/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 21:15:49.000000 gitaudit-0.9.0/gitaudit/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.016141 gitaudit-0.9.0/gitaudit/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.016141 gitaudit-0.9.0/gitaudit/analysis/merge_diff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/merge_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/pruners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.020141 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/combined_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.020141 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/css/adapted.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.020141 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/macros/change_log_entry.html
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/match_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/prune_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/single_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/statistics_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/unmatched_table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.020141 gitaudit-0.9.0/gitaudit/analysis/sha_version_mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/sha_version_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/analysis/sha_version_mapper/sha_version_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.024141 gitaudit-0.9.0/gitaudit/branch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/branch/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/branch/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/branch/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/branch/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/branch/tree_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.024141 gitaudit-0.9.0/gitaudit/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/git/change_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/git/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.024141 gitaudit-0.9.0/gitaudit/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/github/graphql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/github/graphql_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-16 21:15:36.000000 gitaudit-0.9.0/gitaudit/github/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.016141 gitaudit-0.9.0/gitaudit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-16 21:15:50.000000 gitaudit-0.9.0/gitaudit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-16 21:15:50.000000 gitaudit-0.9.0/gitaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:15:50.000000 gitaudit-0.9.0/gitaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 21:15:50.000000 gitaudit-0.9.0/gitaudit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 21:15:50.000000 gitaudit-0.9.0/gitaudit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 21:15:50.024141 gitaudit-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-16 21:15:36.000000 gitaudit-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:15:50.024141 gitaudit-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 21:15:36.000000 gitaudit-0.9.0/tests/test_custom_assert.py
```

### Comparing `gitaudit-0.8.8/LICENSE` & `gitaudit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/buckets.py` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/buckets.py`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/matchers.py` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/matchers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Matchers for merge debt analysis
+"""Matchers for merge diff analysis
 """
 
 from typing import List
 from hashlib import sha1
 
 from pydantic import BaseModel
 
@@ -13,15 +13,15 @@
 class MatchResult(BaseModel):
     """Match Result consisting of head, base, and confidence entries
     """
     head: ChangeLogEntry
     base: ChangeLogEntry
 
 
-class Matcher:  # pylint: disable=too-few-public-methods
+class Matcher:
     """Generic class for matching commits
     """
 
     def match(self, head: List[BucketEntry], base: List[BucketEntry]) -> List[MatchResult]:
         """Match the bucket entries
 
         Args:
@@ -33,15 +33,15 @@
 
         Returns:
             List[MatchResult]: List of commit Matches
         """
         raise NotImplementedError
 
 
-class SameCommitMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class SameCommitMatcher(Matcher):
     """Accounts for branching strategies where dev and master branches are regularly cross merged.
 
     In very rare occasions it can happen that a feature branch was created before branch off
     and then can be merged into both branches that are to be matched with different merge commits.
 
     All matches will have an ABSOLUTE confidence level.
     """
@@ -67,15 +67,15 @@
                     head=head_entry,
                     base=entry_base_map[sha],
                 ))
 
         return matches
 
 
-class DirectCherryPickMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class DirectCherryPickMatcher(Matcher):
     """If a cherry pick was done with the -x option the commit message will have a
     (cherry picked from commit <sha>) message in the commit body. This sha can be used for matching.
 
     The cherry pick matcher will match in both directions (head <-> base) as it can happen that in a
     project the bugfix has to be done quickly in release and is then cherry picked to main later.
 
     All matches will have an ABSOLUTE confidence level.
@@ -133,15 +133,15 @@
                         head=entry_head_map[base_entry.cherry_pick_sha],
                         base=base_entry,
                     ))
 
         return matches
 
 
-class ThirdPartyCherryPickMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class ThirdPartyCherryPickMatcher(Matcher):
     """It can happen that a bug fix was created on master and then is cherry picked with -x option
     to release and hotfix branch. If a matching between release and hotfix is made the sha in the
     commit messase (cherry picked from commit <sha>) will point to a third party commit unrelated
     to the branches under comparison.
 
     All matches will have an ABSOLUTE confidence level.
     """
@@ -239,15 +239,15 @@
             continue
 
         numstat_map[stat_sha1] = entry
 
     return numstat_map
 
 
-class FilesChangedMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class FilesChangedMatcher(Matcher):
     """In case a cherry pick was NOT done with the -x option enabled an exact matching is not
     possible. But if a cherry pick was done successfully, the files changed in both commits shall
     be the exact same. Therefore, the changes files withing a commit can be used to determine
     if two commits are equal.
 
     All matches will have a STRONG confidence level. If there are multiple matches the additions and
     deletions will be used to filter false positives (note that additions and deletions check is
@@ -302,15 +302,15 @@
                 head=head_entry,
                 base=numstat_base_map[cp_sha],
             ))
 
         return matches
 
 
-class WhitelistMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class WhitelistMatcher(Matcher):
     """A whitelist can be provided from an outside data source to match head and base commits.
 
     All matches will have an ABSOLUTE confidene level.
     """
 
     def match(self, head: List[BucketEntry], base: List[BucketEntry]) -> List[MatchResult]:
         """Match the bucket entries
@@ -323,15 +323,15 @@
             NotImplementedError: Abstract Placeholder
 
         Returns:
             List[MatchResult]: List of commit Matches
         """
 
 
-class JiraIssueKeyMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class JiraIssueKeyMatcher(Matcher):
     """Based on the regular expression r'[\\w\\d]+-\\d+' which matches jira issue keys possible
     matches are determined. A custom regular expression can also be provided.
     A commit may contain multiple issue keys, also multiple matches are possible.
 
     All matches will have a GOOD confidence level. In case the additions and deletions
     are not matched the confidence level is dropped to LOW.
     """
@@ -347,15 +347,15 @@
             NotImplementedError: Abstract Placeholder
 
         Returns:
             List[MatchResult]: List of commit Matches
         """
 
 
-class SubjectMatcher(Matcher):  # pylint: disable=too-few-public-methods
+class SubjectMatcher(Matcher):
     """Based on the subject it is checked whether head subject is contained in base or vice versa.
 
     All matches will have a GOOD confidence level. In case the additions and deletions
     are not matched the confidence level is dropped to LOW.
     """
 
     def match(self, head: List[BucketEntry], base: List[BucketEntry]) -> List[MatchResult]:
```

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/merge_debt.py` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/merge_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     changelog_hydration, \
     log_commit_stats
 from gitaudit.git.controller import Git
 from gitaudit.branch.tree import Tree
 
 from .matchers import Matcher, MatchResult
 from .buckets import BucketList, get_entries_from_bucket_list
-from .report import MergeDebtReport, MergeDebtAlert, RefInfo
+from .report import MergeDiffReport, MergeDiffAlert, RefInfo
 from .pruners import Pruner
 
 
 def get_head_base_hier_logs(git: Git, head_ref: str, base_ref: str):
     """Gets the head and base hierarchy logs from a git instance
-    as preparation for the merge debt analysis
+    as preparation for the merge diff analysis
 
     Args:
         git (Git): Git instance
         head_ref (str): name of the head ref
         base_ref (str): name of the base ref
 
     Returns:
@@ -35,15 +35,15 @@
     base_hier_log = linear_log_to_hierarchy_log(git.log_parentlog(base_ref))
 
     tree = Tree()
     tree.append_log(base_hier_log, base_ref)
     tree.append_log(head_hier_log, head_ref)
 
     ref_segment_map = {
-        x.branch_name: x for x in tree.root.children.values()
+        x.ref_name: x for x in tree.root.children.values()
     }
 
     head_segment = ref_segment_map[head_ref]
     base_segment = ref_segment_map[base_ref]
 
     head_hier_log = changelog_hydration(
         head_segment.entries,
@@ -53,19 +53,19 @@
         base_segment.entries,
         git,
     )
 
     return head_hier_log, base_hier_log
 
 
-class MergeDebt:
-    """Calculates the merge debt by finding commits that are merged in head but not in base
+class MergeDiff:
+    """Calculates the merge diff by finding commits that are merged in head but not in base
     """
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         name,
         head_hier_log,
         base_hier_log,
         head_ref_name,
         base_ref_name,
     ) -> None:
@@ -76,15 +76,15 @@
         self.base_buckets = BucketList(self.base_hier_log)
 
         head_merge_count, head_normal_count, head_add, head_del = log_commit_stats(
             self.head_hier_log)
         base_merge_count, base_normal_count, base_add, base_del = log_commit_stats(
             self.base_hier_log)
 
-        self._report = MergeDebtReport(
+        self._report = MergeDiffReport(
             name=name,
             head_info=RefInfo(
                 ref_name=head_ref_name,
                 sha=self.head_hier_log[0].sha,
                 merge_commit_count=head_merge_count,
                 individual_commit_count=head_normal_count,
                 total_commit_count=head_merge_count+head_normal_count,
@@ -99,19 +99,19 @@
                 total_commit_count=base_merge_count+base_normal_count,
                 additions=base_add,
                 deletions=base_del,
             ),
         )
 
     @property
-    def report(self) -> MergeDebtReport:
-        """Returns the Merge Debt Report as Property
+    def report(self) -> MergeDiffReport:
+        """Returns the Merge diff Report as Property
 
         Returns:
-            MergeDebtReport: Merge Debt Report
+            MergeDiffReport: Merge diff Report
         """
         self._report.set_head_unmatched(
             get_entries_from_bucket_list(self.head_buckets.entries))
         self._report.set_base_unmatched(
             get_entries_from_bucket_list(self.base_buckets.entries))
         return self._report
 
@@ -137,15 +137,15 @@
         Args:
             match (MatchResult): Macth Result
 
         Returns:
             MatchResult: Augmented Match Result
         """
         if match.head.sorted_numstat != match.base.sorted_numstat:
-            self._report.append_alert(MergeDebtAlert.warning(
+            self._report.append_alert(MergeDiffAlert.warning(
                 match,
                 "Files changes / numstats do not match!",
             ))
 
         return match
 
     def execute_matcher(self, matcher: Matcher, prune=True):
@@ -208,34 +208,34 @@
         Args:
             pruner (Pruner): The pruner to select the entries to be removed
         """
         self.execute_head_pruner(pruner)
         self.execute_base_pruner(pruner)
 
     @classmethod
-    def from_tree(  # pylint: disable=too-many-arguments
+    def from_tree(
         cls,
         name: str,
         tree: Tree,
         head_ref: str,
         base_ref: str,
     ):
-        """Generate a merge debt instance by providing a tree object and the head and base ref
+        """Generate a merge diff instance by providing a tree object and the head and base ref
         names.
 
         Args:
             tree (Tree): Tree object the logs are taken from
             head_ref (str): head ref name
             base_ref (str): base ref name
 
         Returns:
-            MergeDebt: Merged Debt Instance
+            MergeDiff: Merged diff Instance
         """
         head_hier_log, base_hier_log = tree.get_entries_until_merge_base(
             head_ref, base_ref)
-        return MergeDebt(
+        return MergeDiff(
             name=name,
             head_hier_log=head_hier_log,
             base_hier_log=base_hier_log,
             head_ref_name=head_ref,
             base_ref_name=base_ref,
         )
```

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/pruners.py` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/pruners.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Callable
 import re
 
 from gitaudit.git.change_log_entry import ChangeLogEntry
 from .buckets import BucketEntry, get_sha_to_bucket_entry_map
 
 
-class Pruner:  # pylint: disable=too-few-public-methods
+class Pruner:
     """Generic class for pruning commits without matching
     """
 
     def prune(self, bucket_list: List[BucketEntry]) -> List[ChangeLogEntry]:
         """Prune bucket entries
 
         Args:
@@ -32,26 +32,26 @@
 
         return prune_results
 
     def _do_prune_entry(self, entry: ChangeLogEntry) -> bool:
         raise NotImplementedError
 
 
-class LambdaPruner(Pruner):  # pylint: disable=too-few-public-methods
+class LambdaPruner(Pruner):
     """Pruning based on user defined function"""
 
     def __init__(self, func: Callable) -> None:
         super().__init__()
         self.func = func
 
     def _do_prune_entry(self, entry: ChangeLogEntry) -> bool:
         return self.func(entry)
 
 
-class CommitSubjectBodyPruner(Pruner):  # pylint: disable=too-few-public-methods
+class CommitSubjectBodyPruner(Pruner):
     """Pruning based on subject / body content"""
 
     def __init__(self, pattern, invert: bool = False) -> None:
         super().__init__()
         self.pattern = pattern
         self.invert = invert
         self.regexp = re.compile(self.pattern)
@@ -59,15 +59,15 @@
     def _do_prune_entry(self, entry: ChangeLogEntry) -> bool:
         if self.invert:
             return not (self.regexp.search(entry.subject) or self.regexp.search(entry.body))
 
         return self.regexp.search(entry.subject) or self.regexp.search(entry.body)
 
 
-class CommitFilePathPruner(Pruner):  # pylint: disable=too-few-public-methods
+class CommitFilePathPruner(Pruner):
     """Pruning based on file path content. All file pathes must match the regexp."""
 
     def __init__(self, pattern) -> None:
         super().__init__()
         self.pattern = pattern
         self.regexp = re.compile(self.pattern)
```

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/report.py` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Reporting code for merge debt
+"""Reporting code for merge diff
 """
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import List, Tuple
 import os
@@ -11,77 +11,77 @@
 
 from pydantic import BaseModel, Field
 
 from gitaudit.git.change_log_entry import ChangeLogEntry
 from .matchers import MatchResult
 
 
-class MergeDebtReportAlertSeverity(Enum):
-    """Merge Debt Severity
+class MergeDiffReportAlertSeverity(Enum):
+    """Merge diff Severity
     """
     INFO = "INFO"
     WARNING = "WARNING"
     ERROR = "ERROR"
 
 
-class MergeDebtAlert(BaseModel):
-    """Merge Debt Report Alert
+class MergeDiffAlert(BaseModel):
+    """Merge diff Report Alert
     """
     match: MatchResult
-    severity: MergeDebtReportAlertSeverity
+    severity: MergeDiffReportAlertSeverity
     message: str
 
     @classmethod
     def info(cls, match, message):
-        """Create Info Merge Debt Report Alert
+        """Create Info Merge diff Report Alert
 
         Args:
             match (MatchResult): Match Result
             message (str): Message
 
         Returns:
-            MergeDebtAlert: Alert
+            MergeDiffAlert: Alert
         """
-        return MergeDebtAlert(
+        return MergeDiffAlert(
             match=match,
-            severity=MergeDebtReportAlertSeverity.INFO,
+            severity=MergeDiffReportAlertSeverity.INFO,
             message=message,
         )
 
     @classmethod
     def warning(cls, match, message):
-        """Create Warning Merge Debt Report Alert
+        """Create Warning Merge diff Report Alert
 
         Args:
             match (MatchResult): Match Result
             message (str): Message
 
         Returns:
-            MergeDebtAlert: Alert
+            MergeDiffAlert: Alert
         """
-        return MergeDebtAlert(
+        return MergeDiffAlert(
             match=match,
-            severity=MergeDebtReportAlertSeverity.WARNING,
+            severity=MergeDiffReportAlertSeverity.WARNING,
             message=message,
         )
 
     @classmethod
     def error(cls, match, message):
-        """Create Error Merge Debt Report Alert
+        """Create Error Merge diff Report Alert
 
         Args:
             match (MatchResult): Match Result
             message (str): Message
 
         Returns:
-            MergeDebtAlert: Alert
+            MergeDiffAlert: Alert
         """
-        return MergeDebtAlert(
+        return MergeDiffAlert(
             match=match,
-            severity=MergeDebtReportAlertSeverity.ERROR,
+            severity=MergeDiffReportAlertSeverity.ERROR,
             message=message,
         )
 
 
 class RefInfo(BaseModel):
     """Reference Info
     """
@@ -121,22 +121,22 @@
             individual_commit_count=individual_commit_count,
             total_commit_count=total_commit_count,
             additions=additions,
             deletions=deletions,
         )
 
 
-class MergeDebtReport(BaseModel):
+class MergeDiffReport(BaseModel):
     """Merge Report class
     """
     name: str
     head_info: RefInfo
     base_info: RefInfo
     matches: List[Tuple[str, List[MatchResult]]] = Field(default_factory=list)
-    alerts: List[MergeDebtAlert] = Field(default_factory=list)
+    alerts: List[MergeDiffAlert] = Field(default_factory=list)
     head_prunes: List[Tuple[str, List[ChangeLogEntry]]
                       ] = Field(default_factory=list)
     base_prunes: List[Tuple[str, List[ChangeLogEntry]]
                       ] = Field(default_factory=list)
     head_unmatched: List[ChangeLogEntry] = Field(default_factory=list)
     base_unmatched: List[ChangeLogEntry] = Field(default_factory=list)
 
@@ -162,19 +162,19 @@
         """Append match result to report
 
         Args:
             match (MatchResult): Match result to be added
         """
         self.matches.append((matcher_id, matches))
 
-    def append_alert(self, alert: MergeDebtAlert):
-        """Append merge debt report alert
+    def append_alert(self, alert: MergeDiffAlert):
+        """Append merge diff report alert
 
             Args:
-                alert (MergeDebtReportEntry): Merge Debt Report Alert
+                alert (MergeDiffReportEntry): Merge diff Report Alert
             """
         self.alerts.append(alert)
 
     def append_head_prune(self, pruner_id: str, entries: List[ChangeLogEntry]):
         """Append a head prune entry
         Args:
             entry (ChangeLogEntry): Pruned change log entry
@@ -231,22 +231,22 @@
         Args:
             file_path (str): File path for report to be save to
         """
         with open(file_path, 'w', encoding='utf-8') as file_p:
             file_p.write(self.render_to_text())
 
     @ classmethod
-    def combine(cls, arr: List[MergeDebtReport]) -> MergeDebtReport:
-        """Combine multiple merge debt reports into one
+    def combine(cls, arr: List[MergeDiffReport]) -> MergeDiffReport:
+        """Combine multiple merge diff reports into one
 
         Args:
-            arr (List[MergeDebtReport]): list of merge debt reports
+            arr (List[MergeDiffReport]): list of merge diff reports
 
         Returns:
-            MergeDebtReport: single merge debt report
+            MergeDiffReport: single merge diff report
         """
         head_info = RefInfo.combine(list(map(lambda x: x.head_info, arr)))
         base_info = RefInfo.combine(list(map(lambda x: x.base_info, arr)))
 
         matches = list(itertools.chain.from_iterable(
             map(lambda x: x.matches, arr)))
         alerts = list(itertools.chain.from_iterable(
@@ -256,45 +256,45 @@
         base_prunes = list(itertools.chain.from_iterable(
             map(lambda x: x.base_prunes, arr)))
         head_unmatched = list(itertools.chain.from_iterable(
             map(lambda x: x.head_unmatched, arr)))
         base_unmatched = list(itertools.chain.from_iterable(
             map(lambda x: x.base_unmatched, arr)))
 
-        return MergeDebtReport(
+        return MergeDiffReport(
             name="Combined",
             head_info=head_info,
             base_info=base_info,
             matches=matches,
             alerts=alerts,
             head_prunes=head_prunes,
             base_prunes=base_prunes,
             head_unmatched=head_unmatched,
             base_unmatched=base_unmatched,
         )
 
 
-def render_combined_report_to_text(reports: List[MergeDebtReport]) -> str:
+def render_combined_report_to_text(reports: List[MergeDiffReport]) -> str:
     """Render multiple reports to a single text report
 
     Returns:
         str: Html report as text
     """
-    combined = MergeDebtReport.combine(reports)
+    combined = MergeDiffReport.combine(reports)
 
     template_root = os.path.join(
         os.path.dirname(__file__), 'report_templates')
 
     template_loader = jinja2.FileSystemLoader(searchpath=template_root)
     template_env = jinja2.Environment(loader=template_loader)
     template = template_env.get_template("combined_report.html")
     return template.render(combined=combined, reports=reports)
 
 
-def render_combined_report_to_file(reports: List[MergeDebtReport], file_path: str) -> None:
+def render_combined_report_to_file(reports: List[MergeDiffReport], file_path: str) -> None:
     """Writemultiple reports as single html to file
 
     Args:
         file_path (str): File path for report to be save to
     """
     with open(file_path, 'w', encoding='utf-8') as file_p:
         file_p.write(render_combined_report_to_text(reports))
```

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/css/adapted.min.css` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/css/adapted.min.css`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/match_table.html` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/match_table.html`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/prune_table.html` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/prune_table.html`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/analysis/merge_debt/report_templates/statistics_table.html` & `gitaudit-0.9.0/gitaudit/analysis/merge_diff/report_templates/statistics_table.html`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/branch/hierarchy.py` & `gitaudit-0.9.0/gitaudit/branch/hierarchy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Analyse git logs to create hiearchy
 """
 
 
 from typing import List, Tuple
 from gitaudit.git.change_log_entry import ChangeLogEntry
+from gitaudit.git.controller import Git
 
 
 def take_first_parent_log(initial_sha, take_map):
     """Creates first parent log of git entries
 
     Args:
         initial_sha (str): start sha
@@ -70,14 +71,20 @@
 
     full_map = {x.sha: x for x in lin_log}
     take_map = {x.sha: x for x in lin_log}
 
     hie_log, take_map = _recursive_hierarchy_log(
         lin_log[0].sha, take_map, full_map)
 
+    # the last item of a hie_log (earliest item) should
+    # not have a branch_off. Either it is the initial commit
+    # or the log was stopped at some point meaning it
+    # is not a real branch off
+    hie_log[-1].branch_offs = []
+
     return hie_log
 
 
 def hierarchy_log_to_linear_log_entry(entry):
     """For a log entry remove hierarchy and return
     as linear log
 
@@ -111,15 +118,15 @@
 
     for entry in hier_log:
         lin_log.extend(hierarchy_log_to_linear_log_entry(entry))
 
     return lin_log
 
 
-def changelog_hydration(log, git, changelog_map=None):
+def changelog_hydration(log: List[ChangeLogEntry], git: Git, changelog_map=None, patch=True):
     """Hydrates a parent log with changelog entries
 
     Args:
         log (List[ChangeLogEntry]): Parent log
         git (Git): Git instance
         changelog_map (Dict[str, ChangeLogEntry], optional): Dictionary sha -> ChangeLogEntry.
             Defaults to None.
@@ -130,28 +137,35 @@
     if changelog_map is None:
         end_sha = log[0].sha
         start_sha_parent_sha = \
             log[-1].parent_shas[0] if log[-1].parent_shas else None
         changelog = git.log_changelog(
             end_ref=end_sha,
             start_ref=start_sha_parent_sha,
-            patch=True,
+            patch=patch,
         )
         changelog_map = {x.sha: x for x in changelog}
 
     for index, entry in enumerate(log):
         if entry.sha in changelog_map:
             changelog_entry = changelog_map[entry.sha]
         else:
-            changelog_entry = git.show_changelog_entry(entry.sha)
+            changelog_entry = git.show_changelog_entry(entry.sha, patch=patch)
 
         assert entry.sha == changelog_entry.sha
         assert entry.parent_shas == changelog_entry.parent_shas
 
-        log[index] = changelog_entry
+        update_dict = {key: val for key, val in changelog_entry if val}
+        curr_dict = {key: val for key, val in vars(entry).items() if val}
+
+        for key, val in curr_dict.items():
+            if key in update_dict:
+                assert val == update_dict[key], 'Hydration Update changes value in base element'
+
+        log[index] = log[index].copy(update=update_dict)
 
         for o_parent in entry.other_parents:
             changelog_entry.other_parents.append(changelog_hydration(
                 o_parent,
                 git,
                 changelog_map,
             ))
```

### Comparing `gitaudit-0.8.8/gitaudit/branch/plotting.py` & `gitaudit-0.9.0/gitaudit/branch/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 class TreeConnection:
     """Tree Connection
     """
     from_id: str
     to_id: str
 
 
-class TreeLane:  # pylint: disable=too-few-public-methods
+class TreeLane:
     """Tree Lane
     """
 
     def __init__(self, ref_name: str, xpos: float, extend_to_top: bool = True) -> None:
         self.ref_name = ref_name
         self.items = []
 
@@ -76,19 +76,19 @@
 
         Args:
             item (TreeLaneItem): New tree item
         """
         self.items.append(item)
 
 
-class TreePlot(Svg):  # pylint: disable=too-many-instance-attributes
+class TreePlot(Svg):
     """Class for plotting a branching tree
     """
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
             self,
             tree: Tree,
             active_refs: List[str] = None,
             ref_color_map: Dict[str, str] = None,
             graph_stroke_width_px: int = 1,
             column_spacing: float = 200.0,
             apply_linear_vert_pos_correction: bool = True,
@@ -104,15 +104,15 @@
         self.apply_linear_vert_pos_correction = apply_linear_vert_pos_correction
         self.directly_connected_to_root_refs = []
         self.column_spacing = column_spacing
         self.end_sha_seg_map = {
             seg.end_sha: seg for seg in self.tree.flatten_segments()
         }
         self.end_ref_name_seg_map = {
-            x.branch_name: x for x in self.tree.flatten_segments()}
+            x.ref_name: x for x in self.tree.flatten_segments()}
 
         self.show_commit_callback = show_commit_callback
         self.sha_svg_append_callback = sha_svg_append_callback
         self.ref_name_formatting_callback = ref_name_formatting_callback
 
         self.lanes: List[TreeLane] = []
         self.connections = []
@@ -133,49 +133,49 @@
     def _get_end_seg_counts(self) -> Dict[str, Tuple[int, int]]:
         """For the given tree return the segment / sha count from each end point to the root
 
         Returns:
             Dict[str, Tuple[int, int, int]]: second / Seg / sha count distance information
             from the root
         """
-        root_ref_name = self.tree.root.branch_name
+        root_ref_name = self.tree.root.ref_name
         assert root_ref_name in self.end_ref_name_seg_map
         root_end_segment = self.end_ref_name_seg_map[root_ref_name]
 
         ref_name_counts = {}
 
         for segment in self.end_ref_name_seg_map.values():
             curr_segment = segment
             seg_count = 1
             sha_count = curr_segment.length
             seconds_from_root_end = \
                 int((root_end_segment.end_entry.commit_date -
                      curr_segment.end_entry.commit_date).total_seconds())
 
             while curr_segment.end_sha != root_end_segment.end_sha:
-                if curr_segment.branch_name != root_ref_name:
+                if curr_segment.ref_name != root_ref_name:
                     # go down
                     curr_segment = self.end_sha_seg_map[curr_segment.start_entry.parent_shas[0]]
-                    if curr_segment.branch_name != root_ref_name:
+                    if curr_segment.ref_name != root_ref_name:
                         seg_count += 1
                         sha_count += curr_segment.length
                     else:
                         seconds_from_root_end = \
                             int((root_end_segment.end_entry.commit_date -
                                  curr_segment.end_entry.commit_date).total_seconds())
                 else:
                     curr_segment = list(filter(
-                        lambda x: x.branch_name == root_ref_name, curr_segment.children.values()
+                        lambda x: x.ref_name == root_ref_name, curr_segment.children.values()
                     ))[0]
                     seg_count += 1
                     sha_count += curr_segment.length
 
-            ref_name_counts[segment.branch_name] = (
+            ref_name_counts[segment.ref_name] = (
                 seconds_from_root_end,
-                segment.branch_name not in self.active_refs,
+                segment.ref_name not in self.active_refs,
                 seg_count,
                 -sha_count
             )
 
         return ref_name_counts
 
     def determine_ref_name_order(self) -> List[str]:
@@ -211,25 +211,25 @@
                 else:
                     # need to create new connection here
                     from_id = segment.start_entry.parent_shas[0]
                     self.connections.append(TreeConnection(
                         to_id=lane.items[-1].id,
                         from_id=from_id,
                     ))
-                    if self.end_sha_seg_map[from_id].branch_name == self.tree.root.branch_name:
+                    if self.end_sha_seg_map[from_id].ref_name == self.tree.root.ref_name:
                         self.directly_connected_to_root_refs.append(ref_name)
                     segment = None
             else:
                 segment = None
 
         return lane
 
     def _create_lanes(self) -> None:
         ref_order_names = self.determine_ref_name_order()
-        self.directly_connected_to_root_refs.append(self.tree.root.branch_name)
+        self.directly_connected_to_root_refs.append(self.tree.root.ref_name)
 
         for index, ref_name in enumerate(ref_order_names):
             lane = self._create_lane(ref_name, index * 300)
 
             for item in lane.items:
                 self.id_item_map[item.id] = item
                 self.id_lane_map[item.id] = lane
@@ -310,15 +310,15 @@
                 ),
             ))
 
             offset += bnds[3]-bnds[2] + 10
 
         return return_elems
 
-    def _calculate_positions(self):  # pylint: disable=too-many-locals
+    def _calculate_positions(self):
         lane_progess_map = {}
         lane_initial_datetime_map = {
             x.ref_name: x.items[0].date_time for x in self.lanes
         }
 
         curr_offset_date = max(lane_initial_datetime_map.values())
         curr_offset = 30
```

### Comparing `gitaudit-0.8.8/gitaudit/branch/serialization.py` & `gitaudit-0.9.0/gitaudit/branch/serialization.py`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/branch/tree.py` & `gitaudit-0.9.0/gitaudit/branch/tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class Segment(BaseModel):
     """Class for Storing a Branch Segment
     """
     entries: List[ChangeLogEntry]
     children: Optional[Dict[str, Segment]] = Field(default_factory=dict)
-    branch_name: Optional[str]
+    ref_name: Optional[str]
 
     @property
     def length(self):
         """Returns the number of entries in this segment
         """
         return len(self.entries)
 
@@ -54,24 +54,24 @@
 
 
 class Tree(BaseModel):
     """Branching tree out of segments
     """
     root: Segment = None
 
-    def append_log(self, hier_log: List[ChangeLogEntry], branch_name: str):
+    def append_log(self, hier_log: List[ChangeLogEntry], ref_name: str):
         """Append a new hierarchy log history to the tre
 
         Args:
             hier_log (List[ChangeLogEntry]): to be appended log
-            branch_name (str): name of the branch / ref
+            ref_name (str): name of the branch / ref
         """
         new_segment = Segment(
             entries=hier_log,
-            branch_name=branch_name,
+            ref_name=ref_name,
         )
 
         if not self.root:
             self.root = new_segment
         else:
             self._merge_segment(new_segment)
 
@@ -98,15 +98,15 @@
             elif len(current_segment.entries) <= (-index-1):
                 # the new segment exceeds the existing one
                 # --> replace the existing one with the new one
                 if current_segment.children:
                     # replace current segment
                     new_segment = Segment(
                         entries=new_segment.entries[:(index+1)],
-                        branch_name=new_segment.branch_name,
+                        ref_name=new_segment.ref_name,
                     )
 
                     if new_segment.start_sha in current_segment.children:
                         parent_segment = current_segment
                         current_segment = current_segment.children[new_segment.start_sha]
                         index = -1
                     else:
@@ -118,24 +118,24 @@
                         new_segment = None
                     else:
                         self.root = new_segment
                         new_segment = None
             else:
                 current_segment_pre = Segment(
                     entries=current_segment.entries[(index+1):],
-                    branch_name=current_segment.branch_name,
+                    ref_name=current_segment.ref_name,
                 )
                 current_segment_post = Segment(
                     entries=current_segment.entries[:(index+1)],
-                    branch_name=current_segment.branch_name,
+                    ref_name=current_segment.ref_name,
                     children=current_segment.children,
                 )
                 new_segment_post = Segment(
                     entries=new_segment.entries[:(index+1)],
-                    branch_name=new_segment.branch_name,
+                    ref_name=new_segment.ref_name,
                 )
 
                 current_segment_pre.children[current_segment_post.start_sha] = current_segment_post
                 current_segment_pre.children[new_segment_post.start_sha] = new_segment_post
 
                 if parent_segment:
                     parent_segment.children[current_segment_pre.start_sha] = current_segment_pre
@@ -169,84 +169,84 @@
         """Return a list of end segments
 
         Returns:
             List[Segment]: end segments
         """
         return list(filter(lambda x: not x.children, self.flatten_segments()))
 
-    def get_segment_trace(self, branch_name: str) -> List[Segment]:
+    def get_segment_trace(self, ref_name: str) -> List[Segment]:
         """Returns the segment trace from a branch name until the root segment (also including it)
 
         Args:
-            branch_name (str): The name of the end segment (branch name)
+            ref_name (str): The name of the end segment (branch name)
 
         Returns:
             List[Segment]: List of segments from end segment (first) to root (last)
         """
         end_sha_segments_map = {x.end_sha: x for x in self.flatten_segments()}
-        branch_name_end_segments_map = {
-            x.branch_name: x for x in self.end_segments()}
+        ref_name_end_segments_map = {
+            x.ref_name: x for x in self.end_segments()}
 
-        assert branch_name in branch_name_end_segments_map, \
-            f'Branch name "{branch_name}" is not used by any end segment!'
+        assert ref_name in ref_name_end_segments_map, \
+            f'Branch name "{ref_name}" is not used by any end segment!'
 
-        segments = [branch_name_end_segments_map[branch_name]]
+        segments = [ref_name_end_segments_map[ref_name]]
 
         while segments[-1].start_entry.parent_shas:
             fp_sha = segments[-1].start_entry.parent_shas[0]
             segments.append(end_sha_segments_map[fp_sha])
 
         return segments
 
     def get_segments_trace_until_merge_base(
         self,
-        head_branch_name: str,
-        base_branch_name: str,
+        head_ref_name: str,
+        base_ref_name: str,
     ) -> Tuple[List[Segment], List[Segment]]:
         """Gets the trace of two end refs (head and base) and returns the segments until the
         first combined segments (thus extracting the individual head and base segment traces).
 
         Args:
-            head_branch_name (str): The head branch name
-            base_branch_name (str): The base branch name
+            head_ref_name (str): The head branch name
+            base_ref_name (str): The base branch name
 
         Returns:
             Tuple[List[Segment], List[Segment]]: The individual segment lists (head, base)
         """
-        head_segments = self.get_segment_trace(head_branch_name)
-        base_segments = self.get_segment_trace(base_branch_name)
+        head_segments = self.get_segment_trace(head_ref_name)
+        base_segments = self.get_segment_trace(base_ref_name)
 
         index = -1
 
         while head_segments[index].end_sha == base_segments[index].end_sha:
             index -= 1
 
         index += 1
 
         return head_segments[:index], base_segments[:index]
 
     def get_entries_until_merge_base(
         self,
-        head_branch_name: str,
-        base_branch_name: str,
+        head_ref_name: str,
+        base_ref_name: str,
     ) -> Tuple[List[ChangeLogEntry], List[ChangeLogEntry]]:
         """Gets the change log of both branches until the
         first combined segments (thus extracting the individual head and base changelogs).
 
         Args:
-            head_branch_name (str): The head branch name
-            base_branch_name (str): The base branch name
+            head_ref_name (str): The head branch name
+            base_ref_name (str): The base branch name
 
         Returns:
             Tuple[List[ChangeLogEntry], List[ChangeLogEntry]]: The individual changelogs
                 (head, base)
         """
         head_segments, base_segments = self.get_segments_trace_until_merge_base(
-            head_branch_name,
-            base_branch_name,
+            head_ref_name,
+            base_ref_name,
         )
 
         head_entries_arr = map(lambda x: x.entries, head_segments)
         base_entries_arr = map(lambda x: x.entries, base_segments)
 
         head_entries = list(itertools.chain.from_iterable(head_entries_arr))
         base_entries = list(itertools.chain.from_iterable(base_entries_arr))
```

### Comparing `gitaudit-0.8.8/gitaudit/branch/tree_creator.py` & `gitaudit-0.9.0/gitaudit/branch/tree_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     root_ref: Optional[str] = None
 
 
 CACHE_PARENT_LOG_FOLDER_NAME = 'parent_log'
 CACHE_CHANGE_LOG_FOLDER_NAME = 'change_log'
 
 
-class TreeCreatorCache:  # pylint: disable=too-few-public-methods
+class TreeCreatorCache:
     """Tree Creator Cache
     """
 
     def __init__(self, root_location: str) -> None:
         self.root_location = root_location
         self.parent_log_location = os.path.join(
             self.root_location, CACHE_PARENT_LOG_FOLDER_NAME)
@@ -99,48 +99,59 @@
             patch=True,
         ))
         save_log_to_file(log, log_file_path)
 
         return log
 
 
-class TreeCreator:  # pylint: disable=too-few-public-methods
+class TreeCreator:
     """Tree Creator
     """
 
     def __init__(self, git: Git, config: TreeCreatorConfig, cache: TreeCreatorCache = None) -> None:
         self.git = git
         self.config = config
         self.cache = cache
 
     def _get_refs(self):
         refs = []
 
         refs.extend(filter(
             self.config.local_branch_filter_func,
-            self.git.local_branch_names(),
+            self.git.local_ref_names(),
         ))
         refs.extend(filter(
             self.config.remote_branch_filter_func,
-            self.git.remote_branch_names(),
+            self.git.remote_ref_names(),
         ))
         refs.extend(filter(
             self.config.tag_filter_func,
             self.git.tags(),
         ))
 
         return refs
 
     def create_tree(
         self,
         hydrate_with_changelog: bool = True,
         hydrate_root_segment: bool = False,
+        patch: bool = True,
     ) -> Tree:
         """Create the tree
 
+        Args:
+        hydrate_with_changelog (bool): Determines wether to hydrate the tree log (which initially
+            creates a parent log with the change log). Defaults to True.
+        hydrate_root_segment (bool): When hydrating the log by default the root segment is not
+            hydrated (due to performance reasons). The root segment can be hydrated by setting this
+            option to True. Defaults to False.
+        patch (bool): Wether or not the hydration shall be done with the patch option of git
+            enabled. If deactivated numstats and submodule updates cannot be determined and are thus
+            not part of the hydration. Defaults to True.
+
         Returns:
             Tree: Created Tree
         """
         refs = self._get_refs()
 
         if self.config.root_ref:
             assert self.config.root_ref in refs
@@ -155,10 +166,10 @@
 
         if not hydrate_with_changelog:
             return tree
 
         for seg in tree.iter_segments():
             if not hydrate_root_segment and seg.end_sha == tree.root.end_sha:
                 continue
-            changelog_hydration(seg.entries, self.git)
+            changelog_hydration(seg.entries, self.git, patch=patch)
 
         return tree
```

### Comparing `gitaudit-0.8.8/gitaudit/git/change_log_entry.py` & `gitaudit-0.9.0/gitaudit/git/change_log_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             )))
 
         if other_parents_dict:
             local_dict['other_parents'] = other_parents_dict
         return local_dict
 
     @classmethod
-    def from_log_text(cls, log_text, url_provider=None):  # pylint: disable=too-many-locals
+    def from_log_text(cls, log_text, url_provider=None):
         """Create ChangeLogEntry from logging text
 
         Args:
             log_text (str): Logging text
 
         Returns:
             ChangeLogEntry: Change log entry dataclass
```

### Comparing `gitaudit-0.8.8/gitaudit/git/controller.py` & `gitaudit-0.9.0/gitaudit/git/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,22 +165,22 @@
         args = ["checkout", "--no-recurse-submodules"]
 
         if create_branch:
             args.append("-b")
 
         self._execute_git_cmd(*args, ref)
 
-    def push(self, branch_name: str, remote="origin"):
+    def push(self, ref_name: str, remote="origin"):
         """Execute Git Push
 
         Args:
-            branch_name (str): Name of the branch
+            ref_name (str): Name of the branch
             remote (str, optional): Name of the remote. Defaults to "origin".
         """
-        self._execute_git_cmd("push", remote, f"{branch_name}:{branch_name}")
+        self._execute_git_cmd("push", remote, f"{ref_name}:{ref_name}")
 
     def add(self, path: str):
         """Execute git add
 
         Args:
             path (str): the path to the file to the staged (relative).
                 "." for all.
@@ -223,28 +223,28 @@
         """Returns remotes as list of strings
 
         Returns:
             List(str): Remotes of the repository
         """
         return self._execute_git_cmd_split_strip("remote")
 
-    def local_branch_names(self):
+    def local_ref_names(self):
         """Returns list of local branch names.
 
         Returns:
             List(str): List of locally checked out branches.
         """
         local_branches = self._execute_git_cmd_split_strip("branch")
         local_branches = list(
             map(lambda x: x.replace('* ', ''), local_branches))
         return local_branches
 
-    def remote_branch_names(self):
+    def remote_ref_names(self):
         """Returns list of remote branches including remote name
-        (e.g. <remote>/<branch_name>)
+        (e.g. <remote>/<ref_name>)
 
         Returns:
             List(str): List of branches across all remotes
         """
         remotes = self.remotes()
         remote_branches = self._execute_git_cmd_split_strip("branch", "-r")
 
@@ -262,15 +262,15 @@
         Returns:
             List(str): List of tags checked out locally
         """
         arr = self._execute_git_cmd_split_strip("tag", "-l")
         arr = list(filter(lambda x: x, arr))
         return arr
 
-    def log(  # pylint: disable=too-many-arguments
+    def log(
         self,
         pretty,
         end_ref, start_ref=None,
         first_parent=False,
         submodule=None,
         patch=False,
         other=None,
@@ -297,15 +297,15 @@
             start_ref=start_ref,
             first_parent=first_parent,
             submodule=submodule,
             patch=patch,
             other=other,
         ))
 
-    def _yield_line_log(  # pylint: disable=too-many-arguments
+    def _yield_line_log(
         self,
         pretty,
         end_ref, start_ref=None,
         first_parent=False,
         submodule=None,
         patch=False,
         other=None,
@@ -320,15 +320,15 @@
             f"{start_ref}...{end_ref}" if start_ref else end_ref,
         ] + (other if other else [])
         args = list(filter(lambda x: x is not None, args))
 
         for line in self._execute_git_cmd_yield(*args):
             yield line
 
-    def show(  # pylint: disable=too-many-arguments
+    def show(
         self,
         pretty,
         ref,
         submodule=None,
         patch=False,
         other=None,
     ):
```

### Comparing `gitaudit-0.8.8/gitaudit/github/graphql_objects.py` & `gitaudit-0.9.0/gitaudit/github/graphql_objects.py`

 * *Files identical despite different names*

### Comparing `gitaudit-0.8.8/gitaudit/github/instance.py` & `gitaudit-0.9.0/gitaudit/github/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 )
 
             results.extend(res['search']['nodes'])
             has_next_page = res['search']['pageInfo']['hasNextPage']
             end_cursor = res['search']['pageInfo']['endCursor']
         return list(map(PullRequest.parse_obj, results))
 
-    def create_pull_request(  # pylint: disable=too-many-arguments
+    def create_pull_request(
         self,
         repository_id: str,
         head_ref_name: str,
         base_ref_name: str,
         title: str,
         body: str = None,
         draft: bool = False,
@@ -267,21 +267,21 @@
 
     # def all_label_to_labelable(self, labelable_id, label_ids):
     #     raise NotImplementedError
 
     # def remove_label_from_labelable(self, labelable_id, label_ids):
     #     raise NotImplementedError
 
-    # def create_branch(self, owner, repo, base_oid, branch_name):
+    # def create_branch(self, owner, repo, base_oid, ref_name):
     #     raise NotImplementedError
 
     # def create_tag(self, owner, repo, base_oid, tag_name):
     #     raise NotImplementedError
 
-    # def create_commit_on_branch(self, owner, repo, branch_name, head_sha, message_headline,
+    # def create_commit_on_branch(self, owner, repo, ref_name, head_sha, message_headline,
     # message_body, additions, deletions):
     #     raise NotImplementedError
 
     # def unsure___(self):
     #     # get_file_commit_history
     #     # get_file_pull_request_history
     #     # get_submodules
```

### Comparing `gitaudit-0.8.8/gitaudit.egg-info/SOURCES.txt` & `gitaudit-0.9.0/gitaudit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 gitaudit/__init__.py
 gitaudit.egg-info/PKG-INFO
 gitaudit.egg-info/SOURCES.txt
 gitaudit.egg-info/dependency_links.txt
 gitaudit.egg-info/requires.txt
 gitaudit.egg-info/top_level.txt
 gitaudit/analysis/__init__.py
-gitaudit/analysis/merge_debt/__init__.py
-gitaudit/analysis/merge_debt/buckets.py
-gitaudit/analysis/merge_debt/matchers.py
-gitaudit/analysis/merge_debt/merge_debt.py
-gitaudit/analysis/merge_debt/pruners.py
-gitaudit/analysis/merge_debt/report.py
-gitaudit/analysis/merge_debt/report_templates/combined_report.html
-gitaudit/analysis/merge_debt/report_templates/match_table.html
-gitaudit/analysis/merge_debt/report_templates/prune_table.html
-gitaudit/analysis/merge_debt/report_templates/single_report.html
-gitaudit/analysis/merge_debt/report_templates/statistics_table.html
-gitaudit/analysis/merge_debt/report_templates/unmatched_table.html
-gitaudit/analysis/merge_debt/report_templates/css/adapted.min.css
-gitaudit/analysis/merge_debt/report_templates/macros/change_log_entry.html
+gitaudit/analysis/merge_diff/__init__.py
+gitaudit/analysis/merge_diff/buckets.py
+gitaudit/analysis/merge_diff/matchers.py
+gitaudit/analysis/merge_diff/merge_diff.py
+gitaudit/analysis/merge_diff/pruners.py
+gitaudit/analysis/merge_diff/report.py
+gitaudit/analysis/merge_diff/report_templates/combined_report.html
+gitaudit/analysis/merge_diff/report_templates/match_table.html
+gitaudit/analysis/merge_diff/report_templates/prune_table.html
+gitaudit/analysis/merge_diff/report_templates/single_report.html
+gitaudit/analysis/merge_diff/report_templates/statistics_table.html
+gitaudit/analysis/merge_diff/report_templates/unmatched_table.html
+gitaudit/analysis/merge_diff/report_templates/css/adapted.min.css
+gitaudit/analysis/merge_diff/report_templates/macros/change_log_entry.html
+gitaudit/analysis/sha_version_mapper/__init__.py
+gitaudit/analysis/sha_version_mapper/sha_version_mapper.py
 gitaudit/branch/__init__.py
 gitaudit/branch/hierarchy.py
 gitaudit/branch/plotting.py
 gitaudit/branch/serialization.py
 gitaudit/branch/tree.py
 gitaudit/branch/tree_creator.py
 gitaudit/git/__init__.py
```

### Comparing `gitaudit-0.8.8/setup.py` & `gitaudit-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,14 @@
     description="Analyse git repositories",
     long_description="Analyse git repositories",
     url="https://github.com/MatthiasRieck/gitaudit",
     packages=setuptools.find_packages(exclude=["tests*"]),
     package_data={"gitaudit": [
         "VERSION",
         "REQUIREMENTS",
-        "analysis/merge_debt/report_templates/*",
-        "analysis/merge_debt/report_templates/css/*",
-        "analysis/merge_debt/report_templates/macros/*",
+        "analysis/merge_diff/report_templates/*",
+        "analysis/merge_diff/report_templates/css/*",
+        "analysis/merge_diff/report_templates/macros/*",
     ]},
     include_package_data=True,
     install_requires=requires,  # determined by requirements.txt
 )
```

### Comparing `gitaudit-0.8.8/tests/test_custom_assert.py` & `gitaudit-0.9.0/tests/test_custom_assert.py`

 * *Files identical despite different names*

