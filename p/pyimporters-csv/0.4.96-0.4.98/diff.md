# Comparing `tmp/pyimporters-csv-0.4.96.tar.gz` & `tmp/pyimporters-csv-0.4.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimporters-csv-0.4.96.tar", last modified: Thu Feb 24 16:50:48 2022, max compression
+gzip compressed data, was "pyimporters-csv-0.4.98.tar", last modified: Thu Feb 24 17:06:51 2022, max compression
```

## Comparing `pyimporters-csv-0.4.96.tar` & `pyimporters-csv-0.4.98.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       97 2021-11-23 15:54:27.958527 pyimporters-csv-0.4.96/.dockerignore
--rw-r--r--   0        0        0      147 2021-11-23 15:54:27.958527 pyimporters-csv-0.4.96/.gitignore
--rw-r--r--   0        0        0      466 2021-11-23 15:54:27.959527 pyimporters-csv-0.4.96/Dockerfile
--rw-r--r--   0        0        0    10065 2022-02-24 16:48:19.467151 pyimporters-csv-0.4.96/Jenkinsfile
--rw-r--r--   0        0        0      148 2021-11-23 15:54:27.960527 pyimporters-csv-0.4.96/README.md
--rw-r--r--   0        0        0       61 2022-02-24 16:50:46.535021 pyimporters-csv-0.4.96/pyimporters_csv/__init__.py
--rw-r--r--   0        0        0     5042 2021-11-23 15:54:27.965527 pyimporters-csv-0.4.96/pyimporters_csv/csv.py
--rw-r--r--   0        0        0     4624 2021-11-23 15:54:27.968527 pyimporters-csv-0.4.96/pyimporters_csv/excel.py
--rw-r--r--   0        0        0     1635 2021-11-23 15:54:27.969527 pyimporters-csv-0.4.96/pyimporters_csv/text.py
--rw-r--r--   0        0        0     2164 2021-11-23 15:54:27.970527 pyimporters-csv-0.4.96/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-23 15:54:27.970527 pyimporters-csv-0.4.96/tests/__init__.py
--rw-r--r--   0        0        0    52920 2021-11-23 15:54:27.971527 pyimporters-csv-0.4.96/tests/data/Digestion.csv
--rw-r--r--   0        0        0    66048 2021-11-23 15:54:27.972527 pyimporters-csv-0.4.96/tests/data/Digestion.xls
--rw-r--r--   0        0        0    24029 2021-11-23 15:54:27.972527 pyimporters-csv-0.4.96/tests/data/Digestion.xlsx
--rw-r--r--   0        0        0    15103 2021-11-23 15:54:27.975527 pyimporters-csv-0.4.96/tests/data/Digestion.zip
--rw-r--r--   0        0        0    65555 2021-11-23 15:54:27.978527 pyimporters-csv-0.4.96/tests/data/Liste-des-codes-APE-NAF-excel-2017.xlsx
--rw-r--r--   0        0        0     2605 2021-11-23 15:54:27.980527 pyimporters-csv-0.4.96/tests/data/currencies.txt
--rw-r--r--   0        0        0     1536 2021-11-23 15:54:27.986528 pyimporters-csv-0.4.96/tests/data/currencies.zip
--rw-r--r--   0        0        0     5386 2021-11-23 15:54:27.988528 pyimporters-csv-0.4.96/tests/data/lexicon.xlsx.zip
--rw-r--r--   0        0        0     1450 2021-11-23 15:54:27.990527 pyimporters-csv-0.4.96/tests/test_csv.py
--rw-r--r--   0        0        0     2520 2021-11-23 15:54:27.993528 pyimporters-csv-0.4.96/tests/test_excel.py
--rw-r--r--   0        0        0      955 2021-11-23 15:54:27.998528 pyimporters-csv-0.4.96/tests/test_text.py
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 pyimporters-csv-0.4.96/setup.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 pyimporters-csv-0.4.96/PKG-INFO
+-rw-r--r--   0        0        0       97 2021-11-23 15:54:27.958527 pyimporters-csv-0.4.98/.dockerignore
+-rw-r--r--   0        0        0      147 2021-11-23 15:54:27.958527 pyimporters-csv-0.4.98/.gitignore
+-rw-r--r--   0        0        0      466 2021-11-23 15:54:27.959527 pyimporters-csv-0.4.98/Dockerfile
+-rw-r--r--   0        0        0    10228 2022-02-24 17:04:54.687362 pyimporters-csv-0.4.98/Jenkinsfile
+-rw-r--r--   0        0        0      148 2021-11-23 15:54:27.960527 pyimporters-csv-0.4.98/README.md
+-rw-r--r--   0        0        0       61 2022-02-24 17:06:49.664389 pyimporters-csv-0.4.98/pyimporters_csv/__init__.py
+-rw-r--r--   0        0        0     5042 2021-11-23 15:54:27.965527 pyimporters-csv-0.4.98/pyimporters_csv/csv.py
+-rw-r--r--   0        0        0     4624 2021-11-23 15:54:27.968527 pyimporters-csv-0.4.98/pyimporters_csv/excel.py
+-rw-r--r--   0        0        0     1635 2021-11-23 15:54:27.969527 pyimporters-csv-0.4.98/pyimporters_csv/text.py
+-rw-r--r--   0        0        0     2164 2021-11-23 15:54:27.970527 pyimporters-csv-0.4.98/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-23 15:54:27.970527 pyimporters-csv-0.4.98/tests/__init__.py
+-rw-r--r--   0        0        0    52920 2021-11-23 15:54:27.971527 pyimporters-csv-0.4.98/tests/data/Digestion.csv
+-rw-r--r--   0        0        0    66048 2021-11-23 15:54:27.972527 pyimporters-csv-0.4.98/tests/data/Digestion.xls
+-rw-r--r--   0        0        0    24029 2021-11-23 15:54:27.972527 pyimporters-csv-0.4.98/tests/data/Digestion.xlsx
+-rw-r--r--   0        0        0    15103 2021-11-23 15:54:27.975527 pyimporters-csv-0.4.98/tests/data/Digestion.zip
+-rw-r--r--   0        0        0    65555 2021-11-23 15:54:27.978527 pyimporters-csv-0.4.98/tests/data/Liste-des-codes-APE-NAF-excel-2017.xlsx
+-rw-r--r--   0        0        0     2605 2021-11-23 15:54:27.980527 pyimporters-csv-0.4.98/tests/data/currencies.txt
+-rw-r--r--   0        0        0     1536 2021-11-23 15:54:27.986528 pyimporters-csv-0.4.98/tests/data/currencies.zip
+-rw-r--r--   0        0        0     5386 2021-11-23 15:54:27.988528 pyimporters-csv-0.4.98/tests/data/lexicon.xlsx.zip
+-rw-r--r--   0        0        0     1450 2021-11-23 15:54:27.990527 pyimporters-csv-0.4.98/tests/test_csv.py
+-rw-r--r--   0        0        0     2520 2021-11-23 15:54:27.993528 pyimporters-csv-0.4.98/tests/test_excel.py
+-rw-r--r--   0        0        0      955 2021-11-23 15:54:27.998528 pyimporters-csv-0.4.98/tests/test_text.py
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 pyimporters-csv-0.4.98/setup.py
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 pyimporters-csv-0.4.98/PKG-INFO
```

### Comparing `pyimporters-csv-0.4.96/Jenkinsfile` & `pyimporters-csv-0.4.98/Jenkinsfile`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,20 @@
   // returnStatus = 1 when string not found -> Team commit
   // returnStatus = 0 when string is found  -> CI commit
   def last_commit_is_team = sh(
     script: 'git log -1 | grep "\\[Jenkins CI\\]"',
     returnStatus: true
   )
   if (params.forcePublishing) {
-    println "Try to publish, considering last commit has been done by Team"
+    println "Try to publish, proceeding"
+    last_commit_is_team = 1
+  }
+  def isStartedByUser = currentBuild.rawBuild.getCause(hudson.model.Cause$UserIdCause) != null
+  if (isStartedByUser) {
+    println "Job started by User, proceeding"
     last_commit_is_team = 1
   }
   if (last_commit_is_team == 0) {
     println 'Aborting build because last commit has been done by CI'
     currentBuild.result = 'ABORTED'
     currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
     sleep(1)   // Interrupt is not blocking and does not take effect immediately.
```

