# Comparing `tmp/perceval-0.9.6.tar.gz` & `tmp/perceval-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/dist/perceval-0.9.6.tar", last modified: Mon Nov 27 11:04:12 2017, max compression
+gzip compressed data, was "/dist/perceval-0.9.9.tar", last modified: Fri Dec 29 08:20:30 2017, max compression
```

## Comparing `perceval-0.9.6.tar` & `perceval-0.9.9.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:12.000000 perceval-0.9.6/
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1317 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/SOURCES.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      122 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/requires.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        1 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/not-zip-safe
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12553 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/PKG-INFO
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        1 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/dependency_links.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        9 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval.egg-info/top_level.txt
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      198 2017-11-27 11:04:12.000000 perceval-0.9.6/setup.cfg
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:12.000000 perceval-0.9.6/bin/
--rwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)     6760 2017-11-27 11:04:11.000000 perceval-0.9.6/bin/perceval
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8368 2017-11-27 11:04:11.000000 perceval-0.9.6/README.md
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)       18 2017-11-27 11:04:11.000000 perceval-0.9.6/MANIFEST.in
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval/
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval/backends/
-drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:12.000000 perceval-0.9.6/perceval/backends/core/
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12206 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/jira.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    11366 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/telegram.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8132 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/jenkins.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    10350 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/stackexchange.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    24119 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/github.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    17964 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/askbot.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8934 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/nntp.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    16381 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/meetup.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    16077 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/bugzillarest.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    14403 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/slack.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12230 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/mbox.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     9512 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/pipermail.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     5299 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/rss.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12304 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/discourse.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    20955 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/launchpad.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     6849 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/dockerhub.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19360 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/bugzilla.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19641 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/phabricator.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    41459 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/git.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12352 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/gmane.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12906 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/supybot.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/__init__.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8867 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/hyperkitty.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    16070 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/gerrit.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    13068 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/confluence.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15344 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/redmine.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19299 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/core/mediawiki.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      879 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backends/__init__.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     4900 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/cache.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1969 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/errors.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15182 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/backend.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1011 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/__init__.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)       97 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/_version.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8300 2017-11-27 11:04:11.000000 perceval-0.9.6/perceval/utils.py
--rwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)     2981 2017-11-27 11:04:11.000000 perceval-0.9.6/setup.py
--rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12553 2017-11-27 11:04:12.000000 perceval-0.9.6/PKG-INFO
+drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/
+drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1336 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/SOURCES.txt
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      136 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/requires.txt
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        1 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/not-zip-safe
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12553 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/PKG-INFO
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        1 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/dependency_links.txt
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        9 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval.egg-info/top_level.txt
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      198 2017-12-29 08:20:30.000000 perceval-0.9.9/setup.cfg
+drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/bin/
+-rwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)     6760 2017-12-29 08:20:29.000000 perceval-0.9.9/bin/perceval
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8368 2017-12-29 08:20:29.000000 perceval-0.9.9/README.md
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)       18 2017-12-29 08:20:29.000000 perceval-0.9.9/MANIFEST.in
+drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval/
+drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval/backends/
+drwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:30.000000 perceval-0.9.9/perceval/backends/core/
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    11900 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/jira.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    11404 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/telegram.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     7596 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/jenkins.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    10128 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/stackexchange.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    23452 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/github.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    18036 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/askbot.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8934 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/nntp.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15295 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/meetup.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15954 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/bugzillarest.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    14437 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/slack.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12230 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/mbox.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     9512 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/pipermail.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     5138 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/rss.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12329 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/discourse.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    20426 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/launchpad.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     6530 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/dockerhub.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19036 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/bugzilla.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19391 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/phabricator.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    42297 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/git.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12352 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/gmane.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12906 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/supybot.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)        0 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/__init__.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8851 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/hyperkitty.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    16418 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/gerrit.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    13081 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/confluence.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15361 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/redmine.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    19277 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/core/mediawiki.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)      879 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backends/__init__.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     9373 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/client.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     4900 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/cache.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     2071 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/errors.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    15249 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/backend.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     1011 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/__init__.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)       97 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/_version.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)     8300 2017-12-29 08:20:29.000000 perceval-0.9.9/perceval/utils.py
+-rwxr-xr-x   0 grimoirelab  (1000) grimoirelab  (1000)     3008 2017-12-29 08:20:29.000000 perceval-0.9.9/setup.py
+-rw-r--r--   0 grimoirelab  (1000) grimoirelab  (1000)    12553 2017-12-29 08:20:30.000000 perceval-0.9.9/PKG-INFO
```

### Comparing `perceval-0.9.6/perceval.egg-info/SOURCES.txt` & `perceval-0.9.9/perceval.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.cfg
 setup.py
 bin/perceval
 perceval/__init__.py
 perceval/_version.py
 perceval/backend.py
 perceval/cache.py
+perceval/client.py
 perceval/errors.py
 perceval/utils.py
 perceval.egg-info/PKG-INFO
 perceval.egg-info/SOURCES.txt
 perceval.egg-info/dependency_links.txt
 perceval.egg-info/not-zip-safe
 perceval.egg-info/requires.txt
```

### Comparing `perceval-0.9.6/perceval.egg-info/PKG-INFO` & `perceval-0.9.9/perceval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: perceval
-Version: 0.9.6
+Version: 0.9.9
 Summary: Fetch data from software repositories
 Home-page: https://github.com/grimoirelab/perceval
 Author: Bitergia
 Author-email: sduenas@bitergia.com
 License: GPLv3
 Description-Content-Type: UNKNOWN
 Description: Perceval |Build Status| |Coverage Status| |PyPI version|
```

### Comparing `perceval-0.9.6/bin/perceval` & `perceval-0.9.9/bin/perceval`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/README.md` & `perceval-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/backends/core/jira.py` & `perceval-0.9.9/perceval/backends/core/jira.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 MAX_ISSUES = 100  # Maximum number of issues per query
 
 logger = logging.getLogger(__name__)
@@ -92,15 +93,15 @@
     :param user: Jira user
     :param password: Jira user password
     :param verify: allows to disable SSL verification
     :param cert: SSL certificate path (PEM)
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.7.1'
+    version = '0.8.0'
 
     def __init__(self, url, project=None,
                  user=None, password=None,
                  verify=None, cert=None,
                  max_issues=None, tag=None, cache=None):
         origin = url
 
@@ -231,15 +232,15 @@
         """
         raw_issues = json.loads(raw_page)
         issues = raw_issues['issues']
         for issue in issues:
             yield issue
 
 
-class JiraClient:
+class JiraClient(HttpClient):
     """JIRA API client.
 
     This class implements a simple client to retrieve issues from
     any JIRA issue tracking system.
 
     :param URL: URL of the JIRA server
     :param project: filter issues by project
@@ -253,26 +254,23 @@
     """
 
     EXPAND = 'renderedFields,transitions,operations,changelog'
     VERSION_API = '2'
     RESOURCE = 'rest/api'
 
     def __init__(self, url, project, user, password, verify, cert, max_issues):
-        self.url = url
+        super().__init__(url)
         self.project = project
         self.user = user
         self.password = password
         self.verify = verify
         self.cert = cert
         self.max_issues = max_issues
 
-    def __build_base_url(self, type='search'):
-        base_api_url = self.url
-        base_api_url = urijoin(base_api_url, self.RESOURCE, self.VERSION_API, type)
-        return base_api_url
+        self.__init_session()
 
     def __build_jql_query(self, from_date):
         AND_OP = 'AND'
         UPDATED_OP = 'updated >'
         PROJECT_OP = 'project ='
         ORDER_BY_OP = 'order by'
         ASC_OP = 'asc'
@@ -305,67 +303,60 @@
             nissues = min(max_issues, total)
             logger.info("Fetching issues: %s/%s" % (nissues,
                                                     total))
         else:
             logger.info("No issues were found.")
 
     def __init_session(self):
-        session = requests.Session()
-
         if (self.user and self.password) is not None:
-            session.auth = (self.user, self.password)
+            self.session.auth = (self.user, self.password)
 
         if self.cert:
-            session.cert = self.cert
+            self.session.cert = self.cert
 
         if self.verify is not True:
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
-            session.verify = False
-
-        return session
+            self.session.verify = False
 
     def get_issues(self, from_date):
         """Retrieve all the issues from a given date.
 
         :param from_date: obtain issues updated since this date
         """
-        session = self.__init_session()
-
         start_at = 0
-        req = session.get(self.__build_base_url(),
-                          params=self.__build_payload(start_at, from_date))
-        req.raise_for_status()
+
+        url = urijoin(self.base_url, self.RESOURCE, self.VERSION_API, 'search')
+        req = self.fetch(url, payload=self.__build_payload(start_at, from_date))
         issues = req.text
 
         data = req.json()
         tissues = data['total']
         nissues = data['maxResults']
 
         start_at += min(nissues, tissues)
         self.__log_status(start_at, tissues)
 
         while issues:
             yield issues
             issues = None
 
             if data['startAt'] + nissues < tissues:
-                req = session.get(self.__build_base_url(),
-                                  params=self.__build_payload(start_at, from_date))
-                req.raise_for_status()
+                req = self.fetch(url, payload=self.__build_payload(start_at, from_date))
+
                 data = req.json()
                 start_at += nissues
                 issues = req.text
                 self.__log_status(start_at, tissues)
 
     def get_fields(self):
-        """Retrieve all the fields available.  """
-        session = self.__init_session()
+        """Retrieve all the fields available."""
+
+        url = urijoin(self.base_url, self.RESOURCE, self.VERSION_API, 'field')
+        req = self.fetch(url)
 
-        req = session.get(self.__build_base_url('field'))
-        req.raise_for_status()
         return req.text
 
 
 class JiraCommand(BackendCommand):
     """Class to run Jira backend from the command line."""
 
     BACKEND = Jira
```

### Comparing `perceval-0.9.6/perceval/backends/core/telegram.py` & `perceval-0.9.9/perceval/backends/core/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import functools
 import json
 import logging
 
-import requests
-
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 
 
 logger = logging.getLogger(__name__)
 
 
 TELEGRAM_URL = 'https://telegram.org'
@@ -77,15 +76,15 @@
     of the bot; i.e 'http://telegram.org/mybot'.
 
     :param bot: name of the bot
     :param bot_token: authentication token used by the bot
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.1'
+    version = '0.6.0'
 
     def __init__(self, bot, bot_token, tag=None, cache=None):
         origin = urijoin(TELEGRAM_URL, bot)
 
         super().__init__(origin, tag=tag, cache=cache)
         self.bot = bot
         self.client = TelegramBotClient(bot_token)
@@ -303,29 +302,30 @@
         # Required arguments
         parser.parser.add_argument('bot',
                                    help="Name of the bot")
 
         return parser
 
 
-class TelegramBotClient:
+class TelegramBotClient(HttpClient):
     """Telegram Bot API 2.0 client.
 
     This class implements a simple client to retrieve those messages
     sent to a Telegram bot. This includes personal messages or
     messages sent to a channel (when privacy settings are disabled).
 
     :param bot_token: token for the bot
     """
     API_URL = "https://api.telegram.org/bot%(token)s/%(method)s"
 
     UPDATES_METHOD = 'getUpdates'
     OFFSET = 'offset'
 
     def __init__(self, bot_token):
