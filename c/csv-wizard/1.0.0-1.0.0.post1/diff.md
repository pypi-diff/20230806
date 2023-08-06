# Comparing `tmp/csv-wizard-1.0.0.tar.gz` & `tmp/csv-wizard-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-wizard-1.0.0.tar", last modified: Mon Jun 19 13:02:30 2023, max compression
+gzip compressed data, was "csv-wizard-1.0.0.post1.tar", last modified: Mon Jun 19 13:37:52 2023, max compression
```

## Comparing `csv-wizard-1.0.0.tar` & `csv-wizard-1.0.0.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-1.0.0/LICENSE
--rw-r--r--   0        0        0      529 2023-06-19 12:54:35.526954 csv-wizard-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9516 2023-06-19 12:29:04.878243 csv-wizard-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-1.0.0/src/__init__.py
--rw-r--r--   0        0        0    11690 2023-06-19 12:53:52.145338 csv-wizard-1.0.0/src/csv_wizard.py
--rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-1.0.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-1.0.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-1.0.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-1.0.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-1.0.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-06-15 12:57:01.556547 csv-wizard-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      852 2023-06-19 12:23:08.073079 csv-wizard-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-16 12:26:56.159429 csv-wizard-1.0.0/tests/empty.csv
--rw-r--r--   0        0        0      698 2023-06-19 12:23:08.043157 csv-wizard-1.0.0/tests/test_divide.py
--rw-r--r--   0        0        0      256 2023-06-19 12:23:08.026358 csv-wizard-1.0.0/tests/test_encoding.py
--rw-r--r--   0        0        0      206 2023-06-16 16:32:30.995957 csv-wizard-1.0.0/tests/test_file_backup.csv
--rw-r--r--   0        0        0      257 2023-06-16 15:20:44.927006 csv-wizard-1.0.0/tests/test_file_diff.csv
--rw-r--r--   0        0        0      273 2023-06-16 15:16:32.197038 csv-wizard-1.0.0/tests/test_file_with_dups.csv
--rw-r--r--   0        0        0      610 2023-06-19 12:23:08.060112 csv-wizard-1.0.0/tests/test_find_common_rows.py
--rw-r--r--   0        0        0      750 2023-06-19 12:23:08.039169 csv-wizard-1.0.0/tests/test_find_different_rows.py
--rw-r--r--   0        0        0      634 2023-06-19 12:23:08.011398 csv-wizard-1.0.0/tests/test_get_all_rows.py
--rw-r--r--   0        0        0     1025 2023-06-19 12:23:08.022667 csv-wizard-1.0.0/tests/test_get_dialect.py
--rw-r--r--   0        0        0      938 2023-06-19 12:23:08.080060 csv-wizard-1.0.0/tests/test_get_duplicates.py
--rw-r--r--   0        0        0      437 2023-06-16 15:19:38.891982 csv-wizard-1.0.0/tests/test_get_headers.py
--rw-r--r--   0        0        0     1392 2023-06-19 12:23:08.100021 csv-wizard-1.0.0/tests/test_misc.py
--rw-r--r--   0        0        0      334 2023-06-19 12:23:08.068246 csv-wizard-1.0.0/tests/test_slice.py
--rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 csv-wizard-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-13 12:46:11.220776 csv-wizard-1.0.0.post1/LICENSE
+-rw-r--r--   0        0        0      535 2023-06-19 13:36:30.248960 csv-wizard-1.0.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     9591 2023-06-19 13:35:41.518927 csv-wizard-1.0.0.post1/README.md
+-rw-r--r--   0        0        0        0 2023-02-19 02:10:32.471751 csv-wizard-1.0.0.post1/src/__init__.py
+-rw-r--r--   0        0        0    11690 2023-06-19 13:17:53.241542 csv-wizard-1.0.0.post1/src/csv_wizard.py
+-rw-r--r--   0        0        0       39 2023-02-16 02:52:30.274333 csv-wizard-1.0.0.post1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-16 02:52:30.275330 csv-wizard-1.0.0.post1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-16 02:52:30.273335 csv-wizard-1.0.0.post1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      251 2023-02-16 02:52:30.275330 csv-wizard-1.0.0.post1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302624 csv-wizard-1.0.0.post1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-16 04:05:01.302950 csv-wizard-1.0.0.post1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-06-15 12:57:01.556547 csv-wizard-1.0.0.post1/tests/__init__.py
+-rw-r--r--   0        0        0      852 2023-06-19 12:23:08.073079 csv-wizard-1.0.0.post1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:26:56.159429 csv-wizard-1.0.0.post1/tests/empty.csv
+-rw-r--r--   0        0        0      698 2023-06-19 12:23:08.043157 csv-wizard-1.0.0.post1/tests/test_divide.py
+-rw-r--r--   0        0        0      256 2023-06-19 12:23:08.026358 csv-wizard-1.0.0.post1/tests/test_encoding.py
+-rw-r--r--   0        0        0      206 2023-06-16 16:32:30.995957 csv-wizard-1.0.0.post1/tests/test_file_backup.csv
+-rw-r--r--   0        0        0      257 2023-06-16 15:20:44.927006 csv-wizard-1.0.0.post1/tests/test_file_diff.csv
+-rw-r--r--   0        0        0      273 2023-06-16 15:16:32.197038 csv-wizard-1.0.0.post1/tests/test_file_with_dups.csv
+-rw-r--r--   0        0        0      610 2023-06-19 12:23:08.060112 csv-wizard-1.0.0.post1/tests/test_find_common_rows.py
+-rw-r--r--   0        0        0      750 2023-06-19 12:23:08.039169 csv-wizard-1.0.0.post1/tests/test_find_different_rows.py
+-rw-r--r--   0        0        0      634 2023-06-19 12:23:08.011398 csv-wizard-1.0.0.post1/tests/test_get_all_rows.py
+-rw-r--r--   0        0        0     1025 2023-06-19 12:23:08.022667 csv-wizard-1.0.0.post1/tests/test_get_dialect.py
+-rw-r--r--   0        0        0      938 2023-06-19 12:23:08.080060 csv-wizard-1.0.0.post1/tests/test_get_duplicates.py
+-rw-r--r--   0        0        0      437 2023-06-16 15:19:38.891982 csv-wizard-1.0.0.post1/tests/test_get_headers.py
+-rw-r--r--   0        0        0     1392 2023-06-19 12:23:08.100021 csv-wizard-1.0.0.post1/tests/test_misc.py
+-rw-r--r--   0        0        0      334 2023-06-19 12:23:08.068246 csv-wizard-1.0.0.post1/tests/test_slice.py
+-rw-r--r--   0        0        0     9690 1970-01-01 00:00:00.000000 csv-wizard-1.0.0.post1/PKG-INFO
```

### Comparing `csv-wizard-1.0.0/LICENSE` & `csv-wizard-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/pyproject.toml` & `csv-wizard-1.0.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "pytest>=7.2.1",
     "black>=23.3.0",
     "isort>=5.12.0",
 ]
 
 [project]
 name = "csv_wizard"
