# Comparing `tmp/BeyotekTools-0.0.1.tar.gz` & `tmp/BeyotekTools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyotekTools-0.0.1.tar", last modified: Sat Aug  5 22:13:23 2023, max compression
+gzip compressed data, was "BeyotekTools-0.0.2.tar", last modified: Sat Aug  5 22:48:21 2023, max compression
```

## Comparing `BeyotekTools-0.0.1.tar` & `BeyotekTools-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 22:13:23.481075 BeyotekTools-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      363 2023-08-05 22:13:23.481075 BeyotekTools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.1/README.md
--rw-rw-rw-   0        0        0      581 2023-08-05 22:09:40.000000 BeyotekTools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 22:13:23.482197 BeyotekTools-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 22:13:23.460896 BeyotekTools-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 22:13:23.466901 BeyotekTools-0.0.1/src/BeyotekTools/
--rw-rw-rw-   0        0        0        0 2023-08-05 21:33:00.000000 BeyotekTools-0.0.1/src/BeyotekTools/__init__.py
--rw-rw-rw-   0        0        0      651 2023-08-05 22:06:22.000000 BeyotekTools-0.0.1/src/BeyotekTools/speedlimit.py
-drwxrwxrwx   0        0        0        0 2023-08-05 22:13:23.479006 BeyotekTools-0.0.1/src/BeyotekTools.egg-info/
--rw-rw-rw-   0        0        0      363 2023-08-05 22:13:23.000000 BeyotekTools-0.0.1/src/BeyotekTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-08-05 22:13:23.000000 BeyotekTools-0.0.1/src/BeyotekTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 22:13:23.000000 BeyotekTools-0.0.1/src/BeyotekTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 22:13:23.000000 BeyotekTools-0.0.1/src/BeyotekTools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 22:13:23.479006 BeyotekTools-0.0.1/tests/
--rw-rw-rw-   0        0        0      155 2023-08-05 22:06:22.000000 BeyotekTools-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-08-05 22:48:21.775115 BeyotekTools-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      363 2023-08-05 22:48:21.775115 BeyotekTools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.2/README.md
+-rw-rw-rw-   0        0        0      581 2023-08-05 22:48:10.000000 BeyotekTools-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 22:48:21.776122 BeyotekTools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 22:48:21.759588 BeyotekTools-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 22:48:21.764589 BeyotekTools-0.0.2/src/BeyotekTools/
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:33:00.000000 BeyotekTools-0.0.2/src/BeyotekTools/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-08-05 22:46:29.000000 BeyotekTools-0.0.2/src/BeyotekTools/speedlimit.py
+drwxrwxrwx   0        0        0        0 2023-08-05 22:48:21.773120 BeyotekTools-0.0.2/src/BeyotekTools.egg-info/
+-rw-rw-rw-   0        0        0      363 2023-08-05 22:48:21.000000 BeyotekTools-0.0.2/src/BeyotekTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-08-05 22:48:21.000000 BeyotekTools-0.0.2/src/BeyotekTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 22:48:21.000000 BeyotekTools-0.0.2/src/BeyotekTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 22:48:21.000000 BeyotekTools-0.0.2/src/BeyotekTools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 22:48:21.774116 BeyotekTools-0.0.2/tests/
+-rw-rw-rw-   0        0        0      187 2023-08-05 22:47:15.000000 BeyotekTools-0.0.2/tests/test.py
```

### Comparing `BeyotekTools-0.0.1/LICENSE` & `BeyotekTools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.1/pyproject.toml` & `BeyotekTools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BeyotekTools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Beyotek", email="chuck@beyotek.com" },
 ]
 description = "Beyotek Tools"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `BeyotekTools-0.0.1/src/BeyotekTools/speedlimit.py` & `BeyotekTools-0.0.2/src/BeyotekTools/speedlimit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import time
 
-last_call_time = time.time()
+class limiter:
+    def __init__(self):
+        self.last_call_time = time.time()
+
+    def limit(self, milliseconds):
+        """
+        Slows down a loop by pausing for a given number of milliseconds since the last call.
+
+        Parameters:
+            milliseconds (float): Number of milliseconds to limit the loop's speed.
+
+        Returns:
+            None
+        """
+
+        current_time = time.time()
+        loop_time = (current_time - self.last_call_time) * 1000  # Convert to milliseconds
+        # TODO Add randomize time ability
+        if loop_time < milliseconds:
+            time.sleep((milliseconds - loop_time) / 1000)  # Convert back to seconds
 
-
-def speedlimit(milliseconds):
-    """
-    Slows down a loop by pausing for a given number of milliseconds since the last call.
-
-    Parameters:
-        milliseconds (float): Number of milliseconds to limit the loop's speed.
-
-    Returns:
-        None
-    """
-    global last_call_time
-    current_time = time.time()
-    loop_time = (current_time - last_call_time) * 1000  # Convert to milliseconds
-    # TODO Add randomize time ability
-    if loop_time < milliseconds:
-        time.sleep((milliseconds - loop_time) / 1000)  # Convert back to seconds
-
-    last_call_time = time.time()
+        self.last_call_time = time.time()
```