+        super().__init__(self.API_URL)
         self.bot_token = bot_token
 
     def updates(self, offset=None):
         """Fetch the messages that a bot can read.
 
         When the `offset` is given it will retrieve all the messages
         that are greater or equal to that offset. Take into account
@@ -346,16 +346,15 @@
     def _call(self, method, params):
         """Retrive the given resource.
 
         :param resource: resource to retrieve
         :param params: dict with the HTTP parameters needed to retrieve
             the given resource
         """
-        url = self.API_URL % {'token': self.bot_token, 'method': method}
+        url = self.base_url % {'token': self.bot_token, 'method': method}
 
         logger.debug("Telegram bot calls method: %s params: %s",
                      method, str(params))
 
-        r = requests.get(url, params=params)
-        r.raise_for_status()
+        r = self.fetch(url, payload=params)
 
         return r.text
```

### Comparing `perceval-0.9.6/perceval/backends/core/jenkins.py` & `perceval-0.9.9/perceval/backends/core/jenkins.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 #
 # Authors:
 #     Alvaro del Castillo <acs@bitergia.com>
 #
 
 import json
 import logging
-import time
 
 import requests
 
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 
 
 logger = logging.getLogger(__name__)
 
 
 SLEEP_TIME = 10
@@ -50,15 +50,15 @@
 
     :param url: Jenkins url
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     :param blacklist_jobs: exclude the jobs of this list while fetching
     :param sleep_time: minimun waiting time due to a timeout connection exception
     """
-    version = '0.5.3'
+    version = '0.6.1'
 
     def __init__(self, url, tag=None, cache=None, blacklist_jobs=None, sleep_time=SLEEP_TIME):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
         self.client = JenkinsClient(url, blacklist_jobs, sleep_time)
@@ -180,74 +180,51 @@
 
         This backend only generates one type of item which is
         'build'.
         """
         return 'build'
 
 
-class JenkinsClient:
+class JenkinsClient(HttpClient):
     """Jenkins API client.
 
     This class implements a simple client to retrieve builds from
     projects in a Jenkins node.
 
     :param url: URL of jenkins node: https://build.opnfv.org/ci
 
     :raises HTTPError: when an error occurs doing the request
     """
     MAX_RETRIES = 5
 
     def __init__(self, url, blacklist_jobs=None, sleep_time=SLEEP_TIME):
-        self.url = url
+        super().__init__(url, default_sleep_time=sleep_time, extra_status_forcelist=[410, 502, 503])
         self.blacklist_jobs = blacklist_jobs
-        self.sleep_time = sleep_time
 
     def get_jobs(self):
         """ Retrieve all jobs
         """
-        url_jenkins = urijoin(self.url, "/api/json")
+        url_jenkins = urijoin(self.base_url, "api", "json")
 
-        return self.__send_request(url_jenkins)
+        response = self.fetch(url_jenkins)
+        return response.text
 
     def get_builds(self, job_name):
         """ Retrieve all builds from a job
         """
 
         if self.blacklist_jobs and job_name in self.blacklist_jobs:
             logging.info("Not getting blacklisted job: %s", job_name)
             return
 
         # depth=2 to get builds details
-        job_url = self.url + "/job/%s/" % (job_name)
-        url_jenkins = job_url + "api/json?depth=2"
-
-        return self.__send_request(url_jenkins)
-
-    def __send_request(self, url):
-        """send HTTP requests to the server"""
-
-        retries = 0
-
-        while retries < self.MAX_RETRIES:
-
-            try:
-                req = requests.get(url)
-                req.raise_for_status()
-                break
-            except requests.exceptions.RequestException as e:
-                if e.response.status_code in [408, 410, 502, 503, 504]:
-                    retries += 1
-                    time.sleep(self.sleep_time * retries)
-                else:
-                    raise e
-
-        if retries == self.MAX_RETRIES:
-            req.raise_for_status()
+        url_build = urijoin(self.base_url, "job", job_name, "api", "json?depth=2")
 
-        return req.text
+        response = self.fetch(url_build)
+        return response.text
 
 
 class JenkinsCommand(BackendCommand):
     """Class to run Jenkins backend from the command line."""
 
     BACKEND = Jenkins
```

### Comparing `perceval-0.9.6/perceval/backends/core/stackexchange.py` & `perceval-0.9.9/perceval/backends/core/stackexchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,22 @@
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import json
 import logging
 import time
 
-import requests
-
 from grimoirelab.toolkit.datetime import datetime_to_utc
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 MAX_QUESTIONS = 100  # Maximum number of reviews per query
 
 logger = logging.getLogger(__name__)
@@ -52,15 +51,15 @@
 
     :param site: StackExchange site
     :param tagged: filter items by question Tag
     :param api_token: StackExchange access_token for the API
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.6.1'
+    version = '0.7.0'
 
     def __init__(self, site, tagged=None, api_token=None,
                  max_questions=None, tag=None, cache=None):
         origin = site
 
         super().__init__(origin, tag=tag, cache=cache)
         self.site = site
@@ -175,15 +174,15 @@
         """
         raw_questions = json.loads(raw_page)
         questions = raw_questions['items']
         for question in questions:
             yield question
 
 
-class StackExchangeClient:
+class StackExchangeClient(HttpClient):
     """StackExchange API client.
 
     This class implements a simple client to retrieve questions from
     any Stackexchange site.
 
     :param site: URL of the Bugzilla server
     :param tagged: filter items by question Tag
@@ -199,24 +198,20 @@
     # values for the filter provided.
 
     QUESTIONS_FILTER = 'Bf*y*ByQD_upZqozgU6lXL_62USGOoV3)MFNgiHqHpmO_Y-jHR'
     STACKEXCHANGE_API_URL = 'https://api.stackexchange.com'
     VERSION_API = '2.2'
 
     def __init__(self, site, tagged, token, max_questions):
+        super().__init__(self.STACKEXCHANGE_API_URL)
         self.site = site
         self.tagged = tagged
         self.token = token
         self.max_questions = max_questions
 
-    def __build_base_url(self, type='questions'):
-        base_api_url = self.STACKEXCHANGE_API_URL
-        base_api_url = urijoin(base_api_url, self.VERSION_API, type)
-        return base_api_url
-
     def __build_payload(self, page, from_date, order='desc', sort='activity'):
         payload = {'page': page,
                    'pagesize': self.max_questions,
                    'order': order,
                    'sort': sort,
                    'tagged': self.tagged,
                    'site': self.site,
@@ -241,17 +236,17 @@
     def get_questions(self, from_date):
         """Retrieve all the questions from a given date.
 
         :param from_date: obtain questions updated since this date
         """
 
         page = 1
-        req = requests.get(self.__build_base_url(),
-                           params=self.__build_payload(page, from_date))
-        req.raise_for_status()
+        url = urijoin(self.base_url, self.VERSION_API, "questions")
+
+        req = self.fetch(url, payload=self.__build_payload(page, from_date))
         questions = req.text
 
         data = req.json()
         tquestions = data['total']
         nquestions = data['page_size']
 
         self.__log_status(data['quota_remaining'],
@@ -268,17 +263,15 @@
 
                 backoff = data.get('backoff', None)
                 if backoff:
                     logger.debug("Expensive query. Wait %s secs to send a new request",
                                  backoff)
                     time.sleep(float(backoff))
 
-                req = requests.get(self.__build_base_url(),
-                                   params=self.__build_payload(page, from_date))
-                req.raise_for_status()
+                req = self.fetch(url, payload=self.__build_payload(page, from_date))
                 data = req.json()
                 questions = req.text
                 nquestions += data['page_size']
                 self.__log_status(data['quota_remaining'],
                                   data['quota_max'],
                                   nquestions,
                                   tquestions)
```

### Comparing `perceval-0.9.6/perceval/backends/core/github.py` & `perceval-0.9.9/perceval/backends/core/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,30 @@
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
-from ...errors import CacheError, RateLimitError
+from ...client import HttpClient, RateLimitHandler
+from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 GITHUB_URL = "https://github.com/"
 GITHUB_API_URL = "https://api.github.com"
 
 # Range before sleeping until rate limit reset
 MIN_RATE_LIMIT = 10
 MAX_RATE_LIMIT = 500
 
+# Default sleep time and retries to deal with connection/server problems
+DEFAULT_SLEEP_TIME = 1
+MAX_RETRIES = 5
+
 TARGET_ISSUE_FIELDS = ['user', 'assignee', 'assignees', 'comments', 'reactions']
 
 logger = logging.getLogger(__name__)
 
 
 class GitHub(Backend):
     """GitHub backend for Perceval.
@@ -65,29 +70,31 @@
         from the GitHub public site.
     :param tag: label used to mark the data
     :param cache: use issues already retrieved in cache
     :param sleep_for_rate: sleep until rate limit is reset
     :param min_rate_to_sleep: minimun rate needed to sleep until
          it will be reset
     """
-    version = '0.11.2'
+    version = '0.12.1'
 
     def __init__(self, owner=None, repository=None,
                  api_token=None, base_url=None,
                  tag=None, cache=None,
-                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT):
+                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
+                 max_retries=MAX_RETRIES, default_sleep_time=DEFAULT_SLEEP_TIME):
         origin = base_url if base_url else GITHUB_URL
         origin = urijoin(origin, owner, repository)
 
         super().__init__(origin, tag=tag, cache=cache)
         self.owner = owner
         self.repository = repository
         self.api_token = api_token
         self.client = GitHubClient(owner, repository, api_token, base_url,
-                                   sleep_for_rate, min_rate_to_sleep)
+                                   sleep_for_rate, min_rate_to_sleep,
+                                   max_retries, default_sleep_time)
         self._users = {}  # internal users cache
 
     @classmethod
     def has_caching(cls):
         """Returns whether it supports caching items on the fetch process.
 
         :returns: this backend supports items cache
