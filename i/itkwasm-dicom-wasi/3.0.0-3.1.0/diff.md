# Comparing `tmp/itkwasm_dicom_wasi-3.0.0.tar.gz` & `tmp/itkwasm_dicom_wasi-3.1.0.tar.gz`

## Comparing `itkwasm_dicom_wasi-3.0.0.tar` & `itkwasm_dicom_wasi-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/_version.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/read_image_dicom_file_series.py
--rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/structured_report_to_html.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/structured_report_to_text.py
--rwxr-xr-x   0        0        0  5231236 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
--rwxr-xr-x   0        0        0  1897852 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
--rwxr-xr-x   0        0        0  6070364 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm
--rwxr-xr-x   0        0        0  4588663 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
--rwxr-xr-x   0        0        0  4569283 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/test/test_apply_presentation_state_to_image.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/test/test_read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/test/test_structured_report_to_html.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/test/test_structured_report_to_text.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/.gitignore
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/README.md
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/_version.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/read_image_dicom_file_series.py
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/structured_report_to_html.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/structured_report_to_text.py
+-rwxr-xr-x   0        0        0  5231236 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
+-rwxr-xr-x   0        0        0  1897852 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
+-rwxr-xr-x   0        0        0  6070364 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm
+-rwxr-xr-x   0        0        0  4588663 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
+-rwxr-xr-x   0        0        0  4569283 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/test/test_apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/test/test_read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/test/test_structured_report_to_html.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/test/test_structured_report_to_text.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/.gitignore
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-3.1.0/PKG-INFO
```

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/read_image_dicom_file_series.py` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/read_image_dicom_file_series.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/structured_report_to_html.py` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/structured_report_to_html.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/structured_report_to_text.py` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm` & `itkwasm_dicom_wasi-3.1.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/test/test_apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-3.1.0/test/test_apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/test/test_structured_report_to_html.py` & `itkwasm_dicom_wasi-3.1.0/test/test_structured_report_to_html.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/test/test_structured_report_to_text.py` & `itkwasm_dicom_wasi-3.1.0/test/test_structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/README.md` & `itkwasm_dicom_wasi-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/pyproject.toml` & `itkwasm_dicom_wasi-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-3.0.0/PKG-INFO` & `itkwasm_dicom_wasi-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-wasi
-Version: 3.0.0
+Version: 3.1.0
 Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

