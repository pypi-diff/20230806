# Comparing `tmp/dukeai_lib-0.2.2.tar.gz` & `tmp/dukeai_lib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.2.2.tar", last modified: Sun Aug  6 03:59:55 2023, max compression
+gzip compressed data, was "dukeai_lib-0.2.3.tar", last modified: Sun Aug  6 04:06:39 2023, max compression
```

## Comparing `dukeai_lib-0.2.2.tar` & `dukeai_lib-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.835908 dukeai_lib-0.2.2/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.2.2/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 03:59:55.834908 dukeai_lib-0.2.2/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.2.2/README.md
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.814923 dukeai_lib-0.2.2/dukeai_lib/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      244 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/dukeai_lib/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.2.2/dukeai_lib/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      116 2023-08-05 19:11:34.000000 dukeai_lib-0.2.2/dukeai_lib/globals.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.820908 dukeai_lib-0.2.2/dukeai_lib/load_transmission/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       59 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/dukeai_lib/load_transmission/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     6619 2023-08-06 03:45:42.000000 dukeai_lib-0.2.2/dukeai_lib/load_transmission/functions.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.830907 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/accessorial.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/bill_of_lading.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification_exceptions.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/invoice.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/noa_lor.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rate_confirmation.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rsi_translator.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/schema_utilities.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      601 2023-08-06 03:45:42.000000 dukeai_lib-0.2.2/dukeai_lib/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    18350 2023-08-06 03:54:32.000000 dukeai_lib-0.2.2/dukeai_lib/utilities.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.818907 dukeai_lib-0.2.2/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      967 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      711 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-08-06 03:59:55.835908 dukeai_lib-0.2.2/setup.cfg
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      924 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/setup.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.834908 dukeai_lib-0.2.2/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.2.2/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.2.2/src/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.2.2/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.2.2/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 04:06:39.624457 dukeai_lib-0.2.3/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.2.3/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 04:06:39.623456 dukeai_lib-0.2.3/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.2.3/README.md
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 04:06:39.593456 dukeai_lib-0.2.3/dukeai_lib/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      244 2023-08-06 04:06:30.000000 dukeai_lib-0.2.3/dukeai_lib/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.2.3/dukeai_lib/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      116 2023-08-05 19:11:34.000000 dukeai_lib-0.2.3/dukeai_lib/globals.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 04:06:39.599456 dukeai_lib-0.2.3/dukeai_lib/load_transmission/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       59 2023-08-06 03:59:47.000000 dukeai_lib-0.2.3/dukeai_lib/load_transmission/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     6619 2023-08-06 03:45:42.000000 dukeai_lib-0.2.3/dukeai_lib/load_transmission/functions.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 04:06:39.619456 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/accessorial.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/bill_of_lading.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/classification.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/classification_exceptions.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/invoice.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/noa_lor.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/rate_confirmation.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/rsi_translator.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/schema_utilities.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      601 2023-08-06 03:45:42.000000 dukeai_lib-0.2.3/dukeai_lib/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    22737 2023-08-06 04:06:13.000000 dukeai_lib-0.2.3/dukeai_lib/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 04:06:39.597456 dukeai_lib-0.2.3/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 04:06:39.000000 dukeai_lib-0.2.3/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      967 2023-08-06 04:06:39.000000 dukeai_lib-0.2.3/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-08-06 04:06:39.000000 dukeai_lib-0.2.3/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-08-06 04:06:39.000000 dukeai_lib-0.2.3/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-08-06 04:06:39.000000 dukeai_lib-0.2.3/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      711 2023-08-06 04:06:29.000000 dukeai_lib-0.2.3/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-08-06 04:06:39.624457 dukeai_lib-0.2.3/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      924 2023-08-06 04:06:30.000000 dukeai_lib-0.2.3/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 04:06:39.622458 dukeai_lib-0.2.3/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.2.3/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.2.3/src/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.2.3/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.2.3/src/utilities.py
```

### Comparing `dukeai_lib-0.2.2/LICENSE` & `dukeai_lib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/PKG-INFO` & `dukeai_lib-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.2.2/README.md` & `dukeai_lib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/application.py` & `dukeai_lib-0.2.3/dukeai_lib/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/load_transmission/functions.py` & `dukeai_lib-0.2.3/dukeai_lib/load_transmission/functions.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/accessorial.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/accessorial.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/bill_of_lading.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/bill_of_lading.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/classification.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification_exceptions.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/classification_exceptions.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/invoice.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/invoice.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/noa_lor.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/noa_lor.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/parse_classification_page_range.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/parse_classification_page_range.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rate_confirmation.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/rate_confirmation.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rsi_translator.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/rsi_translator.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/schema_utilities.py` & `dukeai_lib-0.2.3/dukeai_lib/schema_kung_fu/schema_utilities.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/tools.py` & `dukeai_lib-0.2.3/dukeai_lib/tools.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/dukeai_lib/utilities.py` & `dukeai_lib-0.2.3/dukeai_lib/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -234,26 +234,146 @@
         return response
     except Exception as e:
         print(f"[ERROR] {func} Error ==> {e}")
         traceback.print_exc()
         return None
 
 