@@ -146,15 +153,15 @@
         :returns: a generator of issues
         """
 
         self._purge_cache_queue()
 
         from_date = datetime_to_utc(from_date)
 
-        issues_groups = self.client.issues(start=from_date)
+        issues_groups = self.client.issues(from_date=from_date)
 
         for raw_issues in issues_groups:
             self._push_cache_queue('{ISSUES}')
             self._push_cache_queue(raw_issues)
             self._flush_cache_queue()
             issues = json.loads(raw_issues)
             for issue in issues:
@@ -446,214 +453,198 @@
             user['organizations'] = json.loads(raw_org)
             self._users.update({login: user})
             found = self._users.get(login)
 
         return found
 
 
-class GitHubClient:
+class GitHubClient(HttpClient, RateLimitHandler):
     """Client for retieving information from GitHub API"""
 
-    MAX_RETRIES = 5
     _users = {}       # users cache
     _users_orgs = {}  # users orgs cache
 
     def __init__(self, owner, repository, token, base_url=None,
-                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT):
+                 sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
+                 default_sleep_time=DEFAULT_SLEEP_TIME, max_retries=MAX_RETRIES):
         self.owner = owner
         self.repository = repository
         self.token = token
-        self.rate_limit = None
-        self.rate_limit_reset_ts = None
-        self.sleep_for_rate = sleep_for_rate
 
         if base_url:
-            self.api_url = urijoin(base_url, 'api', 'v3')
+            base_url = urijoin(base_url, 'api', 'v3')
         else:
-            self.api_url = GITHUB_API_URL
+            base_url = GITHUB_API_URL
+
+        super().__init__(base_url, default_sleep_time=default_sleep_time, max_retries=max_retries,
+                         extra_headers=self._set_extra_headers())
+        super().setup_rate_limit_handler(sleep_for_rate=sleep_for_rate, min_rate_to_sleep=min_rate_to_sleep)
+
+        self._init_rate_limit()
+
+    def _set_extra_headers(self):
+        """Set extra headers for session"""
+
+        headers = {}
+        headers.update({'Accept': 'application/vnd.github.squirrel-girl-preview'})
+
+        if self.token:
+            headers.update({'Authorization': 'token ' + self.token})
+
+        return headers
 
-        if min_rate_to_sleep > MAX_RATE_LIMIT:
-            msg = "Minimum rate to sleep value exceeded (%d)."
-            msg += "High values might cause the client to sleep forever."
-            msg += "Reset to %d."
-            logger.warning(msg, min_rate_to_sleep, MAX_RATE_LIMIT)
+    def _init_rate_limit(self):
+        """Initialize rate limit information"""
 
-        self.min_rate_to_sleep = min(min_rate_to_sleep, MAX_RATE_LIMIT)
+        url = urijoin(self.base_url, "rate_limit")
+        try:
+            response = super().fetch(url)
+            self.update_rate_limit(response)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code == 404:
+                logger.warning("Rate limit not initialized: %s", error)
+            else:
+                raise error
+
+    def calculate_time_to_reset(self):
+        """Calculate the seconds to reset the token requests, by obtaining the different
+        between the current date and the next date when the token is fully regenerated.
+        """
+
+        return self.rate_limit_reset_ts - (int(time.time()) + 1)
 
     def issue_reactions(self, issue_number):
         """Get reactions of an issue"""
 
-        return self._fetch_items("/issues/" + str(issue_number) + "/reactions", "comment")
+        payload = {
+            'per_page': 30,
+            'direction': 'asc',
+            'sort': 'updated'
+        }
+
+        path = urijoin("issues", str(issue_number), "reactions")
+        return self.fetch_items(path, payload)
 
     def issue_comment_reactions(self, comment_id):
         """Get reactions of an issue comment"""
 
-        return self._fetch_items("/issues/comments/" + str(comment_id) + "/reactions", "comment")
+        payload = {
+            'per_page': 30,
+            'direction': 'asc',
+            'sort': 'updated'
+        }
+
+        path = urijoin("issues", "comments", str(comment_id), "reactions")
+        return self.fetch_items(path, payload)
 
     def issue_comments(self, issue_number):
         """Get the issue comments from pagination"""
 
-        return self._fetch_items("/issues/" + str(issue_number) + "/comments", "comment")
+        payload = {
+            'per_page': 30,
+            'direction': 'asc',
+            'sort': 'updated'
+        }
+
+        path = urijoin("issues", str(issue_number), "comments")
+        return self.fetch_items(path, payload)
 
-    def issues(self, start=None):
+    def issues(self, from_date=None):
         """Get the issues from pagination"""
 
-        return self._fetch_items("/issues", payload_type="issue", start=start)
+        payload = {
+            'state': 'all',
+            'per_page': 30,
+            'direction': 'asc',
+            'sort': 'updated'}
+
+        if from_date:
+            payload['since'] = from_date.isoformat()
+
+        path = urijoin("issues")
+        return self.fetch_items(path, payload)
 
     def user(self, login):
         """Get the user information and update the user cache"""
 
         user = None
 
         if login in self._users:
             return self._users[login]
 
-        url_user = urijoin(self.api_url, 'users', login)
+        url_user = urijoin(self.base_url, 'users', login)
 
         logging.info("Getting info for %s" % (url_user))
-        r = self.__send_request(url_user, headers=self.__build_headers())
+
+        r = self.fetch(url_user)
         user = r.text
         self._users[login] = user
 
         return user
 
     def user_orgs(self, login):
         """Get the user public organizations"""
 
         if login in self._users_orgs:
             return self._users_orgs[login]
 
-        url = urijoin(self.api_url, 'users', login, 'orgs')
+        url = urijoin(self.base_url, 'users', login, 'orgs')
         try:
-            r = self.__send_request(url, headers=self.__build_headers())
+            r = self.fetch(url)
             orgs = r.text
-        except requests.exceptions.HTTPError as ex:
+        except requests.exceptions.HTTPError as error:
             # 404 not found is wrongly received sometimes
-            if ex.response.status_code == 404:
-                logger.error("Can't get github login orgs: %s", ex)
+            if error.response.status_code == 404:
+                logger.error("Can't get github login orgs: %s", error)
                 orgs = '[]'
             else:
-                raise ex
+                raise error
 
         self._users_orgs[login] = orgs
 
         return orgs
 
-    def __get_url_repo(self):
-        """Build URL repo"""
-
-        github_api_repos = urijoin(self.api_url, 'repos')
-        url_repo = urijoin(github_api_repos, self.owner, self.repository)
-        return url_repo
-
-    def __get_url(self, path, startdate=None):
-        """Build repo-"related URL"""
-
-        url = self.__get_url_repo() + path
-        return url
-
-    def __build_payload(self, payload_type='issue', startdate=None):
-        """Build payload"""
-
-        # 100 in other items. 20 for pull requests. 30 issues
-        payload = {'per_page': 30,
-                   'direction': 'asc'}
-        if payload_type == 'issue':
-            payload['state'] = 'all'
-            payload['sort'] = 'updated'
-        elif payload_type == 'comment':
-            payload['sort'] = 'updated'
-
-        if startdate:
-            startdate = startdate.isoformat()
-            payload['since'] = startdate
-        return payload
-
-    def __build_headers(self):
-        """Set header for request"""
-
-        headers = {'Accept': 'application/vnd.github.squirrel-girl-preview'}
-        if self.token:
-            headers.update({'Authorization': 'token ' + self.token})
-        return headers
+    def fetch(self, url, payload=None, headers=None, method=HttpClient.GET, stream=False):
+        self.sleep_for_rate_limit()
+        response = super().fetch(url, payload, headers, method, stream)
+        self.update_rate_limit(response)
 
-    def __send_request(self, url, params=None, headers=None):
-        """GET HTTP caring of rate limit"""
+        return response
 
-        retries = 0
-
-        while retries < self.MAX_RETRIES:
-            try:
-                if self.rate_limit is not None and self.rate_limit <= self.min_rate_to_sleep:
-                    seconds_to_reset = self.rate_limit_reset_ts - int(time.time()) + 1
-                    cause = "GitHub rate limit exhausted."
-                    if self.sleep_for_rate:
-                        logger.info("%s Waiting %i secs for rate limit reset.", cause, seconds_to_reset)
-                        time.sleep(seconds_to_reset)
-                    else:
-                        raise RateLimitError(cause=cause, seconds_to_reset=seconds_to_reset)
-
-                r = requests.get(url, params=params, headers=headers)
-                r.raise_for_status()
-
-                # GitHub service establishes API rate limits.
-                # Enterprise version might have them deactivated.
-                if 'X-RateLimit-Remaining' in r.headers:
-                    self.rate_limit = int(r.headers['X-RateLimit-Remaining'])
-                    self.rate_limit_reset_ts = int(r.headers['X-RateLimit-Reset'])
-                    logger.debug("Rate limit: %s", self.rate_limit)
-                else:
-                    self.rate_limit = None
-                    self.rate_limit_reset_ts = None
-
-                break
-            except requests.exceptions.HTTPError as e:
-                if e.response.status_code == 403 and 'Retry-After' in r.headers:
-                    retry_seconds = int(r.headers['Retry-After'])
-                    logger.warning("Abuse rate limit, the backend will sleep for %s seconds before starting again",
-                                   retry_seconds)
-                    time.sleep(retry_seconds)
-                    retries += 1
-                else:
-                    raise e
-
-        if retries == self.MAX_RETRIES:
-            r.raise_for_status()
-
-        return r
-
-    def _fetch_items(self, path, payload_type, start=None):
+    def fetch_items(self, path, payload):
         """Return the items from github API using links pagination"""
 
         page = 0  # current page
         last_page = None  # last page
-        url_next = self.__get_url(path, start)
+        url_next = urijoin(self.base_url, 'repos', self.owner, self.repository, path)
 
         logger.debug("Get GitHub paginated items from " + url_next)
-        payload = self.__build_payload(payload_type, start)
-        r = self.__send_request(url_next, payload, self.__build_headers())
-        items = r.text
+
+        response = self.fetch(url_next, payload=payload)
+
+        items = response.text
         page += 1
 
-        if 'last' in r.links:
-            last_url = r.links['last']['url']
+        if 'last' in response.links:
+            last_url = response.links['last']['url']
             last_page = last_url.split('&page=')[1].split('&')[0]
             last_page = int(last_page)
             logger.debug("Page: %i/%i" % (page, last_page))
 
         while items:
             yield items
 
             items = None
 
-            if 'next' in r.links:
-                url_next = r.links['next']['url']  # Loving requests :)
-                r = self.__send_request(url_next, payload, self.__build_headers())
+            if 'next' in response.links:
+                url_next = response.links['next']['url']  # Loving requests :)
+                response = self.fetch(url_next, payload=payload)
                 page += 1
-                items = r.text
+
+                items = response.text
                 logger.debug("Page: %i/%i" % (page, last_page))
 
 
 class GitHubCommand(BackendCommand):
     """Class to run GitHub backend from the command line."""
 
     BACKEND = GitHub
@@ -673,14 +664,22 @@
         group.add_argument('--sleep-for-rate', dest='sleep_for_rate',
                            action='store_true',
                            help="sleep for getting more rate")
         group.add_argument('--min-rate-to-sleep', dest='min_rate_to_sleep',
                            default=MIN_RATE_LIMIT, type=int,
                            help="sleep until reset when the rate limit reaches this value")
 
+        # Generic client options
+        group.add_argument('--max-retries', dest='max_retries',
+                           default=MAX_RETRIES, type=int,
+                           help="number of API call retries")
+        group.add_argument('--default-sleep-time', dest='default_sleep_time',
+                           default=DEFAULT_SLEEP_TIME, type=int,
+                           help="sleeping time between API call retries")
+
         # Positional arguments
         parser.parser.add_argument('owner',
                                    help="GitHub owner")
         parser.parser.add_argument('repository',
                                    help="GitHub repository")
 
         return parser
```

### Comparing `perceval-0.9.6/perceval/backends/core/askbot.py` & `perceval-0.9.9/perceval/backends/core/askbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 
 class Askbot(Backend):
@@ -47,15 +48,15 @@
     This class retrieves the questions posted in an Askbot site.
     To initialize this class the URL must be provided. The `url`
     will be set as the origin of the data.
 
     :param url: Askbot site URL
     :param tag: label used to mark the data
     """
-    version = '0.2.4'
+    version = '0.3.0'
 
     def __init__(self, url, tag=None):
         origin = url
 
         super().__init__(origin, tag=tag)
         self.url = url
         self.client = AskbotClient(url)
@@ -74,44 +75,30 @@
         """
 
         if not from_date:
             from_date = DEFAULT_DATETIME
 
         from_date = datetime_to_utc(from_date).timestamp()
 
-        npages = 1
-        next_request = True
-
-        while next_request:
-            whole_page = self.client.get_api_questions(npages)
-            raw_questions = json.loads(whole_page)
-            questions = raw_questions['questions']
-            tpages = raw_questions['pages']
-
-            logger.debug("Fetching questions from '%s': page %s/%s",
-                         self.url, npages, tpages)
+        questions_groups = self.client.get_api_questions(AskbotClient.API_QUESTIONS)
+        for questions in questions_groups:
 
-            for question in questions:
+            for question in questions['questions']:
                 updated_at = int(question['last_activity_at'])
                 if updated_at > from_date:
                     html_question = self.__fetch_question(question)
                     if not html_question:
                         continue
 
                     logger.debug("Fetching HTML question %s", question['id'])
                     comments = self.__fetch_comments(question)
                     question_obj = self.__build_question(html_question, question, comments)
                     question.update(question_obj)
                     yield question
 
