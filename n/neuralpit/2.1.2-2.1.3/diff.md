# Comparing `tmp/neuralpit-2.1.2.tar.gz` & `tmp/neuralpit-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-2.1.2.tar", last modified: Thu Aug  3 05:21:21 2023, max compression
+gzip compressed data, was "neuralpit-2.1.3.tar", last modified: Sun Aug  6 17:32:32 2023, max compression
```

## Comparing `neuralpit-2.1.2.tar` & `neuralpit-2.1.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 05:20:52.000000 neuralpit-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-08-03 05:21:20.993473 neuralpit-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-08-03 05:20:52.000000 neuralpit-2.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)      963 2023-08-03 05:20:52.000000 neuralpit-2.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 05:21:20.993473 neuralpit-2.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      620 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5018 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/services/conversation.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/services/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit/utils/
--rw-r--r--   0 root         (0) root         (0)      580 2023-08-03 05:20:52.000000 neuralpit-2.1.2/src/neuralpit/utils/streamer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-08-03 05:21:20.000000 neuralpit-2.1.2/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 05:21:20.993473 neuralpit-2.1.2/test/
--rw-r--r--   0 root         (0) root         (0)      411 2023-08-03 05:20:52.000000 neuralpit-2.1.2/test/testCreateConversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.669192 neuralpit-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 17:32:02.000000 neuralpit-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-08-06 17:32:32.669192 neuralpit-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-06 17:32:02.000000 neuralpit-2.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-08-06 17:32:02.000000 neuralpit-2.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 17:32:32.669192 neuralpit-2.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.665192 neuralpit-2.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.665192 neuralpit-2.1.3/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-08-06 17:32:02.000000 neuralpit-2.1.3/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.669192 neuralpit-2.1.3/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 17:32:02.000000 neuralpit-2.1.3/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-08-06 17:32:02.000000 neuralpit-2.1.3/src/neuralpit/services/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-08-06 17:32:02.000000 neuralpit-2.1.3/src/neuralpit/services/conversion.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-08-06 17:32:02.000000 neuralpit-2.1.3/src/neuralpit/services/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.669192 neuralpit-2.1.3/src/neuralpit/utils/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-08-06 17:32:02.000000 neuralpit-2.1.3/src/neuralpit/utils/streamer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.665192 neuralpit-2.1.3/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-08-06 17:32:32.000000 neuralpit-2.1.3/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-08-06 17:32:32.000000 neuralpit-2.1.3/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 17:32:32.000000 neuralpit-2.1.3/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-08-06 17:32:32.000000 neuralpit-2.1.3/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-06 17:32:32.000000 neuralpit-2.1.3/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:32:32.669192 neuralpit-2.1.3/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-08-06 17:32:02.000000 neuralpit-2.1.3/test/testCreateConversation.py
```

### Comparing `neuralpit-2.1.2/PKG-INFO` & `neuralpit-2.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.1.2
+Version: 2.1.3
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `neuralpit-2.1.2/pyproject.toml` & `neuralpit-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "2.1.2"
+version = "2.1.3"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-2.1.2/src/neuralpit/__init__.py` & `neuralpit-2.1.3/src/neuralpit/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.2/src/neuralpit/services/conversation.py` & `neuralpit-2.1.3/src/neuralpit/services/conversation.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.2/src/neuralpit/services/conversion.py` & `neuralpit-2.1.3/src/neuralpit/services/conversion.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.2/src/neuralpit/utils/streamer.py` & `neuralpit-2.1.3/src/neuralpit/utils/streamer.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.1.2/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.1.3/src/neuralpit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.1.2
+Version: 2.1.3
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

