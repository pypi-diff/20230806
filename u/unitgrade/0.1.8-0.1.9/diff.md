# Comparing `tmp/unitgrade-0.1.8.tar.gz` & `tmp/unitgrade-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\tuhe\Documents\unitgrade\dist\tmps2hbyvjd\unitgrade-0.1.8.tar", last modified: Fri Sep 17 12:59:57 2021, max compression
+gzip compressed data, was "C:\Users\tuhe\Documents\unitgrade\dist\tmpivoankm2\unitgrade-0.1.9.tar", last modified: Fri Sep 17 13:03:30 2021, max compression
```

## Comparing `unitgrade-0.1.8.tar` & `unitgrade-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-09-17 12:59:57.372674 unitgrade-0.1.8/
--rw-rw-rw-   0        0        0     1091 2021-09-02 10:11:20.000000 unitgrade-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    14357 2021-09-17 12:59:57.370659 unitgrade-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    13756 2021-09-06 22:42:26.000000 unitgrade-0.1.8/README.md
--rw-rw-rw-   0        0        0      108 2021-09-02 10:05:30.000000 unitgrade-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-09-17 12:59:57.372674 unitgrade-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1312 2021-09-16 09:19:14.000000 unitgrade-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-17 12:59:57.224615 unitgrade-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2021-09-17 12:59:57.295675 unitgrade-0.1.8/src/unitgrade/
--rw-rw-rw-   0        0        0     1646 2021-09-17 11:44:49.000000 unitgrade-0.1.8/src/unitgrade/__init__.py
--rw-rw-rw-   0        0        0    12166 2021-09-17 12:59:22.000000 unitgrade-0.1.8/src/unitgrade/evaluate.py
--rw-rw-rw-   0        0        0    21244 2021-09-17 12:54:29.000000 unitgrade-0.1.8/src/unitgrade/framework.py
--rw-rw-rw-   0        0        0     7445 2021-09-17 11:47:34.000000 unitgrade-0.1.8/src/unitgrade/utils.py
--rw-rw-rw-   0        0        0       21 2021-09-17 12:59:36.000000 unitgrade-0.1.8/src/unitgrade/version.py
-drwxrwxrwx   0        0        0        0 2021-09-17 12:59:57.366661 unitgrade-0.1.8/src/unitgrade.egg-info/
--rw-rw-rw-   0        0        0    14357 2021-09-17 12:59:57.000000 unitgrade-0.1.8/src/unitgrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2021-09-17 12:59:57.000000 unitgrade-0.1.8/src/unitgrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-17 12:59:57.000000 unitgrade-0.1.8/src/unitgrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2021-09-17 12:59:57.000000 unitgrade-0.1.8/src/unitgrade.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-09-17 12:59:57.000000 unitgrade-0.1.8/src/unitgrade.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-09-17 13:03:30.098349 unitgrade-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2021-09-02 10:11:20.000000 unitgrade-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    14357 2021-09-17 13:03:30.096348 unitgrade-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13756 2021-09-06 22:42:26.000000 unitgrade-0.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-02 10:05:30.000000 unitgrade-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2021-09-17 13:03:30.099349 unitgrade-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1312 2021-09-16 09:19:14.000000 unitgrade-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-17 13:03:29.875762 unitgrade-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2021-09-17 13:03:30.006543 unitgrade-0.1.9/src/unitgrade/
+-rw-rw-rw-   0        0        0     1646 2021-09-17 11:44:49.000000 unitgrade-0.1.9/src/unitgrade/__init__.py
+-rw-rw-rw-   0        0        0    12166 2021-09-17 12:59:22.000000 unitgrade-0.1.9/src/unitgrade/evaluate.py
+-rw-rw-rw-   0        0        0    21309 2021-09-17 13:03:04.000000 unitgrade-0.1.9/src/unitgrade/framework.py
+-rw-rw-rw-   0        0        0     7445 2021-09-17 11:47:34.000000 unitgrade-0.1.9/src/unitgrade/utils.py
+-rw-rw-rw-   0        0        0       21 2021-09-17 13:02:05.000000 unitgrade-0.1.9/src/unitgrade/version.py
+drwxrwxrwx   0        0        0        0 2021-09-17 13:03:30.091351 unitgrade-0.1.9/src/unitgrade.egg-info/
+-rw-rw-rw-   0        0        0    14357 2021-09-17 13:03:29.000000 unitgrade-0.1.9/src/unitgrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2021-09-17 13:03:29.000000 unitgrade-0.1.9/src/unitgrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-17 13:03:29.000000 unitgrade-0.1.9/src/unitgrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2021-09-17 13:03:29.000000 unitgrade-0.1.9/src/unitgrade.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-09-17 13:03:29.000000 unitgrade-0.1.9/src/unitgrade.egg-info/top_level.txt
```

### Comparing `unitgrade-0.1.8/LICENSE` & `unitgrade-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unitgrade-0.1.8/PKG-INFO` & `unitgrade-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitgrade
-Version: 0.1.8
+Version: 0.1.9
 Summary: A student homework/exam evaluation framework build on pythons unittest framework.
 Home-page: https://lab.compute.dtu.dk/tuhe/unitgrade
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/unitgrade/issues
 Platform: UNKNOWN
```

### Comparing `unitgrade-0.1.8/README.md` & `unitgrade-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `unitgrade-0.1.8/setup.py` & `unitgrade-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `unitgrade-0.1.8/src/unitgrade/__init__.py` & `unitgrade-0.1.9/src/unitgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `unitgrade-0.1.8/src/unitgrade/evaluate.py` & `unitgrade-0.1.9/src/unitgrade/evaluate.py`

 * *Files identical despite different names*

### Comparing `unitgrade-0.1.8/src/unitgrade/framework.py` & `unitgrade-0.1.9/src/unitgrade/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,22 @@
 
     def addFailure(self, test, err):
         super(unittest.TextTestResult, self).addFailure(test, err)
         self.cc_terminate(success=False)
 
     def addSuccess(self, test: unittest.case.TestCase) -> None:
         # test._get_outcome()
-        o = test._get_outcome()
+
         msg = None
-        if isinstance(o, dict):
-            key = (test.cache_id(), "return")
-            if key in o:
-                msg = test._get_outcome()[key]
+        if hasattr(test, '_get_outcome'):
+            o = test._get_outcome()
+            if isinstance(o, dict):
+                key = (test.cache_id(), "return")
+                if key in o:
+                    msg = test._get_outcome()[key]
 
         self.successes.append((test, msg))  # (test, message) (to be consistent with failures and errors).
         self.cc_terminate()
 
     def cc_terminate(self, success=True):
         if self.show_progress_bar or True:
             tsecs = np.round(self.cc.terminate(), 2)
```

### Comparing `unitgrade-0.1.8/src/unitgrade/utils.py` & `unitgrade-0.1.9/src/unitgrade/utils.py`

 * *Files identical despite different names*

### Comparing `unitgrade-0.1.8/src/unitgrade.egg-info/PKG-INFO` & `unitgrade-0.1.9/src/unitgrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitgrade
-Version: 0.1.8
+Version: 0.1.9
 Summary: A student homework/exam evaluation framework build on pythons unittest framework.
 Home-page: https://lab.compute.dtu.dk/tuhe/unitgrade
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/unitgrade/issues
 Platform: UNKNOWN
```