-version = "1.0.0"
+version = "1.0.0.post1"
 description = "Handy extension to Python csv standard library package"
 authors = [
     { name = "liquidsnake", email = "bentsoft365@gmail.com" },
 ]
 dependencies = [
     "chardet>=5.1.0",
 ]
```

### Comparing `csv-wizard-1.0.0/README.md` & `csv-wizard-1.0.0.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # csv wizard
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 ***
-## Import a CSV file by only giving the `CSVWizard` class a `string` containing the full name of the file without the *.csv* extension.
-> `new_file = CSVWizard("my_file")`
+## Import a CSV file by only giving the `CSVWizard` class a `string` containing the full name of the file without the *.csv* extension, and the path of the file (if it is in current folder just use `"."`).
+> `new_file = CSVWizard("my_file", ".")`
 ***
 ## Handling decoding/encoding on a file.
 All methods have an optional `encoding` argument.
 If left empty, csv_wizard will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
 The encoding parameter accepts strings.
 ```
 > file1.get_row_count(encoding='utf-8')
```

### Comparing `csv-wizard-1.0.0/src/csv_wizard.py` & `csv-wizard-1.0.0.post1/src/csv_wizard.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/conftest.py` & `csv-wizard-1.0.0.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_divide.py` & `csv-wizard-1.0.0.post1/tests/test_divide.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_find_common_rows.py` & `csv-wizard-1.0.0.post1/tests/test_find_common_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_find_different_rows.py` & `csv-wizard-1.0.0.post1/tests/test_find_different_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_get_all_rows.py` & `csv-wizard-1.0.0.post1/tests/test_get_all_rows.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_get_dialect.py` & `csv-wizard-1.0.0.post1/tests/test_get_dialect.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_get_duplicates.py` & `csv-wizard-1.0.0.post1/tests/test_get_duplicates.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/tests/test_misc.py` & `csv-wizard-1.0.0.post1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `csv-wizard-1.0.0/PKG-INFO` & `csv-wizard-1.0.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: csv_wizard
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Handy extension to Python csv standard library package
 License: MIT
 Author-email: liquidsnake <bentsoft365@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # csv wizard
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 ***
-## Import a CSV file by only giving the `CSVWizard` class a `string` containing the full name of the file without the *.csv* extension.
-> `new_file = CSVWizard("my_file")`
+## Import a CSV file by only giving the `CSVWizard` class a `string` containing the full name of the file without the *.csv* extension, and the path of the file (if it is in current folder just use `"."`).
+> `new_file = CSVWizard("my_file", ".")`
 ***
 ## Handling decoding/encoding on a file.
 All methods have an optional `encoding` argument.
 If left empty, csv_wizard will attempt to automatically figure out the encoding, however, if a `UnicodeDecodeError` or `UnicodeEncodeError` error are raised, the encoding should be specified manually. 
 The encoding parameter accepts strings.
 ```
 > file1.get_row_count(encoding='utf-8')
```

