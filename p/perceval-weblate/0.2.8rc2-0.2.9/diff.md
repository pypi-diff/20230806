# Comparing `tmp/perceval_weblate-0.2.8rc2.tar.gz` & `tmp/perceval_weblate-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_weblate-0.2.8rc2.tar", max compression
+gzip compressed data, was "perceval_weblate-0.2.9.tar", max compression
```

## Comparing `perceval_weblate-0.2.8rc2.tar` & `perceval_weblate-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      119 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/LICENSE
--rw-r--r--   0        0        0      928 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/NEWS
--rw-r--r--   0        0        0     2187 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/README.md
--rw-r--r--   0        0        0        0 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/perceval/backends/weblate/__init__.py
--rw-r--r--   0        0        0       91 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/perceval/backends/weblate/_version.py
--rw-r--r--   0        0        0    14043 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/perceval/backends/weblate/weblate.py
--rw-r--r--   0        0        0     1390 2023-04-21 09:53:12.874931 perceval_weblate-0.2.8rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/__init__.py
--rw-r--r--   0        0        0     1832 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/base.py
--rw-r--r--   0        0        0      981 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes.json
--rw-r--r--   0        0        0     1922 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes_archived.json
--rw-r--r--   0        0        0     8490 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes_expected.json
--rw-r--r--   0        0        0     1086 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes_page_2.json
--rw-r--r--   0        0        0      719 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_unit.json
--rw-r--r--   0        0        0      359 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_user_1.json
--rw-r--r--   0        0        0      354 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_user_2.json
--rw-r--r--   0        0        0       31 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_user_no_permission.json
--rw-r--r--   0        0        0     1007 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/run_tests.py
--rw-r--r--   0        0        0    16895 2023-04-21 09:53:12.878931 perceval_weblate-0.2.8rc2/tests/test_weblate.py
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 perceval_weblate-0.2.8rc2/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1104 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/NEWS
+-rw-r--r--   0        0        0     2187 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/perceval/backends/weblate/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/perceval/backends/weblate/_version.py
+-rw-r--r--   0        0        0    14043 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/perceval/backends/weblate/weblate.py
+-rw-r--r--   0        0        0     1385 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     1832 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/base.py
+-rw-r--r--   0        0        0      981 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes.json
+-rw-r--r--   0        0        0     1922 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_archived.json
+-rw-r--r--   0        0        0     8490 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_expected.json
+-rw-r--r--   0        0        0     1086 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_page_2.json
+-rw-r--r--   0        0        0      719 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_unit.json
+-rw-r--r--   0        0        0      359 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_user_1.json
+-rw-r--r--   0        0        0      354 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_user_2.json
+-rw-r--r--   0        0        0       31 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_user_no_permission.json
+-rw-r--r--   0        0        0     1007 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/run_tests.py
+-rw-r--r--   0        0        0    16895 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/test_weblate.py
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 perceval_weblate-0.2.9/PKG-INFO
```

### Comparing `perceval_weblate-0.2.8rc2/LICENSE` & `perceval_weblate-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/NEWS` & `perceval_weblate-0.2.9/NEWS`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+  ## perceval-weblate 0.2.9 - (2023-04-26)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-weblate 0.2.8 - (2023-04-21)
+  
+  * Update Poetry's package dependencies
+
   ## perceval-weblate 0.2.7 - (2023-02-03)
   
   * Update Poetry's package dependencies
 
   ## perceval-weblate 0.2.6 - (2023-02-01)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_weblate-0.2.8rc2/README.md` & `perceval_weblate-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/perceval/backends/weblate/weblate.py` & `perceval_weblate-0.2.9/perceval/backends/weblate/weblate.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/pyproject.toml` & `perceval_weblate-0.2.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-weblate"
-version = "0.2.8-rc.2"
+version = "0.2.9"
 description = "Bundle of Perceval backends for Weblate."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_weblate-0.2.8rc2/tests/base.py` & `perceval_weblate-0.2.9/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes.json` & `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes_archived.json` & `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_archived.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes_expected.json` & `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_expected.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_changes_page_2.json` & `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/data/weblate/weblate_unit.json` & `perceval_weblate-0.2.9/tests/data/weblate/weblate_unit.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/run_tests.py` & `perceval_weblate-0.2.9/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/tests/test_weblate.py` & `perceval_weblate-0.2.9/tests/test_weblate.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.8rc2/PKG-INFO` & `perceval_weblate-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-weblate
-Version: 0.2.8rc2
+Version: 0.2.9
 Summary: Bundle of Perceval backends for Weblate.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