-            if npages == tpages:
-                next_request = False
-
-            npages = npages + 1
-
     def __fetch_question(self, question):
         """Fetch an Askbot HTML question body.
 
         The method fetchs the HTML question retrieving the
         question body of the item question received
 
         :param question: item with the question itself
@@ -232,15 +219,15 @@
             for answer in question_object['answers']:
                 if comments[int(answer['id'])]:
                     answer['comments'] = comments[int(answer['id'])]
 
         return question_object
 
 
-class AskbotClient:
+class AskbotClient(HttpClient):
     """Askbot client.
 
     This class implements a simple client to retrieve distinct
     kind of data from an Askbot site.
 
     :param base_url: URL of the Askbot site
 
@@ -251,86 +238,95 @@
     HTML_QUESTION = 'question/'
     ORDER_API = 'activity-asc'
     ORDER_HTML = 'votes'
     COMMENTS = 's/post_comments'
     COMMENTS_OLD = 'post_comments'
 
     def __init__(self, base_url):
-        self.base_url = base_url
+        super().__init__(base_url)
         self._use_new_urls = True
 
-    def get_api_questions(self, page=1):
+    def get_api_questions(self, path):
         """Retrieve a question page using the API.
 
         :param page: page to retrieve
         """
-        path = self.API_QUESTIONS
-        params = {
-            'page': page,
-            'sort': self.ORDER_API
-        }
-        response = self.__call(path, params)
-        return response
+
+        npages = 1
+        next_request = True
+
+        path = urijoin(self.base_url, path)
+        while next_request:
+
+            try:
+                params = {
+                    'page': npages,
+                    'sort': self.ORDER_API
+                }
+
+                response = self.fetch(path, payload=params)
+
+                whole_page = response.text
+
+                raw_questions = json.loads(whole_page)
+                tpages = raw_questions['pages']
+
+                logger.debug("Fetching questions from '%s': page %s/%s",
+                             self.base_url, npages, tpages)
+
+                if npages == tpages:
+                    next_request = False
+
+                npages = npages + 1
+                yield raw_questions
+
+            except requests.exceptions.TooManyRedirects as e:
+                logger.warning("%s, data not retrieved for resource %s", e, path)
+                next_request = False
 
     def get_html_question(self, question_id, page=1):
         """Retrieve a raw HTML question and all it's information.
 
         :param question_id: question identifier
         :param page: page to retrieve
         """
-        path = urijoin(self.HTML_QUESTION, question_id)
+        path = urijoin(self.base_url, self.HTML_QUESTION, question_id)
         params = {
             'page': page,
             'sort': self.ORDER_HTML
         }
 
-        response = self.__call(path, params)
-        return response
+        response = self.fetch(path, payload=params)
+        return response.text
 
     def get_comments(self, post_id):
         """Retrieve a list of comments by a given id.
 
         :param object_id: object identifiere
         """
-        path = self.COMMENTS if self._use_new_urls else self.COMMENTS_OLD
+        path = urijoin(self.base_url, self.COMMENTS if self._use_new_urls else self.COMMENTS_OLD)
         params = {
             'post_id': post_id,
             'post_type': 'answer',
             'avatar_size': 0
         }
         headers = {'X-Requested-With': 'XMLHttpRequest'}
 
         try:
-            response = self.__call(path, params, headers)
+            response = self.fetch(path, payload=params, headers=headers)
         except requests.exceptions.HTTPError as ex:
             if ex.response.status_code == 404:
                 logger.debug("Comments URL did not work. Using old URL schema.")
                 self._use_new_urls = False
-                path = self.COMMENTS_OLD
-                response = self.__call(path, params, headers)
+                path = urijoin(self.base_url, self.COMMENTS_OLD)
+                response = self.fetch(path, payload=params, headers=headers)
             else:
                 raise ex
 
-        return response
-
-    def __call(self, path, params=None, headers=None):
-        """Retrieve all the questions.
-
-        :param path: path of the url
-        :param params: dict with the HTTP parameters needed to run
-            the given command
-        :param headers: headers to use in the request
-        """
-
-        url = urijoin(self.base_url, path)
-
-        req = requests.get(url, params=params, headers=headers)
-        req.raise_for_status()
-
-        return req.text
+        return response.text
 
 
 class AskbotParser:
     """Askbot HTML parser.
 
     This class parses a plain HTML document, converting questions, answers,
     comments and user information into dict items.
```

### Comparing `perceval-0.9.6/perceval/backends/core/nntp.py` & `perceval-0.9.9/perceval/backends/core/nntp.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/backends/core/meetup.py` & `perceval-0.9.9/perceval/backends/core/meetup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,40 +18,37 @@
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import json
 import logging
-import time
-
-import requests
 
 from grimoirelab.toolkit.datetime import datetime_to_utc
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
-from ...errors import CacheError, RateLimitError
+from ...client import HttpClient, RateLimitHandler
+from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 
 MEETUP_URL = 'https://meetup.com/'
 MEETUP_API_URL = 'https://api.meetup.com/'
 MAX_ITEMS = 200
 
 
 # Range before sleeping until rate limit reset
 MIN_RATE_LIMIT = 1
-MAX_RATE_LIMIT = 30
 
 # Time to avoid too many request exception
 SLEEP_TIME = 30
 
 
 class Meetup(Backend):
     """Meetup backend.
@@ -67,15 +64,15 @@
     :param cache: cache object to store raw data
     :param sleep_for_rate: sleep until rate limit is reset
     :param min_rate_to_sleep: minimun rate needed to sleep until
          it will be reset
     :param sleep_time: minimun waiting time to avoid too many request
          exception
     """
-    version = '0.5.2'
+    version = '0.7.0'
 
     def __init__(self, group, api_token, max_items=MAX_ITEMS,
                  tag=None, cache=None,
                  sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
                  sleep_time=SLEEP_TIME):
         origin = MEETUP_URL
 
@@ -332,15 +329,15 @@
         # Required arguments
         parser.parser.add_argument('group',
                                    help="Meetup group name")
 
         return parser
 
 
-class MeetupClient:
+class MeetupClient(HttpClient, RateLimitHandler):
     """Meetup API client.
 
     Client for fetching information from the Meetup server
     using its REST API v3.
 
     :param api_key: key needed to use the API
     :param max_items: maximum number of items per request
@@ -358,36 +355,30 @@
     PSIGN = 'sign'
     PSTATUS = 'status'
 
     VEVENT_FIELDS = ['event_hosts', 'featured', 'group_topics',
                      'plain_text_description', 'rsvpable', 'series']
     VRSVP_FIELDS = ['attendance_status']
     VRESPONSE = ['yes', 'no']
-    VSTATUS = ['cancelled', 'upcoming', 'past', 'proposed',
-               'suggested', 'draft']
+    # FIXME: Add 'draft' status when the bug in the Meetup API gets fixed.
+    # More info in https://github.com/meetup/api/issues/260
+    VSTATUS = ['cancelled', 'upcoming', 'past', 'proposed', 'suggested']
     VUPDATED = 'updated'
 
-    MAX_RETRIES = 5
-
     def __init__(self, api_key, max_items=MAX_ITEMS,
                  sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT, sleep_time=SLEEP_TIME):
         self.api_key = api_key
         self.max_items = max_items
-        self.rate_limit = None
-        self.rate_limit_reset_ts = None
-        self.sleep_for_rate = sleep_for_rate
-        self.sleep_time = sleep_time
-
-        if min_rate_to_sleep > MAX_RATE_LIMIT:
-            msg = "Minimum rate to sleep value exceeded (%d)."
-            msg += "High values might cause the client to sleep forever."
-            msg += "Reset to %d."
-            logger.warning(msg, min_rate_to_sleep, MAX_RATE_LIMIT)
 
-        self.min_rate_to_sleep = min(min_rate_to_sleep, MAX_RATE_LIMIT)
+        super().__init__(MEETUP_API_URL, default_sleep_time=sleep_time, extra_status_forcelist=[429])
+        super().setup_rate_limit_handler(sleep_for_rate=sleep_for_rate, min_rate_to_sleep=min_rate_to_sleep)
+
+    def calculate_time_to_reset(self):
+        """Number of seconds to wait. They are contained in the rate limit reset header"""
+        return self.rate_limit_reset_ts
 
     def events(self, group, from_date=DEFAULT_DATETIME):
         """Fetch the events pages of a given group."""
 
         date = datetime_to_utc(from_date)
         date = date.strftime("since:%Y-%m-%dT%H:%M:%S.000Z")
 
@@ -449,53 +440,29 @@
         pages for that resource and parameters.
 
         :param resource: type of the resource
         :param params: parameters to filter
 
         :returns: a generator of pages for the requeste resource
         """
-        url = urijoin(MEETUP_API_URL, resource)
+        url = urijoin(self.base_url, resource)
 
         params[self.PKEY] = self.api_key
         params[self.PSIGN] = 'true',
 
         do_fetch = True
 
-        retry_time = 0
-        retries = 0
-
         while do_fetch:
             logger.debug("Meetup client calls resource: %s params: %s",
                          resource, str(params))
 
-            if self.rate_limit is not None and self.rate_limit <= self.min_rate_to_sleep:
-                cause = "Meetup rate limit exceeded"
-
-                if self.sleep_for_rate:
-                    logger.warning("%s; waiting %i secs for rate limit reset.",
-                                   cause, self.rate_limit_reset_ts)
-                    time.sleep(self.rate_limit_reset_ts)
-                else:
-                    raise RateLimitError(cause=cause,
-                                         seconds_to_reset=self.rate_limit_reset_ts)
-
-            r = requests.get(url, params=params)
-            time.sleep(retry_time)
-            try:
-                r.raise_for_status()
-            except requests.exceptions.HTTPError as e:
-                if e.response.status_code == 429 and retries < self.MAX_RETRIES:
-                    retries += 1
-                    retry_time = retries * self.sleep_time
-                    continue
-                else:
-                    raise e
+            self.sleep_for_rate_limit()
+            r = self.fetch(url, payload=params)
+            self.update_rate_limit(r)
 
-            self.rate_limit = float(r.headers['X-RateLimit-Remaining'])
-            self.rate_limit_reset_ts = float(r.headers['X-RateLimit-Reset'])
             yield r.text
 
             if r.links and 'next' in r.links:
                 url = r.links['next']['url']
                 params = {
                     self.PKEY: self.api_key,
                     self.PSIGN: 'true'
```

### Comparing `perceval-0.9.6/perceval/backends/core/bugzillarest.py` & `perceval-0.9.9/perceval/backends/core/bugzillarest.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import BaseError, BackendError, CacheError
 from ...utils import DEFAULT_DATETIME
-from ..._version import __version__
 
 
 logger = logging.getLogger(__name__)
 
 
 MAX_BUGS = 500  # Maximum number of bugs per query
 MAX_CONTENTS = 25  # Maximum number of bug contents (history, comments) per query
@@ -57,15 +57,15 @@
     :param user: Bugzilla user
     :param password: Bugzilla user password
     :param api_token: Bugzilla token
     :param max_bugs: maximum number of bugs requested on the same query
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.3'
+    version = '0.6.0'
 
     def __init__(self, url, user=None, password=None, api_token=None,
                  max_bugs=MAX_BUGS, tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
@@ -291,15 +291,15 @@
 
 class BugzillaRESTError(BaseError):
     """Raised when an error occurs using the API"""
 
     message = "%(error)s (code: %(code)s)"
 
 
-class BugzillaRESTClient:
+class BugzillaRESTClient(HttpClient):
     """Bugzilla REST API client.
 
     This class implements a simple client to retrieve distinct
     kind of data from a Bugzilla > 5.0 repository using its
     REST API.
 
     When `user` and `password` parameters are given it logs in
