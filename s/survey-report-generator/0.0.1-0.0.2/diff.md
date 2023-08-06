# Comparing `tmp/survey_report_generator-0.0.1.tar.gz` & `tmp/survey_report_generator-0.0.2.tar.gz`

## Comparing `survey_report_generator-0.0.1.tar` & `survey_report_generator-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/__init__.py
--rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/databases.py
--rw-r--r--   0        0        0    12246 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/databases_summary.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/date_time.py
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/download_files.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/fesm.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/figures_utils.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/filter_utils.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/filter_utils_summary.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/g_drive_utils.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/generate_report.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/koala_habitat.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/pct.py
--rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/report-template.docx
--rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/report.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/storage.json
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/summary.py
--rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/src/report_generation/tables.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/LICENSE
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 survey_report_generator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/setup.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/__init__.py
+-rw-r--r--   0        0        0    10539 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/databases.py
+-rw-r--r--   0        0        0    12246 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/databases_summary.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/date_time.py
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/download_files.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/fesm.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/figures_utils.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/filter_utils.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/filter_utils_summary.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/g_drive_utils.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/generate_report.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/koala_habitat.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/pct.py
+-rw-r--r--   0        0        0  1246571 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/report-template.docx
+-rw-r--r--   0        0        0     6550 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/report.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/storage.json
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/summary.py
+-rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/src/report_generation/tables.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/README.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 survey_report_generator-0.0.2/PKG-INFO
```

### Comparing `survey_report_generator-0.0.1/src/.DS_Store` & `survey_report_generator-0.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/.DS_Store` & `survey_report_generator-0.0.2/src/report_generation/.DS_Store`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/databases.py` & `survey_report_generator-0.0.2/src/report_generation/databases.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/databases_summary.py` & `survey_report_generator-0.0.2/src/report_generation/databases_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/date_time.py` & `survey_report_generator-0.0.2/src/report_generation/date_time.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/download_files.py` & `survey_report_generator-0.0.2/src/report_generation/download_files.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/fesm.py` & `survey_report_generator-0.0.2/src/report_generation/fesm.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/figures_utils.py` & `survey_report_generator-0.0.2/src/report_generation/figures_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/filter_utils.py` & `survey_report_generator-0.0.2/src/report_generation/filter_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/filter_utils_summary.py` & `survey_report_generator-0.0.2/src/report_generation/filter_utils_summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/g_drive_utils.py` & `survey_report_generator-0.0.2/src/report_generation/g_drive_utils.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/generate_report.py` & `survey_report_generator-0.0.2/src/report_generation/generate_report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/koala_habitat.py` & `survey_report_generator-0.0.2/src/report_generation/koala_habitat.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/pct.py` & `survey_report_generator-0.0.2/src/report_generation/pct.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/report-template.docx` & `survey_report_generator-0.0.2/src/report_generation/report-template.docx`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/report.py` & `survey_report_generator-0.0.2/src/report_generation/report.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/storage.json` & `survey_report_generator-0.0.2/src/report_generation/storage.json`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/summary.py` & `survey_report_generator-0.0.2/src/report_generation/summary.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/src/report_generation/tables.py` & `survey_report_generator-0.0.2/src/report_generation/tables.py`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/.gitignore` & `survey_report_generator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/LICENSE` & `survey_report_generator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `survey_report_generator-0.0.1/README.md` & `survey_report_generator-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Report Generator
 
-[![PyPI version](https://badge.fury.io/py/my-python-package.svg)](https://badge.fury.io/py/my-python-package)
-[![Build Status](https://travis-ci.com/username/my-python-package.svg?branch=master)](https://travis-ci.com/username/my-python-package)
+[![PyPI version](https://badge.fury.io/py/survey-report-generator.svg)](https://badge.fury.io/py/survey-report-generator)
 
 Report Generator is a Python package used to generate reports for drone surveys. 
 You input the location name and a few other variables and the package will return a Word document pre-filled with tables and figures summarising the data collected for that survey.
 
 ## Installation
 
 Install Report Generator with pip:
 
 ```bash
-pip install report-generator
+pip install survey-report-generator
 ```
 
 ## Usage
 
 Initially, you need to create a Report object, outlined in the `report.py` file, which takes the following parameters:
 - **Required Parameters**
   - `location_name (str)`: The title of the report, this could be the official name of the location like
```

### Comparing `survey_report_generator-0.0.1/pyproject.toml` & `survey_report_generator-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "survey-report-generator"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Oliver Hahn", email="oliver.a.hahn@gmail.com" },
 ]
 description = "A tool to generate survey reports from collected data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `survey_report_generator-0.0.1/PKG-INFO` & `survey_report_generator-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: survey-report-generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to generate survey reports from collected data
 Project-URL: Homepage, https://github.com/nsw-wildlife-drone-hub/report-generator
 Author-email: Oliver Hahn <oliver.a.hahn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Report Generator
 
-[![PyPI version](https://badge.fury.io/py/my-python-package.svg)](https://badge.fury.io/py/my-python-package)
-[![Build Status](https://travis-ci.com/username/my-python-package.svg?branch=master)](https://travis-ci.com/username/my-python-package)
+[![PyPI version](https://badge.fury.io/py/survey-report-generator.svg)](https://badge.fury.io/py/survey-report-generator)
 
 Report Generator is a Python package used to generate reports for drone surveys. 
 You input the location name and a few other variables and the package will return a Word document pre-filled with tables and figures summarising the data collected for that survey.
 
 ## Installation
 
 Install Report Generator with pip:
 
 ```bash
-pip install report-generator
+pip install survey-report-generator
 ```
 
 ## Usage
 
 Initially, you need to create a Report object, outlined in the `report.py` file, which takes the following parameters:
 - **Required Parameters**
   - `location_name (str)`: The title of the report, this could be the official name of the location like
```

