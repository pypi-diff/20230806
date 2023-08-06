# Comparing `tmp/itkwasm_dicom_emscripten-3.0.0.tar.gz` & `tmp/itkwasm_dicom_emscripten-3.1.0.tar.gz`

## Comparing `itkwasm_dicom_emscripten-3.0.0.tar` & `itkwasm_dicom_emscripten-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/_version.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/js_package.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/read_image_dicom_file_series_async.py
--rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/fixtures.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/test_apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/test_itkwasm_dicom.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/test_read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/test_structured_report_to_html_async.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/test/test_structured_report_to_text_async.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/.gitignore
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/README.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/_version.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/js_package.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/read_image_dicom_file_series_async.py
+-rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/fixtures.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/test_apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/test_itkwasm_dicom.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/test_read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/test_structured_report_to_html_async.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/test/test_structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/.gitignore
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-3.1.0/PKG-INFO
```

### Comparing `itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/__init__.py` & `itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/read_image_dicom_file_series_async.py` & `itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/read_image_dicom_file_series_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-3.1.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/test/fixtures.py` & `itkwasm_dicom_emscripten-3.1.0/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/test/test_apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-3.1.0/test/test_apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/test/test_itkwasm_dicom.py` & `itkwasm_dicom_emscripten-3.1.0/test/test_itkwasm_dicom.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/test/test_read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-3.1.0/test/test_read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/test/test_structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-3.1.0/test/test_structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/test/test_structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-3.1.0/test/test_structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/README.md` & `itkwasm_dicom_emscripten-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/pyproject.toml` & `itkwasm_dicom_emscripten-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-3.0.0/PKG-INFO` & `itkwasm_dicom_emscripten-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-emscripten
-Version: 3.0.0
+Version: 3.1.0
 Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