@@ -312,15 +312,14 @@
     :param api_token: api token for user; when this is provided
         `user` and `password` parameters will be ignored
 
     :raises BackendError: when an error occurs initilizing the
         client
     """
     URL = "%(base)s/rest/%(resource)s"
-    HEADERS = {'User-Agent': 'Perceval/' + __version__}
 
     # API resources
     RBUG = 'bug'
     RATTACHMENT = 'attachment'
     RCOMMENT = 'comment'
     RHISTORY = 'history'
     RLOGIN = 'login'
@@ -339,15 +338,15 @@
 
     # Predefined values
     VCHANGE_DATE_ORDER = 'changeddate'
     VINCLUDE_ALL = '_all'
     VEXCLUDE_ATTCH_DATA = 'data'
 
     def __init__(self, base_url, user=None, password=None, api_token=None):
-        self.base_url = base_url
+        super().__init__(base_url)
         self.api_token = api_token if api_token else None
 
         if user is not None and password is not None:
             self.login(user, password)
 
     def login(self, user, password):
         """Authenticate a user in the server.
@@ -457,17 +456,15 @@
 
         if self.api_token:
             params[self.PBUGZILLA_TOKEN] = self.api_token
 
         logger.debug("Bugzilla REST client requests: %s params: %s",
                      resource, str(params))
 
-        headers = self.HEADERS
-        r = requests.get(url, headers=headers, params=params)
-        r.raise_for_status()
+        r = self.fetch(url, payload=params)
 
         # Check for possible Bugzilla API errors
         result = r.json()
 
         if result.get('error', False):
             raise BugzillaRESTError(error=result['message'],
                                     code=result['code'])
```

### Comparing `perceval-0.9.6/perceval/backends/core/slack.py` & `perceval-0.9.9/perceval/backends/core/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import json
 import logging
 
-import requests
-
 from grimoirelab.toolkit.datetime import datetime_to_utc, datetime_utcnow
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import BaseError, CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 SLACK_URL = 'https://slack.com/'
@@ -54,15 +53,15 @@
 
     :param channel: identifier of the channel where data will be fetched
     :param api_token: token or key needed to use the API
     :param max_items: maximum number of message requested on the same query
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.2.3'
+    version = '0.3.0'
 
     def __init__(self, channel, api_token, max_items=MAX_ITEMS,
                  tag=None, cache=None):
         origin = urijoin(SLACK_URL, channel)
 
         super().__init__(origin, tag=tag, cache=cache)
         self.channel = channel
@@ -342,15 +341,15 @@
 
 class SlackClientError(BaseError):
     """Raised when an error occurs using the Slack client"""
 
     message = "%(error)s"
 
 
-class SlackClient:
+class SlackClient(HttpClient):
     """Slack API client.
 
     Client for fetching information from the Slack server
     using its REST API.
 
     :param api_key: key needed to use the API
     :param max_items: maximum number of items per request
@@ -365,14 +364,15 @@
     PCOUNT = 'count'
     POLDEST = 'oldest'
     PLATEST = 'latest'
     PTOKEN = 'token'
     PUSER = 'user'
 
     def __init__(self, api_token, max_items=MAX_ITEMS):
+        super().__init__(SLACK_URL)
         self.api_token = api_token
         self.max_items = max_items
 
     def channel_info(self, channel):
         """Fetch information about a channel."""
 
         resource = self.RCHANNEL_INFO
@@ -426,16 +426,15 @@
         """
         url = self.URL % {'resource': resource}
         params[self.PTOKEN] = self.api_token
 
         logger.debug("Slack client requests: %s params: %s",
                      resource, str(params))
 
-        r = requests.get(url, params=params)
-        r.raise_for_status()
+        r = self.fetch(url, payload=params)
 
         # Check for possible API errors
         result = r.json()
 
         if not result['ok']:
             raise SlackClientError(error=result['error'])
```

### Comparing `perceval-0.9.6/perceval/backends/core/mbox.py` & `perceval-0.9.9/perceval/backends/core/mbox.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/backends/core/pipermail.py` & `perceval-0.9.9/perceval/backends/core/pipermail.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/backends/core/rss.py` & `perceval-0.9.9/perceval/backends/core/rss.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 # Authors:
 #     Alvaro del Castillo <acs@bitergia.com>
 #
 
 import logging
 
 import feedparser
-import requests
 
 from grimoirelab.toolkit.datetime import str_to_datetime
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
-from ..._version import __version__
 
 
 logger = logging.getLogger(__name__)
 
 
 class RSS(Backend):
     """RSS backend for Perceval.
@@ -45,15 +44,15 @@
     To initialize this class the URL must be provided.
     The `url` will be set as the origin of the data.
 
     :param url: RSS url
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.1.2'
+    version = '0.2.0'
 
     def __init__(self, url, tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
         self.client = RSSClient(url)
@@ -147,36 +146,32 @@
 
         This backend only generates one type of item which is
         'entry'.
         """
         return 'entry'
 
 
-class RSSClient:
+class RSSClient(HttpClient):
     """RSS API client.
 
     This class implements a simple client to retrieve entries from
     projects in a RSS node.
 
     :param url: URL of rss node: https://item.opnfv.org/ci
 
     :raises HTTPError: when an error occurs doing the request
     """
 
     def __init__(self, url):
-        self.url = url
+        super().__init__(url)
 
     def get_entries(self):
         """ Retrieve all entries from a RSS feed"""
 
-        # wordpress.com blogs need a User-Agent header
-        headers = {'User-Agent': 'perceval-' + __version__}
-
-        req = requests.get(self.url, headers=headers)
-        req.raise_for_status()
+        req = self.fetch(self.base_url)
         return req.text
 
 
 class RSSCommand(BackendCommand):
     """Class to run RSS backend from the command line."""
 
     BACKEND = RSS
```

### Comparing `perceval-0.9.6/perceval/backends/core/discourse.py` & `perceval-0.9.9/perceval/backends/core/discourse.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,22 @@
 #    J. Manrique López de la Fuente <jsmanrique@bitergia.com>
 #    Alvaro del Castillo San Felix <acs@bitergia.com>
 #
 
 import json
 import logging
 
