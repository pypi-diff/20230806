# Comparing `tmp/itkwasm_dicom-3.0.0.tar.gz` & `tmp/itkwasm_dicom-3.1.0.tar.gz`

## Comparing `itkwasm_dicom-3.0.0.tar` & `itkwasm_dicom-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/Makefile
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/conf.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/make.bat
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/_version.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/apply_presentation_state_to_image.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/read_image_dicom_file_series.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/read_image_dicom_file_series_async.py
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_html.py
--rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_html_async.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_text.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_text_async.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/.gitignore
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/README.md
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 itkwasm_dicom-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/conf.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/_version.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/read_image_dicom_file_series.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/read_image_dicom_file_series_async.py
+-rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_html.py
+-rw-r--r--   0        0        0     7893 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_text.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/.gitignore
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/README.md
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 itkwasm_dicom-3.1.0/PKG-INFO
```

### Comparing `itkwasm_dicom-3.0.0/docs/Makefile` & `itkwasm_dicom-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/docs/conf.py` & `itkwasm_dicom-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/docs/index.md` & `itkwasm_dicom-3.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/docs/make.bat` & `itkwasm_dicom-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/docs/_static/favicon.png` & `itkwasm_dicom-3.1.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/docs/_static/logo.svg` & `itkwasm_dicom-3.1.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/__init__.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/apply_presentation_state_to_image.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/apply_presentation_state_to_image_async.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/read_dicom_encapsulated_pdf.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/read_dicom_encapsulated_pdf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/read_image_dicom_file_series.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/read_image_dicom_file_series.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/read_image_dicom_file_series_async.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/read_image_dicom_file_series_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_html.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_html.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_html_async.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_text.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/itkwasm_dicom/structured_report_to_text_async.py` & `itkwasm_dicom-3.1.0/itkwasm_dicom/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/pyproject.toml` & `itkwasm_dicom-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom-3.0.0/PKG-INFO` & `itkwasm_dicom-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom
-Version: 3.0.0
+Version: 3.1.0
 Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