### Comparing `pyimporters-csv-0.4.96/pyimporters_csv/csv.py` & `pyimporters-csv-0.4.98/pyimporters_csv/csv.py`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/pyimporters_csv/excel.py` & `pyimporters-csv-0.4.98/pyimporters_csv/excel.py`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/pyimporters_csv/text.py` & `pyimporters-csv-0.4.98/pyimporters_csv/text.py`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/pyproject.toml` & `pyimporters-csv-0.4.98/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/Digestion.csv` & `pyimporters-csv-0.4.98/tests/data/Digestion.csv`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/Digestion.xls` & `pyimporters-csv-0.4.98/tests/data/Digestion.xls`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/Digestion.xlsx` & `pyimporters-csv-0.4.98/tests/data/Digestion.xlsx`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/Digestion.zip` & `pyimporters-csv-0.4.98/tests/data/Digestion.zip`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/Liste-des-codes-APE-NAF-excel-2017.xlsx` & `pyimporters-csv-0.4.98/tests/data/Liste-des-codes-APE-NAF-excel-2017.xlsx`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/currencies.txt` & `pyimporters-csv-0.4.98/tests/data/currencies.txt`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/currencies.zip` & `pyimporters-csv-0.4.98/tests/data/currencies.zip`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/data/lexicon.xlsx.zip` & `pyimporters-csv-0.4.98/tests/data/lexicon.xlsx.zip`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/test_csv.py` & `pyimporters-csv-0.4.98/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/test_excel.py` & `pyimporters-csv-0.4.98/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/tests/test_text.py` & `pyimporters-csv-0.4.98/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pyimporters-csv-0.4.96/setup.py` & `pyimporters-csv-0.4.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 entry_points = \
 {'pyimporters.plugins': ['csv = pyimporters_csv.csv:CSVKnowledgeParser',
                          'excel = pyimporters_csv.excel:ExcelKnowledgeParser',
                          'text = pyimporters_csv.text:TXTKnowledgeParser']}
 
 setup(name='pyimporters-csv',
-      version='0.4.96',
+      version='0.4.98',
       description='Sherpa knowledge import plugins',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyimporters-csv-0.4.96/PKG-INFO` & `pyimporters-csv-0.4.98/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimporters-csv
-Version: 0.4.96
+Version: 0.4.98
 Summary: Sherpa knowledge import plugins
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