-def multi_load_confirmation_email(
+def multi_load_confirmation_email(subject, body, recipient, all_response_data, email_sender, email_client, body2="", body3=""):
+    func = multi_load_confirmation_email.__name__
+    try:
+        if isinstance(recipient, str):
+            recipient = [recipient]
+
+        load_responses = list()
+        for load_resp in all_response_data:
+            idx = all_response_data.index(load_resp)
+
+            button_data = [
+                {
+                    'button_header': 'Invoice',
+                    'button_text': 'Download PDF',
+                    'link': load_resp['duke_invoice_url']
+                },
+                {
+                    'button_header': 'DUKE Verified Score',
+                    'button_text': 'Download PDF',
+                    'link': load_resp['score_report_url']
+                },
+                {
+                    'button_header': 'Load Documents',
+                    'button_text': 'Download PDF',
+                    'link': load_resp['load_document_link']
+                }
+            ]
+            success, table = gen_three_button_html(button_data)
+            if not success:
+                raise Exception(f"gen_three_button_html encountered an error")
+
+            if load_resp['vendor_bill_no'] not in ["0000", "00", "0"]:
+                load_responses.append(
+                    f"""
+                    <p>Rate Confirmation Reference #: {load_resp['load_reference']}</p>
+                    <p>DUKE.ai Invoice #: {load_resp['duke_invoice_no']}</p>
+                    <p>Vendor Bill #: {load_resp['vendor_bill_no']}</p>
+                    <p>DUKE.ai Load reference #: {load_resp['load_id']}</p>
+                    <p>Total: ${load_resp['amount']}</p>
+                    {table}
+                    """
+                )
+
+            else:
+                # """
+                # <p>Downloadable Invoice PDF: {load_resp['duke_invoice_url']}</p>
+                # <p>Downloadable Load Acceptance Score PDF: {load_resp['score_report_url']}</p>
+                # <p>Downloadable Load Document PDF: {load_resp['load_document_link']}</p>
+                # """
+                load_responses.append(
+                    f"""
+                    <p>Rate Confirmation Reference #: {load_resp['load_reference']}</p>
+                    <p>DUKE.ai Invoice #: {load_resp['duke_invoice_no']}</p>
+                    <p>DUKE.ai Load reference #: {load_resp['load_id']}</p>
+                    <p>Total: ${load_resp['amount']}</p>
+                    {table}
+                    """
+                )
+
+            if idx != (len(all_response_data) - 1):
+                load_responses.append(
+                    "<p>-----------------------------------</p>"
+                )
+            else:
+                load_responses.append("<p></p>")
+
+        load_responses.append(
+            f"""
+            <p></p>
+            <p>-----------------------------------</p>
+            <p></p>
+            <p>Please contact Support@Duke.ai if you have any questions, and thank you for trucking with DUKE.ai!</p>
+            """
+        )
+
+        body_string = "".join(load_responses)
+
+        body_html = f"""
+        <html>
+        <head></head>
+        <body>
+        <p>{body}</p>
+        <p>{body2}</p>
+        <p>{body3}</p>
+        <p></p>
+        {body_string}
+        </body>
+        </html>
+          """
+
+        response = email_client.send_email(
+            Destination={
+                'ToAddresses': recipient
+            },
+            Message={
+                'Body': {
+                    'Html': {
+                        'Charset': "UTF-8",
+                        'Data': body_html,
+                    },
+                    'Text': {
+                        'Charset': "UTF-8",
+                        'Data': (str(body_html)),
+                    }
+                },
+                'Subject': {
+                    'Charset': "UTF-8",
+                    'Data': subject,
+                },
+            },
+            Source=email_sender
+        )
+        print(f"[INFO] {func} Email sent! Message ID: {response}")
+        return True, response, ""
+    except Exception as e:
+        print(f"[ERROR] {func} Error ==> {e}")
+        traceback.print_exc()
+        return False, None, f"{e}"
+
+
+def multi_load_confirmation_email_v2(
         subject: str,
         body: str,
         recipient: str,
         invoice_response_data: list,
         bol_response_data: list,
         email_client,
         email_sender,
         body2="",
         body3=""
 ):
-    function_name = multi_load_confirmation_email.__name__
+    function_name = multi_load_confirmation_email_v2.__name__
     if isinstance(recipient, str):
         recipient = [recipient]
 
     bol_responses = list()
     for bol_res in bol_response_data:
         idx = bol_response_data.index(bol_res)
         button = gen_single_button_html(
```

### Comparing `dukeai_lib-0.2.2/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.2.3/dukeai_lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.2.2/dukeai_lib.egg-info/SOURCES.txt` & `dukeai_lib-0.2.3/dukeai_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/pyproject.toml` & `dukeai_lib-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dukeai_lib-0.2.2/setup.py` & `dukeai_lib-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dukeai_lib',
-    version="0.2.2",
+    version="0.2.3",
     description="Common functions used across the DUKE.ai project environments.",
     url='https://duke.ai',
     author='Blake Donahoo',
     author_email='blake@duke.ai',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
     keywords=['dukeai', 'duke.ai'],
```

### Comparing `dukeai_lib-0.2.2/src/application.py` & `dukeai_lib-0.2.3/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.2/src/tools.py` & `dukeai_lib-0.2.3/src/tools.py`

 * *Files identical despite different names*

