# Comparing `tmp/pypomes_events-0.1.0.tar.gz` & `tmp/pypomes_events-0.1.1.tar.gz`

## Comparing `pypomes_events-0.1.0.tar` & `pypomes_events-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/src/pypomes_events/__init__.py
--rw-r--r--   0        0        0    19075 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/src/pypomes_events/publisher_pomes.py
--rw-r--r--   0        0        0    19954 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/src/pypomes_events/subscriber_pomes.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pypomes_events-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/src/pypomes_events/__init__.py
+-rw-r--r--   0        0        0    19075 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/src/pypomes_events/publisher_pomes.py
+-rw-r--r--   0        0        0    19954 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/src/pypomes_events/subscriber_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 pypomes_events-0.1.1/PKG-INFO
```

### Comparing `pypomes_events-0.1.0/src/pypomes_events/__init__.py` & `pypomes_events-0.1.1/src/pypomes_events/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_events-0.1.0/src/pypomes_events/publisher_pomes.py` & `pypomes_events-0.1.1/src/pypomes_events/publisher_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_events-0.1.0/src/pypomes_events/subscriber_pomes.py` & `pypomes_events-0.1.1/src/pypomes_events/subscriber_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_events-0.1.0/LICENSE` & `pypomes_events-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_events-0.1.0/pyproject.toml` & `pypomes_events-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_events"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (event handling modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "asn1crypto>=1.5.1",
-    "pip>=23.3.1",
+    "pip>=23.2.1",
     "pika>=1.3.2",
     "pypomes_core>=0.2.3",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_events-0.1.0/PKG-INFO` & `pypomes_events-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pypomes_events
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of Python pomes, pennyeach (event handling modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Events
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Events/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: asn1crypto>=1.5.1
 Requires-Dist: pika>=1.3.2
-Requires-Dist: pip>=23.3.1
+Requires-Dist: pip>=23.2.1
 Requires-Dist: pypomes-core>=0.2.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

