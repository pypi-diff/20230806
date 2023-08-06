# Comparing `tmp/datoso-0.3.2.tar.gz` & `tmp/datoso-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.3.2.tar", last modified: Thu Jul 13 14:06:41 2023, max compression
+gzip compressed data, was "datoso-0.3.3.tar", last modified: Sat Jul 15 23:32:35 2023, max compression
```

## Comparing `datoso-0.3.2.tar` & `datoso-0.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 14:06:26.000000 datoso-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 14:06:26.000000 datoso-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-13 14:06:41.347535 datoso-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-13 14:06:26.000000 datoso-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-13 14:06:26.000000 datoso-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 14:06:41.351535 datoso-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.343535 datoso-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-07-13 14:06:26.000000 datoso-0.3.2/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:06:41.347535 datoso-0.3.2/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-13 14:06:41.000000 datoso-0.3.2/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-13 14:06:41.000000 datoso-0.3.2/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:06:41.000000 datoso-0.3.2/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 14:06:41.000000 datoso-0.3.2/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-13 14:06:41.000000 datoso-0.3.2/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 14:06:41.000000 datoso-0.3.2/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-15 23:32:23.000000 datoso-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 23:32:23.000000 datoso-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-15 23:32:35.928523 datoso-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 23:32:23.000000 datoso-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-15 23:32:23.000000 datoso-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-15 23:32:35.928523 datoso-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.920523 datoso-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.924523 datoso-0.3.3/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.924523 datoso-0.3.3/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.924523 datoso-0.3.3/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.928523 datoso-0.3.3/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-07-15 23:32:23.000000 datoso-0.3.3/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:32:35.924523 datoso-0.3.3/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-15 23:32:35.000000 datoso-0.3.3/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-15 23:32:35.000000 datoso-0.3.3/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 23:32:35.000000 datoso-0.3.3/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 23:32:35.000000 datoso-0.3.3/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-15 23:32:35.000000 datoso-0.3.3/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 23:32:35.000000 datoso-0.3.3/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.3.2/LICENSE` & `datoso-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/PKG-INFO` & `datoso-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.3.2/README.md` & `datoso-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/pyproject.toml` & `datoso-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/__main__.py` & `datoso-0.3.3/src/datoso/__main__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/actions/processor.py` & `datoso-0.3.3/src/datoso/actions/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 # pylint: disable=too-few-public-methods
 from contextlib import suppress
 import os
 import shutil
 from dateutil import parser
 from datoso.configuration import config
-from datoso.helpers import FileUtils
+from datoso.helpers import FileUtils, compare_dates
 from datoso.repositories.dedupe import Dedupe
 from datoso.database.models.datfile import Dat
 
 class Processor:
     """ Process actions. """
     _previous = None
     actions = []
@@ -77,18 +77,21 @@
     database = None
     def process(self):
         """ Delete old dat file. """
         from datoso.database.models.datfile import Dat
         self.database = Dat(seed=self.previous['seed'], name=self.previous['name'])
         self.database.load()
         olddat = self.database.dict()
-        if self.previous and getattr(self.database, 'date', None) and self.previous.get('date', None) and parser.parse(self.database.date, fuzzy=True) > parser.parse(self.previous['date'], fuzzy=True):
-            result = "No Action Taken, Newer Found"
-            self.stop = True
-            return result
+        try:
+            if self.previous and getattr(self.database, 'date', None) and self.previous.get('date', None) and compare_dates(self.database.date, self.previous['date']):
+                result = "No Action Taken, Newer Found"
+                self.stop = True
+                return result
+        except ValueError:
+            print(self.database.date, self.previous['date'])
 
         result = None
         if 'new_file' in olddat and olddat['new_file']:
             try:
                 shutil.rmtree(olddat['new_file'])
             except NotADirectoryError:
                 with suppress(FileNotFoundError):
@@ -127,15 +130,15 @@
                     if not old_file:
                         result = "Created"
                     elif old_file != new_file:
                         result = "Updated"
                     elif config.getboolean('GENERAL', 'Overwrite', fallback=False):
                         result = "Overwritten"
                     try:
-                        if getattr(self.database, 'date', None) and self.previous.get('date', None) and parser.parse(self.database.date, fuzzy=True) > parser.parse(self.previous['date'], fuzzy=True):
+                        if getattr(self.database, 'date', None) and self.previous.get('date', None) and compare_dates(self.database.date, self.previous['date']):
                             result = "No Action Taken, Newer Found"
                         else:
                             self.previous['new_file'] = destination
                             FileUtils.copy(origin, destination)
                     except ValueError:
                         pass
                 else:
```

### Comparing `datoso-0.3.2/src/datoso/commands/doctor.py` & `datoso-0.3.3/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/commands/seed.py` & `datoso-0.3.3/src/datoso/commands/seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/configuration/folder_helper.py` & `datoso-0.3.3/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/configuration/logger.py` & `datoso-0.3.3/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/database/__init__.py` & `datoso-0.3.3/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/database/models/datfile.py` & `datoso-0.3.3/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/database/seeds/dat_repos.py` & `datoso-0.3.3/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/database/seeds/dat_rules.py` & `datoso-0.3.3/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/datoso.ini` & `datoso-0.3.3/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/helpers/__init__.py` & `datoso-0.3.3/src/datoso/helpers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -141,8 +141,19 @@
     XML = '<?xml'
     CLRMAMEPRO = 'clrma'
 
 def show_progress(block_num, block_size, total_size):
     if total_size != -1:
         print(f' {block_num * block_size / total_size:.1%}', end="\r")
     else:
-        print(f' {block_num * block_size / 1024 / 1024:.1f} MB', end="\r")
+        print(f' {block_num * block_size / 1024 / 1024:.1f} MB', end="\r")
+
+def compare_dates(date1, date2):
+    if date1 is None or date2 is None:
+        return False
+    if isinstance(date1, str):
+        date1 = date1.split(' ')[0]
+        date1 = parser.parse(date1, fuzzy=True)
+    if isinstance(date2, str):
+        date2 = date2.split(' ')[0]
+        date2 = parser.parse(date2, fuzzy=True)
+    return date1 > date2
```

### Comparing `datoso-0.3.2/src/datoso/helpers/executor.py` & `datoso-0.3.3/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/helpers/plugins.py` & `datoso-0.3.3/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/repositories/dat.py` & `datoso-0.3.3/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/repositories/dedupe.py` & `datoso-0.3.3/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/seeds/unknown_seed.py` & `datoso-0.3.3/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/seeds.txt` & `datoso-0.3.3/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso/systems.json` & `datoso-0.3.3/src/datoso/systems.json`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso.egg-info/PKG-INFO` & `datoso-0.3.3/src/datoso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.3.2/src/datoso.egg-info/SOURCES.txt` & `datoso-0.3.3/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.3.2/src/datoso.egg-info/requires.txt` & `datoso-0.3.3/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

