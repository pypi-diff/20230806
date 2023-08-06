# Comparing `tmp/satdigitalinvoice-4.0.8.tar.gz` & `tmp/satdigitalinvoice-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.8.tar", last modified: Wed May 31 02:35:25 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.9.tar", last modified: Tue Jun 27 20:13:16 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.8.tar` & `satdigitalinvoice-4.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42176 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    31447 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 02:35:25.000000 satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:35:25.477380 satdigitalinvoice-4.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-31 02:35:14.000000 satdigitalinvoice-4.0.8/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.493614 satdigitalinvoice-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-27 20:13:16.493614 satdigitalinvoice-4.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.489614 satdigitalinvoice-4.0.9/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42858 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.489614 satdigitalinvoice-4.0.9/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.489614 satdigitalinvoice-4.0.9/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31454 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.489614 satdigitalinvoice-4.0.9/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.489614 satdigitalinvoice-4.0.9/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.489614 satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-27 20:13:16.000000 satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-27 20:13:16.000000 satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:13:16.000000 satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 20:13:16.000000 satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 20:13:16.000000 satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:13:16.493614 satdigitalinvoice-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:13:16.493614 satdigitalinvoice-4.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-27 20:13:06.000000 satdigitalinvoice-4.0.9/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.8/PKG-INFO` & `satdigitalinvoice-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.8
+Version: 4.0.9
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/client_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import re
 import warnings
 
-# noinspection PyUnresolvedReferences
 from bs4.builder import XMLParsedAsHTMLWarning
-from satcfdi import csf, RFC, RFCType
+from satcfdi.models import RFC, RFCType
+from satcfdi import csf
 from satcfdi.pacs.sat import SAT
 
 sat_service = SAT()
 logger = logging.getLogger(__name__)
 warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
 
 EMAIL_REGEX = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/facturacion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import logging
 import os
 from datetime import date, datetime
 from uuid import UUID
 from zipfile import ZipFile
 
 from PySimpleGUI import POPUP_BUTTONS_OK_CANCEL, PySimpleGUI as sg, POPUP_BUTTONS_NO_BUTTONS
-from satcfdi import DatePeriod, csf
+from satcfdi import csf
+from satcfdi.models import DatePeriod
 from satcfdi.accounting import EmailManager
 from satcfdi.accounting.models import EstadoComprobante
 from satcfdi.accounting.process import complement_invoices
 from satcfdi.create.cfd import cfdi40
 from satcfdi.create.cfd.catalogos import MetodoPago, TipoDeComprobante
 from satcfdi.exceptions import ResponseError
 from satcfdi.pacs import Accept
@@ -352,29 +353,44 @@
                                 file_attachments=attachments()
                             )
                             for r in facturas:
                                 self.local_db.notified_set(r.uuid, True)
 
                 case 'ajustes' | 'depositos':
                     with self.email_manager.sender as s:
-                        for data in self.progress_iterate(action_text, action_items):
-                            if file_name := data['create_fn']():
-                                receptor = data['receptor']
+                        grouped_action_items = []
+                        for _, g_data in itertools.groupby(
+                            sorted(
+                                action_items,
+                                key=lambda r: r["receptor"]["Rfc"]
+                            ),
+                            lambda r: r["receptor"]["Rfc"]
+                        ):
+                            grouped_action_items.append(list(g_data))
+
+                        for g_data in self.progress_iterate(action_text, grouped_action_items):
+                            file_names = []
+                            for data in g_data:
+                                if file := data['create_fn']():
+                                    file_names.append(file)
+
+                            if file_names:
+                                receptor = g_data[0]['receptor']
                                 if action_name == 'ajustes':
                                     subject = f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
                                 elif action_name == 'depositos':
                                     subject = f"Depósito Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
                                 else:
                                     raise NotImplementedError()
 
                                 s.send_email(
                                     subject=subject,
                                     to_addrs=receptor["Email"],
                                     html=facturacion_environment.get_template(f'mail_{action_name}_template.html').render(data),
-                                    file_attachments=[file_name]
+                                    file_attachments=file_names
                                 )
 
                 case 'clientes':
                     for client in self.progress_iterate(
                             action_text, action_items, lambda x: f"Validando: {x['Rfc']}"
                     ):
                         validar_client(client)
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/file_data_managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import re
 from decimal import Decimal
 
 import jsonschema as jsonschema
 import yaml
-from satcfdi import Code, DatePeriod
+from satcfdi.models import Code, DatePeriod
 from satcfdi.pacs import sat
 from satcfdi.transform.helpers import Xint
 from yaml import MappingNode, SafeLoader
 from yaml.constructor import ConstructorError
 
 from . import SOURCE_DIRECTORY
 from .utils import find_best_match, first_duplicate
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/gui_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import os
 from datetime import datetime, date
 from decimal import Decimal
 from decimal import InvalidOperation
 
 import xlsxwriter
 from markdown2 import markdown