-import requests
-
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -49,15 +48,15 @@
     will be set as the origin of the data.
 
     :param url: Discourse URL
     :param api_token: Discourse API access token
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.1'
+    version = '0.6.0'
 
     def __init__(self, url, api_token=None,
                  tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
@@ -288,15 +287,15 @@
 
         This backend only generates one type of item which is
         'topic'.
         """
         return 'topic'
 
 
-class DiscourseClient:
+class DiscourseClient(HttpClient):
     """Discourse API client.
 
     This class implements a simple client to retrieve topics from
     any Discourse board.
 
     :param url: URL of the Discourse site
     :param api_key: Discourse API access token
@@ -312,16 +311,16 @@
     # Params
     PKEY = 'api_key'
     PPAGE = 'page'
 
     # Data type
     TJSON = '.json'
 
-    def __init__(self, url, api_key=None):
-        self.url = url
+    def __init__(self, base_url, api_key=None):
+        super().__init__(base_url)
         self.api_key = api_key
 
     def topics_page(self, page=None):
         """Retrieve the #page summaries of the latest topics.
 
         :param page: number of page to retrieve
         """
@@ -371,24 +370,23 @@
 
         :param res: type of resource to fetch
         :param res_id: identifier of the resource
         :param params: dict with the HTTP parameters needed to run
             the given command
         """
         if res:
-            url = urijoin(self.url, res, res_id)
+            url = urijoin(self.base_url, res, res_id)
         else:
-            url = urijoin(self.url, res_id)
+            url = urijoin(self.base_url, res_id)
         url += self.TJSON
 
         logger.debug("Discourse client calls resource: %s %s params: %s",
                      res, res_id, str(params))
 
-        r = requests.get(url, params=params)
-        r.raise_for_status()
+        r = self.fetch(url, payload=params)
 
         return r.text
 
 
 class DiscourseCommand(BackendCommand):
     """Class to run Discourse backend from the command line."""
```

### Comparing `perceval-0.9.6/perceval/backends/core/launchpad.py` & `perceval-0.9.9/perceval/backends/core/launchpad.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 #
 
 import hmac
 import hashlib
 import json
 import logging
 import requests
-import time
 
 from grimoirelab.toolkit.datetime import (datetime_utcnow,
                                           datetime_to_utc,
                                           str_to_datetime)
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 LAUNCHPAD_URL = "https://launchpad.net/"
-LAUNCHPAD_API_URL = 'https://api.launchpad.net/1.0/'
+LAUNCHPAD_API_URL = 'https://api.launchpad.net/1.0'
 
 TARGET_ISSUE_FIELDS = ['bug_link', 'owner_link', 'assignee_link']
 ITEMS_PER_PAGE = 75
 SLEEP_TIME = 300
 
 logger = logging.getLogger(__name__)
 
@@ -61,15 +61,15 @@
     :param api_token: Launchpad auth token to access the API
     :param tag: label used to mark the data
     :param cache: use issues already retrieved in cache
     :param sleep_for_rate: sleep until rate limit is reset
     :param min_rate_to_sleep: minimun rate needed to sleep until
            it will be reset
     """
-    version = '0.1.0'
+    version = '0.2.0'
 
     def __init__(self, distribution, package=None,
                  consumer_key=None, api_token=None,
                  items_per_page=ITEMS_PER_PAGE, sleep_time=SLEEP_TIME,
                  tag=None, cache=None):
 
         origin = urijoin(LAUNCHPAD_URL, distribution)
@@ -398,30 +398,28 @@
         self._push_cache_queue(user_raw)
 
         user = json.loads(user_raw)
 
         return user
 
 
-class LaunchpadClient:
+class LaunchpadClient(HttpClient):
     """Client for retrieving information from Launchpad API"""
 
-    # Max retries for handled HTTP errors
-    MAX_RETRIES = 5
     _users = {}
 
     def __init__(self, distribution, package=None,
                  consumer_key=None, api_token=None,
                  items_per_page=ITEMS_PER_PAGE, sleep_time=SLEEP_TIME):
+        super().__init__(LAUNCHPAD_API_URL, default_sleep_time=sleep_time)
         self.consumer_key = consumer_key
         self.api_token = api_token
         self.distribution = distribution
         self.package = package
         self.items_per_page = items_per_page
-        self.sleep_time = sleep_time
 
     def issues(self, start=None):
         """Get the issues from pagination"""
 
         payload = self.__build_payload(size=self.items_per_page, operation=True, startdate=start)
         path = self.__get_url_project()
         return self.__fetch_items(path=path, payload=payload)
@@ -438,16 +436,16 @@
 
         logger.info("Getting info for %s" % (url_user))
 
         try:
             raw_user = self.__send_request(url_user, headers=self.__get_headers())
             user = raw_user
         except requests.exceptions.HTTPError as e:
-            if e.response.status_code == 410:
-                logger.warning("Data is not available due to HTTP 410 Gone - %s", url_user)
+            if e.response.status_code in [404, 410]:
+                logger.warning("Data is not available - %s", url_user)
                 user = '{}'
             else:
                 raise e
 
         self._users[user_name] = user
 
         return user
@@ -486,25 +484,25 @@
             url = self.__get_url_distribution()
 
         return url
 
     def __get_url_distribution(self):
         """Build URL distribution"""
 
-        return LAUNCHPAD_API_URL + self.distribution
+        return urijoin(self.base_url, self.distribution)
 
     def __get_url_distribution_package(self):
         """Build URL distribution package"""
 
         return urijoin(self.__get_url_distribution(), "+source", self.package)
 
     def __get_url(self, path):
         """Build genereic URL"""
 
-        return LAUNCHPAD_API_URL + path
+        return urijoin(self.base_url, path)
 
     def _generate_signature(self):
         """Get HTTP request signature based on consumer_key and token"""
 
         sign = hmac.new(bytes(self.consumer_key.encode('utf-8')),
                         bytes(self.api_token.encode('utf-8')),
                         hashlib.sha256).hexdigest()
@@ -520,30 +518,15 @@
 
     def __send_request(self, url, params=None, headers=None):
         """Send request"""
 
         if self.consumer_key and self.api_token:
             headers['Sign'] = self._generate_signature()
 
-        retries = 0
-
-        while retries < self.MAX_RETRIES:
-            try:
-                r = requests.get(url,
-                                 params=params,
-                                 headers=headers)
-                break
-            except requests.exceptions.ConnectionError:
-                logger.warning("Connection was lost, the backend will sleep for " +
-                               str(self.sleep_time) + "s before starting again")
-                time.sleep(self.sleep_time * retries)
-                retries += 1
-
-        r.raise_for_status()
-
+        r = self.fetch(url, payload=params, headers=headers)
         return r.text
 
     def __build_payload(self, size, operation=False, startdate=None):
         """Build payload"""
 
         payload = {
             'ws.size': size,
@@ -574,16 +557,16 @@
         while fetch_data:
             logger.debug("Fetching page: %i", page)
 
             try:
                 raw_content = self.__send_request(url_next, payload, self.__get_headers())
                 content = json.loads(raw_content)
             except requests.exceptions.HTTPError as e:
-                if e.response.status_code == 410:
-                    logger.warning("Data is not available due to HTTP 410 Gone - %s", url_next)
+                if e.response.status_code in [410]:
+                    logger.warning("Data is not available - %s", url_next)
                     raw_content = '{"total_size": 0, "start": 0, "entries": []}'
                     content = json.loads(raw_content)
                 else:
                     raise e
 
             if 'next_collection_link' in content:
                 url_next = content['next_collection_link']
```

### Comparing `perceval-0.9.6/perceval/backends/core/dockerhub.py` & `perceval-0.9.9/perceval/backends/core/dockerhub.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import json
 import logging
 
-import requests
-
 from grimoirelab.toolkit.datetime import datetime_utcnow
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 
 
 logger = logging.getLogger(__name__)
 
 
 DOCKERHUB_URL = "https://hub.docker.com/"
@@ -57,15 +56,15 @@
     be replaced by its long name: `library`.
 
     :param owner: DockerHub owner
     :param repository: DockerHub repository owned by `owner`
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.1.2'
+    version = '0.2.0'
 
     def __init__(self, owner, repository,
                  tag=None, cache=None):
         if owner == DOCKER_SHORTCUT_OWNER:
             owner = DOCKER_OWNER
 
         origin = urijoin(DOCKERHUB_URL, owner, repository)
@@ -183,46 +182,35 @@
 
         :returns: a dict with the parsed data
         """
         result = json.loads(raw_json)
         return result
 
 
-class DockerHubClient:
+class DockerHubClient(HttpClient):
     """DockerHub API client.
 
     Client for fetching information from the DockerHub server
     using its REST API v2.
     """
     RREPOSITORY = 'repositories'
 
+    def __init__(self):
+        super().__init__(DOCKERHUB_API_URL)
+
     def repository(self, owner, repository):
         """Fetch information about a repository."""
 
-        resource = urijoin(self.RREPOSITORY, owner, repository)
-        response = self._fetch(resource, {})
-
-        return response
-
-    def _fetch(self, resource, params):
-        """Fetch a resource.
-
-        :param resource: resource to fetch
-        :param params: dict with the HTTP parameters needed to call
-            the given method
-        """
-        url = urijoin(DOCKERHUB_API_URL, resource)
+        url = urijoin(self.base_url, self.RREPOSITORY, owner, repository)
 
-        logger.debug("DockerHub client requests: %s params: %s",
-                     resource, str(params))
+        logger.debug("DockerHub client requests: %s", url)
 
-        r = requests.get(url, params=params)
-        r.raise_for_status()
+        response = self.fetch(url)
 
-        return r.text
+        return response.text
 
 
 class DockerHubCommand(BackendCommand):
     """Class to run DockerHub backend from the command line."""
 
     BACKEND = DockerHub
```

### Comparing `perceval-0.9.6/perceval/backends/core/bugzilla.py` & `perceval-0.9.9/perceval/backends/core/bugzilla.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,24 @@
 import csv
 import datetime
 import logging
 import re
 
 import bs4
 import dateutil.tz
-import requests
 
 from grimoirelab.toolkit.datetime import str_to_datetime
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import BackendError, CacheError, ParseError
 from ...utils import DEFAULT_DATETIME, xml_to_dict
-from ..._version import __version__
 
 
 MAX_BUGS = 200  # Maximum number of bugs per query
 MAX_BUGS_CSV = 10000  # Maximum number of bugs per CSV query
 
 logger = logging.getLogger(__name__)
 
@@ -58,15 +57,15 @@
     :param url: Bugzilla server URL
     :param user: Bugzilla user
     :param password: Bugzilla user password
     :param max_bugs: maximum number of bugs requested on the same query
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.6.2'
+    version = '0.7.0'
 
     def __init__(self, url, user=None, password=None,
                  max_bugs=MAX_BUGS, max_bugs_csv=MAX_BUGS_CSV,
                  tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
@@ -396,15 +395,15 @@
         # Required arguments
         parser.parser.add_argument('url',
                                    help="URL of the Bugzilla server")
 
         return parser
 
 
-class BugzillaClient:
+class BugzillaClient(HttpClient):
     """Bugzilla API client.
 
     This class implements a simple client to retrieve distinct
     kind of data from a Bugzilla repository. Currently, it only
     supports 3.x and 4.x servers.
 
     When it is initialized, it checks if the given Bugzilla is
@@ -415,15 +414,14 @@
     :param password: user password
     :param max_bugs_cvs: max bugs requested per CSV query
 
     :raises BackendError: when an error occurs initilizing the
         client
     """
     URL = "%(base)s/%(cgi)s"
-    HEADERS = {'User-Agent': 'Perceval/' + __version__}
 
     # Regular expression to check the Bugzilla version
     VERSION_REGEX = re.compile(r'.+bugzilla version="([^"]+)"',
                                flags=re.DOTALL)
 
     # Bugzilla versions that follow the old style queries
     OLD_STYLE_VERSIONS = ['3.2.3', '3.2.2']
@@ -448,17 +446,16 @@
 
     # Content-type values
     CTYPE_CSV = 'csv'
     CTYPE_XML = 'xml'
 
     def __init__(self, base_url, user=None, password=None,
                  max_bugs_csv=MAX_BUGS_CSV):
-        self.base_url = base_url
         self.version = None
-        self._session = self.__create_http_session()
+        super().__init__(base_url)
 
         if user is not None and password is not None:
             self.login(user, password)
 
         self.max_bugs_csv = max_bugs_csv
 
     def login(self, user, password):
@@ -473,16 +470,15 @@
             self.PBUGZILLA_LOGIN: user,
             self.PBUGZILLA_PASSWORD: password,
             self.PLOGIN: 'Log in'
         }
 
         headers = {'Referer': self.base_url}
 
-        req = self._session.post(url, data=payload, headers=headers)
-        req.raise_for_status()
+        req = self.fetch(url, payload=payload, headers=headers, method=HttpClient.POST)
 
         # Check if the authentication went OK. When this string
         # is found means that the authentication was successful
         if req.text.find("index.cgi?logout=1") < 0:
             cause = ("Bugzilla client could not authenticate user %s. "
                      "Please check user and password parameters. "
                      "URLs may also need a trailing '/'.") % user
@@ -495,15 +491,15 @@
         """Logout from the server."""
 
         params = {
             self.PLOGOUT: '1'
         }
 
         self.call(self.CGI_LOGIN, params)
-        self._session = self.__create_http_session()
+        self._close_http_session()
 
         logger.debug("Bugzilla user logged out from %s",
                      self.base_url)
 
     def metadata(self):
         """Get metadata information in XML format."""
 
@@ -577,24 +573,18 @@
             the given command
         """
         url = self.URL % {'base': self.base_url, 'cgi': cgi}
 
         logger.debug("Bugzilla client calls command: %s params: %s",
                      cgi, str(params))
 
-        req = self._session.get(url, params=params)
-        req.raise_for_status()
+        req = self.fetch(url, payload=params)
 
         return req.text
 
-    def __create_http_session(self):
-        session = requests.Session()
-        session.headers.update(self.HEADERS)
-        return session
-
     def __fetch_version(self):
         response = self.metadata()
         m = re.match(self.VERSION_REGEX, response)
 
         if m:
             version = m.group(1)
             logger.debug("Bugzilla server is online: %s (v. %s)",
```

### Comparing `perceval-0.9.6/perceval/backends/core/phabricator.py` & `perceval-0.9.9/perceval/backends/core/phabricator.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,22 @@
 #
 # Authors:
 #     Santiago Dueñas <sduenas@bitergia.com>
 #
 
 import json
 import logging
-import time
-
-import requests
 
 from grimoirelab.toolkit.datetime import datetime_to_utc
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import BaseError, CacheError
 from ...utils import DEFAULT_DATETIME
 
 logger = logging.getLogger(__name__)
 
 
 class Phabricator(Backend):
@@ -47,15 +45,15 @@
     URL.
 
     :param url: URL of the server
     :param api_token: token needed to use the API
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.4'
+    version = '0.6.1'
 
     def __init__(self, url, api_token, tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
         self.client = ConduitClient(url, api_token)
@@ -488,30 +486,27 @@
 
 class ConduitError(BaseError):
     """Raised when an error occurs using Conduit"""
 
     message = "%(error)s (code: %(code)s)"
 
 
-class ConduitClient:
+class ConduitClient(HttpClient):
     """Conduit API Client.
 
     Phabricator uses Conduit as the Phabricator REST API.
     This class implements some of its methods to retrieve the
     contents from a Phabricator server.
 
     :param base_url: URL of the Phabricator server
     :param api_token: token to get access to restricted methods
         of the API
     """
     URL = '%(base)s/api/%(method)s'
 
-    # Max retries for handled HTTP errors
-    MAX_RETRIES = 3
-
     # Methods
     MANIPHEST_TASKS = 'maniphest.search'
     MANIPHEST_TRANSACTIONS = 'maniphest.gettasktransactions'
     PHAB_PHIDS = 'phid.query'
     PHAB_USERS = 'user.query'
 
     PAFTER = 'after'
@@ -522,15 +517,15 @@
     PPROJECTS = 'projects'
     PORDER = 'order'
     PMODIFIED_START = 'modifiedStart'
 
     VOUTDATED = 'outdated'
 
     def __init__(self, base_url, api_token):
-        self.base_url = base_url.rstrip('/')
+        super().__init__(base_url.rstrip('/'), max_retries=3, extra_status_forcelist=[502, 503])
         self.api_token = api_token
 
     def tasks(self, from_date=DEFAULT_DATETIME):
         """Retrieve tasks.
 
         :param from_date: retrieve tasks that where updated from that date;
             dates are converted epoch time.
@@ -621,27 +616,15 @@
             'output': 'json',
             '__conduit__': True
         }
 
         logger.debug("Phabricator Conduit client requests: %s params: %s",
                      method, str(data))
 
-        retries = 0
-
-        while retries < self.MAX_RETRIES:
-            r = requests.post(url, data=data, verify=False)
-
-            if r.status_code not in [502, 503]:
-                break
-
-            time.sleep(0.5 * retries)
-            retries += 1
-
-        # Check for other possible HTTP errors
-        r.raise_for_status()
+        r = self.fetch(url, payload=data, method=HttpClient.POST, verify=False)
 
         # Check for possible Conduit API errors
         result = r.json()
 
         if result['error_code']:
             raise ConduitError(error=result['error_info'],
                                code=result['error_code'])
```

### Comparing `perceval-0.9.6/perceval/backends/core/git.py` & `perceval-0.9.9/perceval/backends/core/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     :param gitpath: path to the repository or to the log file
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
 
     :raises RepositoryError: raised when there was an error cloning or
         updating the repository.
     """
-    version = '0.8.7'
+    version = '0.8.9'
 
     def __init__(self, uri, gitpath, tag=None, cache=None):
         origin = uri
 
         super().__init__(origin, tag=tag, cache=cache)
         self.uri = uri
         self.gitpath = gitpath
@@ -972,26 +972,29 @@
 
         logger.debug("Git show fetched from %s repository (%s)",
                      self.uri, self.dirpath)
 
     def _fetch_pack(self):
         """Fetch changes and store them in a pack."""
 
+        def prepare_refs(refs):
+            return [ref.hash.encode('utf-8') for ref in refs
+                    if not ref.refname.endswith('^{}')]
+
         def determine_wants(refs):
-            remote_refs = self._discover_refs(remote=True)
-            remote_refs = [ref.hash.encode('utf-8') for ref in remote_refs
-                           if not ref.refname.endswith('^{}')]
-            return remote_refs
+            remote_refs = prepare_refs(self._discover_refs(remote=True))
+            local_refs = prepare_refs(self._discover_refs())
+            wants = [ref for ref in remote_refs if ref not in local_refs]
+            return wants
 
         client, repo_path = dulwich.client.get_transport_and_path(self.uri)
         repo = dulwich.repo.Repo(self.dirpath)
         fd = io.BytesIO()
 
-        local_refs = [ref.hash.encode('utf-8') for ref in self._discover_refs()
-                      if not ref.refname.endswith('^{}')]
+        local_refs = prepare_refs(self._discover_refs())
         graph_walker = _GraphWalker(local_refs)
 
         result = client.fetch_pack(repo_path,
                                    determine_wants,
                                    graph_walker,
                                    fd.write)
         refs = [GitRef(ref_hash.decode('utf-8'), ref_name.decode('utf-8'))
@@ -1056,32 +1059,39 @@
         cmd = ['git', 'remote', 'prune', 'origin']
         self._exec(cmd, cwd=self.dirpath, env=self.gitenv)
 
     def _discover_refs(self, remote=False):
         """Get the current list of local or remote refs."""
 
         if remote:
-            cmd_refs = ['git', 'ls-remote', '-h', '-t', 'origin']
+            cmd_refs = ['git', 'ls-remote', '-h', '-t', '--exit-code', 'origin']
             sep = '\t'
+            ignored_error_codes = [2]
         else:
             # Check first whether the local repo is empty;
             # Running 'show-ref' in empty repos gives an error
             if self.is_empty():
                 raise EmptyRepositoryError(repository=self.uri)
 
             cmd_refs = ['git', 'show-ref', '--heads', '--tags']
             sep = ' '
+            ignored_error_codes = [1]
 
+        # Error codes returned when no matching refs (i.e, no heads
+        # or tags) are found in a repository will be ignored. Otherwise,
+        # the full process would fail for those situations.
         outs = self._exec(cmd_refs, cwd=self.dirpath,
-                          env=self.gitenv)
+                          env=self.gitenv,
+                          ignored_error_codes=ignored_error_codes)
         outs = outs.decode('utf-8', errors='surrogateescape').rstrip()
+        outs = outs.split('\n') if outs else []
 
         refs = []
 
-        for line in outs.split('\n'):
+        for line in outs:
             data = line.split(sep)
             ref = GitRef(data[0], data[1])
             refs.append(ref)
 
         return refs
 
     def _update_ref(self, ref, delete=False):
@@ -1172,37 +1182,45 @@
                     logger.debug("Git log stderr: " + self.failed_message)
                 self.failed_message = err_line
             else:
                 # The subprocess is successfully up to now, print the line
                 logger.debug("Git log stderr: " + err_line)
 
     @staticmethod
-    def _exec(cmd, cwd=None, env=None, encoding='utf-8'):
+    def _exec(cmd, cwd=None, env=None, ignored_error_codes=None,
+              encoding='utf-8'):
         """Run a command.
 
-        Execute `cmd` command in the directory set by `cwd`. Enviroment
+        Execute `cmd` command in the directory set by `cwd`. Environment
         variables can be set using the `env` dictionary. The output
         data is returned as encoded bytes.
 
+        Commands which their returning status codes are non-zero will
+        be treated as failed. Error codes considered as valid can be
+        ignored giving them in the `ignored_error_codes` list.
+
         :returns: the output of the command as encoded bytes
 
         :raises RepositoryError: when an error occurs running the command
         """
+        if ignored_error_codes is None:
+            ignored_error_codes = []
+
         logger.debug("Running command %s (cwd: %s, env: %s)",
                      ' '.join(cmd), cwd, str(env))
 
         try:
             proc = subprocess.Popen(cmd, stdout=subprocess.PIPE,
                                     stderr=subprocess.PIPE,
                                     cwd=cwd, env=env)
             (outs, errs) = proc.communicate()
         except OSError as e:
             raise RepositoryError(cause=str(e))
 
-        if proc.returncode != 0:
+        if proc.returncode != 0 and proc.returncode not in ignored_error_codes:
             err = errs.decode(encoding, errors='surrogateescape')
             cause = "git command - %s" % err
             raise RepositoryError(cause=cause)
         else:
             logger.debug(errs.decode(encoding, errors='surrogateescape'))
 
         return outs
```

### Comparing `perceval-0.9.6/perceval/backends/core/gmane.py` & `perceval-0.9.9/perceval/backends/core/gmane.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/backends/core/supybot.py` & `perceval-0.9.9/perceval/backends/core/supybot.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/backends/core/hyperkitty.py` & `perceval-0.9.9/perceval/backends/core/hyperkitty.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 import datetime
 import logging
 import os
 
 import dateutil.parser
 import dateutil.relativedelta
 import dateutil.tz
-import requests
 
 from grimoirelab.toolkit.datetime import datetime_to_utc, datetime_utcnow
 from grimoirelab.toolkit.uris import urijoin
 
 from .mbox import MBox, MailingList
 from ...backend import (BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...utils import (DEFAULT_DATETIME,
                       months_range)
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -52,15 +52,15 @@
     and stored. The origin of the data will be set to the value of `url`.
 
     :param url: URL to the HyperKitty mailing list archiver
     :param dirpath: directory path where the mboxes are stored
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.1.1'
+    version = '0.2.0'
 
     def __init__(self, url, dirpath, tag=None, cache=None):
         super().__init__(url, dirpath, tag=tag, cache=cache)
         self.url = url
 
     @metadata
     def fetch(self, from_date=DEFAULT_DATETIME):
@@ -121,15 +121,15 @@
     format.
 
     :param url: URL to the HyperKitty archiver for this list
     :param dirpath: path to the local mboxes archives
     """
     def __init__(self, url, dirpath):
         super().__init__(url, dirpath)
-        self.url = url
+        self.client = HttpClient(url)
 
     def fetch(self, from_date=DEFAULT_DATETIME):
         """Fetch the mbox files from the remote archiver.
 
         This method stores the archives in the path given during the
         initialization of this object.
 
@@ -141,20 +141,18 @@
             equal or after the given date; only year and month values
             are compared
 
         :returns: a list of tuples, storing the links and paths of the
             fetched archives
         """
         logger.info("Downloading mboxes from '%s' to since %s",
-                    self.url, str(from_date))
+                    self.client.base_url, str(from_date))
         logger.debug("Storing mboxes in '%s'", self.dirpath)
 
-        # Check mailing list URL
-        r = requests.get(self.url)
-        r.raise_for_status()
+        self.client.fetch(self.client.base_url)
 
         from_date = datetime_to_utc(from_date)
         to_end = datetime_utcnow()
         to_end += dateutil.relativedelta.relativedelta(months=1)
 
         months = months_range(from_date, to_end)
 
@@ -167,15 +165,15 @@
 
         for dts in months:
             tmbox += 1
             start, end = dts[0], dts[1]
             filename = start.strftime("%Y-%m.mbox.gz")
             filepath = os.path.join(self.dirpath, filename)
 
-            url = urijoin(self.url, 'export', filename)
+            url = urijoin(self.client.base_url, 'export', filename)
 
             params = {
                 'start': start.strftime("%Y-%m-%d"),
                 'end': end.strftime("%Y-%m-%d")
             }
 
             success = self._download_archive(url, params, filepath)
@@ -218,16 +216,15 @@
             logger.debug("Date of file %s not detected due to %s",
                          filepath, str(e))
             logger.debug("Date set to default: %s", str(dt))
 
         return dt
 
     def _download_archive(self, url, params, filepath):
-        r = requests.get(url, params=params, stream=True)
-        r.raise_for_status()
+        r = self.client.fetch(url, payload=params, stream=True)
 
         try:
             with open(filepath, 'wb') as fd:
                 fd.write(r.raw.read())
         except OSError as e:
             logger.warning("Ignoring %s archive due to: %s", url, str(e))
             return False
```

### Comparing `perceval-0.9.6/perceval/backends/core/gerrit.py` & `perceval-0.9.9/perceval/backends/core/gerrit.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                         BackendCommandArgumentParser,
                         metadata)
 from ...errors import BackendError, CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 MAX_REVIEWS = 500  # Maximum number of reviews per query
+PORT = '29418'
 
 logger = logging.getLogger(__name__)
 
 
 class Gerrit(Backend):
     """Gerrit backend.
 
@@ -52,29 +53,29 @@
     :param url: Gerrit server URL
     :param user: SSH user used to connect to the Gerrit server
     :param max_reviews: maximum number of reviews requested on the same query
     :param blacklist_reviews: exclude the reviews of this list while fetching
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.7.3'
+    version = '0.7.4'
 
     def __init__(self, url,
-                 user=None, max_reviews=MAX_REVIEWS,
+                 user=None, port=PORT, max_reviews=MAX_REVIEWS,
                  blacklist_reviews=None,
                  disable_host_key_check=False,
                  tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
         self.max_reviews = max(1, max_reviews)
         self.blacklist_reviews = blacklist_reviews
         self.client = GerritClient(self.url, user, max_reviews,
-                                   blacklist_reviews, disable_host_key_check)
+                                   blacklist_reviews, disable_host_key_check, port=port)
 
     @metadata
     def fetch(self, from_date=DEFAULT_DATETIME):
         """Fetch the reviews from the repository.
 
         The method retrieves, from a Gerrit repository, the reviews
         updated since the given date.
@@ -281,32 +282,36 @@
     :param repository: URL of the Gerrit server
     :param user: SSH user to be used to connect to gerrit server
     :param max_reviews: max number of reviews per query
     """
     VERSION_REGEX = re.compile(r'gerrit version (\d+)\.(\d+).*')
     CMD_GERRIT = 'gerrit'
     CMD_VERSION = 'version'
-    PORT = '29418'
     MAX_RETRIES = 3  # max number of retries when a command fails
     RETRY_WAIT = 60  # number of seconds when retrying a ssh command
 
     def __init__(self, repository, user, max_reviews, blacklist_reviews=[],
-                 disable_host_key_check=False):
+                 disable_host_key_check=False, port=PORT):
         self.gerrit_user = user
         self.max_reviews = max_reviews
         self.blacklist_reviews = blacklist_reviews
         self.repository = repository
         self.project = None
         self._version = None
+        self.port = port
         ssh_opts = ''
         if disable_host_key_check:
             ssh_opts += "-o StrictHostKeyChecking=no "
 
-        self.gerrit_cmd = "ssh %s -p %s %s@%s" % (ssh_opts, GerritClient.PORT,
-                                                  self.gerrit_user, self.repository)
+        if self.port:
+            self.gerrit_cmd = "ssh %s -p %s %s@%s" % (ssh_opts, self.port,
+                                                      self.gerrit_user, self.repository)
+        else:
+            self.gerrit_cmd = "ssh %s %s@%s" % (ssh_opts, self.gerrit_user, self.repository)
+
         self.gerrit_cmd += " %s " % (GerritClient.CMD_GERRIT)
 
     def __execute(self, cmd):
         """ Execute gerrit command with retry if it fails """
 
         data = None  # data result from the cmd execution
 
@@ -448,13 +453,16 @@
                            type=int, default=MAX_REVIEWS,
                            help="Max number of reviews per ssh query.")
         group.add_argument('--blacklist-reviews', dest='blacklist_reviews',
                            nargs='*',
                            help="Wrong reviews that must not be retrieved.")
         group.add_argument('--disable-host-key-check', dest='disable_host_key_check', action='store_true',
                            help="Don't check remote host identity")
+        group.add_argument('--ssh-port', dest='port',
+                           default=PORT,
+                           help="Set SSH port of the Gerrit server")
 
         # Required arguments
         parser.parser.add_argument('url',
                                    help="URL of the Gerrit server")
 
         return parser
```

### Comparing `perceval-0.9.6/perceval/backends/core/confluence.py` & `perceval-0.9.9/perceval/backends/core/confluence.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -50,15 +51,15 @@
     passing the URL os this server. The `url` will be set as the
     origin of the data.
 
     :param url: URL of the server
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.1'
+    version = '0.6.0'
 
     def __init__(self, url, tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
         self.client = ConfluenceClient(url)
@@ -302,15 +303,15 @@
         # Required arguments
         parser.parser.add_argument('url',
                                    help="URL of the Confluence server")
 
         return parser
 
 
-class ConfluenceClient:
+class ConfluenceClient(HttpClient):
     """Confluence REST API client.
 
     This class implements a client to retrieve contents from a
     Confluence server using its REST API.
 
     :param base_url: URL of the Confluence server
     """
@@ -334,15 +335,15 @@
 
     # Common values
     VCQL = "lastModified>='%(date)s' order by lastModified"
     VEXPAND = ['body.storage', 'history', 'version']
     VHISTORICAL = 'historical'
 
     def __init__(self, base_url):
-        self.base_url = base_url.rstrip('/')
+        super().__init__(base_url.rstrip('/'))
 
     def contents(self, from_date=DEFAULT_DATETIME,
                  offset=None, max_contents=MAX_CONTENTS):
         """Get the contents of a repository.
 
         This method returns an iterator that manages the pagination
         over contents. Take into account that the seconds of `from_date`
@@ -398,16 +399,15 @@
         """
         url = self.URL % {'base': self.base_url, 'resource': resource}
 
         logger.debug("Confluence client requests: %s params: %s",
                      resource, str(params))
 
         while True:
-            r = requests.get(url, params=params)
-            r.raise_for_status()
+            r = self.fetch(url, payload=params)
             yield r.text
 
             # Pagination is available when 'next' link exists
             j = r.json()
             if '_links' not in j:
                 break
             if 'next' not in j['_links']:
```

### Comparing `perceval-0.9.6/perceval/backends/core/redmine.py` & `perceval-0.9.9/perceval/backends/core/redmine.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -54,15 +55,15 @@
 
     :param url: URL of the server
     :param api_token: token needed to use the API
     :param max_issues:  maximum number of issues requested on the same query
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.2'
+    version = '0.6.0'
 
     def __init__(self, url, api_token=None, max_issues=MAX_ISSUES,
                  tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
@@ -375,15 +376,15 @@
         # Required arguments
         parser.parser.add_argument('url',
                                    help="URL of the Redmine server")
 
         return parser
 
 
-class RedmineClient:
+class RedmineClient(HttpClient):
     """Redmine API client.
 
     This class implements a client that retrieves issues from
     a Redmine server. Remine servers provides a REST API that
     returns its results in JSON format.
 
     :param base_url: URL of the Phabricator server
@@ -408,15 +409,15 @@
     CCHANGESETS = 'changesets'
     CCHILDREN = 'children'
     CJOURNALS = 'journals'
     CRELATIONS = 'relations'
     CWATCHERS = 'watchers'
 
     def __init__(self, base_url, api_token=None):
-        self.base_url = base_url.rstrip('/')
+        super().__init__(base_url.rstrip('/'))
         self.api_token = api_token
 
     def issues(self, from_date=DEFAULT_DATETIME,
                offset=None, max_issues=MAX_ISSUES):
         """Get the information of a list of issues.
 
         :param from_date: retrieve issues that where updated from that date;
@@ -486,11 +487,10 @@
 
         if self.api_token:
             params[self.PKEY] = self.api_token
 
         logger.debug("Redmine client requests: %s params: %s",
                      resource, str(params))
 
-        r = requests.get(url, params=params, verify=False)
-        r.raise_for_status()
+        r = self.fetch(url, payload=params, verify=False)
 
         return r.text
```

### Comparing `perceval-0.9.6/perceval/backends/core/mediawiki.py` & `perceval-0.9.9/perceval/backends/core/mediawiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 #
 
 import datetime
 import json
 import logging
 
 import dateutil
-import requests
 
 from grimoirelab.toolkit.datetime import datetime_to_utc, str_to_datetime
 from grimoirelab.toolkit.uris import urijoin
 
 from ...backend import (Backend,
                         BackendCommand,
                         BackendCommandArgumentParser,
                         metadata)
+from ...client import HttpClient
 from ...errors import BackendError, CacheError
 from ...utils import DEFAULT_DATETIME
 
 
 logger = logging.getLogger(__name__)
 
 MAX_RECENT_DAYS = 30  # max number of days included in MediaWiki recent changes
@@ -66,15 +66,15 @@
 
     Deleted pages are not analyzed.
 
     :param url: MediaWiki url
     :param tag: label used to mark the data
     :param cache: cache object to store raw data
     """
-    version = '0.5.1'
+    version = '0.6.0'
 
     def __init__(self, url, tag=None, cache=None):
         origin = url
 
         super().__init__(origin, tag=tag, cache=cache)
         self.url = url
         self.client = MediaWikiClient(url)
@@ -373,42 +373,39 @@
         else:
             logger.warning("Revisions not found in %s", reviews["query"]["pages"])
             logger.warning("for page: %s", page)
             page = None
         return page
 
 
-class MediaWikiClient:
+class MediaWikiClient(HttpClient):
     """MediaWiki API client.
 
     This class implements a simple client to retrieve pages from
     projects in a MediaWiki node.
 
     :param url: URL of mediawiki site: https://wiki.mozilla.org
 
     :raises HTTPError: when an error occurs doing the request
     """
 
     def __init__(self, url):
-        self.url = url
-        self.api_url = urijoin(self.url, "api.php")
+        super().__init__(urijoin(url, "api.php"))
         self.limit = "max"  # Always get the max number of items
 
     def call(self, params):
         """Run an API command.
         :param cgi: cgi command to run on the server
         :param params: dict with the HTTP parameters needed to run
             the given command
         """
         logger.debug("MediaWiki client calls API: %s params: %s",
-                     self.api_url, str(params))
-
-        req = requests.get(self.api_url, params=params)
-        req.raise_for_status()
+                     self.base_url, str(params))
 
+        req = self.fetch(self.base_url, payload=params)
         return req.text
 
     def get_namespaces(self):
         """ Retrieve all contents namespaces."""
 
         params = {
             "action": "query",
@@ -428,15 +425,15 @@
 
         try:
             res = self.call(params)
             siteinfo = json.loads(res)
             siteinfo = siteinfo["query"]["general"]
         except Exception:
             logger.error(res)
-            cause = "Wrong MediaWiki API: " + self.url
+            cause = "Wrong MediaWiki API: " + self.base_url
             raise BackendError(cause=cause)
 
         version = siteinfo['generator']
         # MediaWiki 1.28.0-wmf.7, MediaWiki 1.19alpha
         version = version.split(" ")[1]  # Removes MediaWiki
         version_major = int(version.split(".")[0])
         version_minor = int(version.split(".")[1][0:2])
```

### Comparing `perceval-0.9.6/perceval/backends/__init__.py` & `perceval-0.9.9/perceval/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/cache.py` & `perceval-0.9.9/perceval/cache.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/errors.py` & `perceval-0.9.9/perceval/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,20 @@
 
 class CacheError(BaseError):
     """Generic error for cache objects"""
 
     message = "%(cause)s"
 
 
+class HttpClientError(BaseError):
+    """Generic error for HTTP Cient"""
+
+    message = "%(cause)s"
+
+
 class RepositoryError(BaseError):
     """Generic error for repositories"""
 
     message = "%(cause)s"
 
 
 class RateLimitError(BaseError):
```

### Comparing `perceval-0.9.6/perceval/backend.py` & `perceval-0.9.9/perceval/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,26 +425,31 @@
     return _import_backends(modules)
 
 
 def _import_backends(modules):
     for module in modules:
         importlib.import_module(module)
 
-    bkls = _filter_classes(Backend.__subclasses__(), modules)
-    ckls = _filter_classes(BackendCommand.__subclasses__(), modules)
+    bkls = _find_classes(Backend, modules)
+    ckls = _find_classes(BackendCommand, modules)
 
     backends = {name: kls for name, kls in bkls}
     commands = {name: klass for name, klass in ckls}
 
     return backends, commands
 
 
-def _filter_classes(klasses, modules):
-    for kls in klasses:
+def _find_classes(parent, modules):
+    parents = parent.__subclasses__()
+
+    while parents:
+        kls = parents.pop()
+
         m = kls.__module__
 
         if m not in modules:
             continue
 
         name = m.split('.')[-1]
+        parents.extend(kls.__subclasses__())
 
         yield name, kls
```

### Comparing `perceval-0.9.6/perceval/__init__.py` & `perceval-0.9.9/perceval/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/perceval/utils.py` & `perceval-0.9.9/perceval/utils.py`

 * *Files identical despite different names*

### Comparing `perceval-0.9.6/setup.py` & `perceval-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,13 +77,14 @@
       ],
       install_requires=[
           'python-dateutil>=2.6.0',
           'requests>=2.7.0',
           'beautifulsoup4>=4.3.2',
           'feedparser>=5.1.3',
           'dulwich>=0.18.5',
+          'urllib3>=1.22',
           'grimoirelab-toolkit>=0.1.1'
       ],
       scripts=[
           'bin/perceval'
       ],
       zip_safe=False)
```

### Comparing `perceval-0.9.6/PKG-INFO` & `perceval-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: perceval
-Version: 0.9.6
+Version: 0.9.9
 Summary: Fetch data from software repositories
 Home-page: https://github.com/grimoirelab/perceval
 Author: Bitergia
 Author-email: sduenas@bitergia.com
 License: GPLv3
 Description-Content-Type: UNKNOWN
 Description: Perceval |Build Status| |Coverage Status| |PyPI version|
```

