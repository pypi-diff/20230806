# Comparing `tmp/FSRS-Optimizer-4.6.0.tar.gz` & `tmp/FSRS-Optimizer-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.6.0.tar", last modified: Tue Aug  1 10:16:12 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.7.0.tar", last modified: Sun Aug  6 05:27:31 2023, max compression
```

## Comparing `FSRS-Optimizer-4.6.0.tar` & `FSRS-Optimizer-4.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.360887 FSRS-Optimizer-4.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 10:16:12.000000 FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:16:12.364887 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52871 2023-08-01 10:15:57.000000 FSRS-Optimizer-4.6.0/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.023194 FSRS-Optimizer-4.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.023194 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 05:27:31.000000 FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:27:31.027194 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53118 2023-08-06 05:27:17.000000 FSRS-Optimizer-4.7.0/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.6.0/LICENSE` & `FSRS-Optimizer-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.6.0/PKG-INFO` & `FSRS-Optimizer-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.6.0
+Version: 4.7.0
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.6.0/README.md` & `FSRS-Optimizer-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.6.0/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.7.0/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.6.0
+Version: 4.7.0
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FSRS Optimizer
```

### Comparing `FSRS-Optimizer-4.6.0/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.7.0/src/fsrs_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.6.0/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.7.0/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             return stabilities.tolist(), difficulties.tolist()
 
 """Used to store all the results from FSRS related functions"""
 class Optimizer:
     def __init__(self) -> None:
         tqdm.pandas()
 
-    def anki_extract(self, filename: str, filter_out_suspended_cards: bool = False):
+    def anki_extract(self, filename: str, filter_out_suspended_cards: bool = False, filter_out_flags: List[int] = []):
         """Step 1"""
         # Extract the collection file or deck file to get the .anki21 database.
         with zipfile.ZipFile(f'{filename}', 'r') as zip_ref:
             zip_ref.extractall('./')
             tqdm.write("Deck file extracted successfully!")
 
         if os.path.isfile("collection.anki21b"):
@@ -330,22 +330,27 @@
         elif os.path.isfile("collection.anki21"):
             con = sqlite3.connect("collection.anki21")
         elif os.path.isfile("collection.anki2"):
             con = sqlite3.connect("collection.anki2")
         else:
             raise Exception("Collection not exist!")
         cur = con.cursor()
+
+        def flags2str(flags: List[int]) -> str:
+            return f"({','.join(map(str, flags))})"
+        
         res = cur.execute(f"""
         SELECT *
         FROM revlog
         WHERE cid IN (
             SELECT id
             FROM cards
             WHERE queue != 0
             {"AND queue != -1" if filter_out_suspended_cards else ""}
+            {"AND flags NOT IN %s" % flags2str(filter_out_flags) if len(filter_out_flags) > 0 else ""}
         )
         """
         )
         revlog = res.fetchall()
         if len(revlog) == 0:
             raise Exception("No review log found!")
         df = pd.DataFrame(revlog)
```