-from satcfdi import DatePeriod
 from satcfdi.accounting import filter_invoices_iter, filter_payments_iter, invoices_export, payments_export
 from satcfdi.accounting.process import payments_groupby_receptor, payments_retentions_export
 from satcfdi.create.cfd import cfdi40
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
+from satcfdi.models import DatePeriod
 from satcfdi.pacs import sat
 from satcfdi.printer import Representable
 from weasyprint import HTML, CSS
 
 from . import SOURCE_DIRECTORY, ARCHIVOS_DIRECTORY, TEMP_DIRECTORY
 from .environments import facturacion_environment
 from .exceptions import ConsoleErrors
@@ -52,14 +52,20 @@
             nombre=receptor_cif['RazonSocial'],
             uso_cfdi=factura_details['UsoCFDI'],
             domicilio_fiscal_receptor=receptor_cif['CodigoPostal'],
             regimen_fiscal_receptor=receptor_cif['RegimenFiscal']
         ),
         metodo_pago=factura_details['MetodoPago'],
         forma_pago=factura_details['FormaPago'],
+        # cfdi_relacionados=[
+        #     cfdi40.CfdiRelacionados(
+        #         tipo_relacion=TipoRelacion.SUSTITUCION_DE_LOS_CFDI_PREVIOSaaaaaaa,
+        #         cfdi_relacionado=''xyc',
+        #     )
+        # ],
         # serie=serie,
         # folio=folio,
         conceptos=factura_details["Conceptos"]
     )
     invoice = invoice.process()
     return invoice
 
@@ -361,15 +367,15 @@
     payments_export(workbook, "EMITIDAS PAGOS", emitidas_pagos)
 
     # RECIBIDAS
     invoices_export(workbook, "RECIBIDAS", recibidas)
     payments_export(workbook, "RECIBIDAS PAGOS", recibidas_pagos)
 
     # SPECIALES
-    payments_export(workbook, f"RECIBIDAS PAGOS IVA {emisor_regimen.code}", pagos_hechos_iva)
+    payments_export(workbook, f"RECIBIDAS PAGOS IVA {emisor_regimen}", pagos_hechos_iva)
     if prediales:
         payments_export(workbook, "PREDIALES", prediales)
 
     # RETENCIONES
     if dp.month is None:
         archivo_retenciones = archivos_filename(dp, ext="retenciones.txt")
         pagos_agrupados = payments_groupby_receptor(emitidas_pagos)
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.9/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date, datetime, timedelta
 from enum import StrEnum
 
 import PySimpleGUI as sg
-from satcfdi import Code
+from satcfdi.models import Code
 from satcfdi.catalogs import select_all
 from satcfdi.pacs.sat import TipoDescargaMasivaTerceros
 
 from satdigitalinvoice.gui_functions import mf_pago_fmt, CALENDAR_FECHA_FMT
 
 FORMA_PAGO = select_all('C756_c_FormaPago')
 TEXT_PADDING = ((5, 0), 3)
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/localdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pickle
 from datetime import datetime
 from enum import Enum
 from uuid import UUID
 
 import diskcache
-from satcfdi import Code
+from satcfdi.models import Code
 from satcfdi.accounting import SatCFDI
 from satcfdi.accounting.models import EstadoComprobante
 from satcfdi.create.cfd.catalogos import MetodoPago, TipoDeComprobante
 from satcfdi.pacs import sat
 
 from .utils import estado_to_estatus
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.9/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.9/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.9/satdigitalinvoice/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import random
 import shutil
 import subprocess
 import sys
 from datetime import datetime
 from uuid import UUID
 
-from satcfdi import Signer, DatePeriod
+from satcfdi.models import Signer, DatePeriod
 from satcfdi.accounting.models import EstadoComprobante
 
 
 def to_date_period(periodo):
     if not periodo:
         return DatePeriod(year=None)
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.8
+Version: 4.0.9
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.8/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.9/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/setup.py` & `satdigitalinvoice-4.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.27',
+        'satcfdi==4.1.0',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-4.0.8/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.9/tests/test_crear_facturas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, datetime
 from decimal import Decimal
 from unittest import mock
 
 import pytest
-from satcfdi import Signer, DatePeriod
+from satcfdi.models import Signer, DatePeriod
 
 from satdigitalinvoice.__version__ import __package__
 from satdigitalinvoice.exceptions import ConsoleErrors
 from satdigitalinvoice.file_data_managers import ClientsManager, FacturasManager
 from satdigitalinvoice.gui_functions import generate_ingresos, periodicidad_desc
 from satdigitalinvoice.utils import find_best_match
 from tests.utils import verify_result, XElementPrettyPrinter
```

### Comparing `satdigitalinvoice-4.0.8/tests/test_localdb.py` & `satdigitalinvoice-4.0.9/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.8/tests/test_main.py` & `satdigitalinvoice-4.0.9/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 
 import pytest
-from satcfdi import DatePeriod
+from satcfdi.models import DatePeriod
 
 from satdigitalinvoice.facturacion import FacturacionGUI
 from yaml.constructor import ConstructorError
 
 from satdigitalinvoice.file_data_managers import LocalData, ConfigManager, FacturasManager
 
 from satdigitalinvoice.layout import make_layout
```

