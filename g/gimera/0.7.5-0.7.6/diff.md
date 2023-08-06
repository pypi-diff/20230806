# Comparing `tmp/gimera-0.7.5.tar.gz` & `tmp/gimera-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.7.5.tar", last modified: Sun Aug  6 13:29:32 2023, max compression
+gzip compressed data, was "gimera-0.7.6.tar", last modified: Sun Aug  6 13:46:09 2023, max compression
```

## Comparing `gimera-0.7.5.tar` & `gimera-0.7.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:29:32.354244 gimera-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 13:28:38.000000 gimera-0.7.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 13:29:32.354244 gimera-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-06 13:28:38.000000 gimera-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:29:32.354244 gimera-0.7.5/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28893 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-08-06 13:28:38.000000 gimera-0.7.5/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:29:32.354244 gimera-0.7.5/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 13:29:32.000000 gimera-0.7.5/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 13:29:32.000000 gimera-0.7.5/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:29:32.000000 gimera-0.7.5/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 13:29:32.000000 gimera-0.7.5/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 13:29:32.000000 gimera-0.7.5/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 13:29:32.000000 gimera-0.7.5/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-06 13:29:32.354244 gimera-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-06 13:28:38.000000 gimera-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:46:09.415567 gimera-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 13:45:20.000000 gimera-0.7.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 13:46:09.415567 gimera-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-06 13:45:20.000000 gimera-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:46:09.415567 gimera-0.7.6/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28893 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:46:09.415567 gimera-0.7.6/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-06 13:46:09.415567 gimera-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-06 13:45:20.000000 gimera-0.7.6/setup.py
```

### Comparing `gimera-0.7.5/LICENSE.txt` & `gimera-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/PKG-INFO` & `gimera-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.5
+Version: 0.7.6
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.5/README.md` & `gimera-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/gimera/config.py` & `gimera-0.7.6/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/gimera/gimera.py` & `gimera-0.7.6/gimera/gimera.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/gimera/gitcommands.py` & `gimera-0.7.6/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/gimera/patches.py` & `gimera-0.7.6/gimera/patches.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/gimera/repo.py` & `gimera-0.7.6/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.5/gimera/tools.py` & `gimera-0.7.6/gimera/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,30 +130,34 @@
     click.secho(msg, fg="yellow")
     res = click.confirm("Continue?", default=True)
     if not res and raise_exception:
         _raise_error("Aborted by user")
     return res
 
 
-def try_rm_tree(path):
-    if not path.exists():
-        return
-    MAX = 3
-    sl = 5
-    for i in range(MAX):
+@contextmanager
+def retry(attempts=3, sleep=5):
+    for i in range(attempts):
         try:
-            shutil.rmtree(path)
-        except:
-            time.sleep(sl)
-            if i > MAX:
+            yield
+        except Exception:
+            if i == attempts - 1:
                 raise
+            time.sleep(sleep)
         else:
             break
 
 
+def try_rm_tree(path):
+    if not path.exists():
+        return
+    with retry():
+        shutil.rmtree(path)
+
+
 @contextmanager
 def temppath():
     path = Path(tempfile.mktemp(suffix="."))
     try:
         path.mkdir()
         yield path
     finally:
```

### Comparing `gimera-0.7.5/gimera.egg-info/PKG-INFO` & `gimera-0.7.6/gimera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.5
+Version: 0.7.6
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.5/setup.py` & `gimera-0.7.6/setup.py`

 * *Files identical despite different names*

