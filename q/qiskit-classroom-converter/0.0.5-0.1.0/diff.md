# Comparing `tmp/qiskit-classroom-converter-0.0.5.tar.gz` & `tmp/qiskit-classroom-converter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-classroom-converter-0.0.5.tar", last modified: Wed Aug  2 13:21:26 2023, max compression
+gzip compressed data, was "qiskit-classroom-converter-0.1.0.tar", last modified: Sun Aug  6 05:21:37 2023, max compression
```

## Comparing `qiskit-classroom-converter-0.0.5.tar` & `qiskit-classroom-converter-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.678543 qiskit-classroom-converter-0.0.5/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.5/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)       59 2023-08-02 12:35:39.000000 qiskit-classroom-converter-0.0.5/MANIFEST.in
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 13:21:26.678673 qiskit-classroom-converter-0.0.5/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.5/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1233 2023-08-02 13:10:51.000000 qiskit-classroom-converter-0.0.5/pyproject.toml
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.673936 qiskit-classroom-converter-0.0.5/qiskit_class_converter/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2166 2023-08-02 13:10:51.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/__init__.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.676072 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/base.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3679 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/braket_notation_to_matrix.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.676655 qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/converter_service.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.678270 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      206 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/top_level.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      126 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.5/requirements.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-08-02 13:21:26.679100 qiskit-classroom-converter-0.0.5/setup.cfg
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-06 05:21:37.672321 qiskit-classroom-converter-0.1.0/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.1.0/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       59 2023-08-02 13:33:45.000000 qiskit-classroom-converter-0.1.0/MANIFEST.in
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2547 2023-08-06 05:21:37.672454 qiskit-classroom-converter-0.1.0/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1940 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1232 2023-08-06 05:21:30.000000 qiskit-classroom-converter-0.1.0/pyproject.toml
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-06 05:21:37.666324 qiskit-classroom-converter-0.1.0/qiskit_class_converter/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2148 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/__init__.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-06 05:21:37.669813 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/base.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1620 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2664 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2260 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3911 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/string_to_braket_notation.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-06 05:21:37.670534 qiskit-classroom-converter-0.1.0/qiskit_class_converter/services/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/services/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     4527 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/qiskit_class_converter/services/converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-06 05:21:37.672086 qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2547 2023-08-06 05:21:37.000000 qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-08-06 05:21:37.000000 qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-08-06 05:21:37.000000 qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      195 2023-08-06 05:21:37.000000 qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-08-06 05:21:37.000000 qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/top_level.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      118 2023-08-06 05:03:24.000000 qiskit-classroom-converter-0.1.0/requirements.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-08-06 05:21:37.672828 qiskit-classroom-converter-0.1.0/setup.cfg
```

### Comparing `qiskit-classroom-converter-0.0.5/LICENSE` & `qiskit-classroom-converter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.5/PKG-INFO` & `qiskit-classroom-converter-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.5
+Version: 0.1.0
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
@@ -21,26 +21,26 @@
 https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
 
 ## Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
-* bra-ket notation to matrix
+* string to bra-ket notation
 
 ---
 
 ## Options
 
-| convert method    | option                                   |
-|-------------------|------------------------------------------|
-| QC_TO_BRA_KET     | expression{simplify, expand}, print{raw} |
-| QC_TO_MATRIX      | -                                        |
-| MATRIX_TO_QC      | label{str}                               |
-| BRA_KET_TO_MATRIX | -                                        |
+| convert method | option                                   |
+|----------------|------------------------------------------|
+| QC_TO_BRA_KET  | expression{simplify, expand}, print{raw} |
+| QC_TO_MATRIX   | print{raw}                               |
+| MATRIX_TO_QC   | label{str}                               |
+| STR_TO_BRA_KET | print{raw}                               |
 
 ```python
 from qiskit_class_converter import ConversionService
 
 ConversionService(conversion_type="QC_TO_BRA_KET", option={"expression": "simplify"})
 ```
```

### Comparing `qiskit-classroom-converter-0.0.5/README.md` & `qiskit-classroom-converter-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
 
 ## Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
-* bra-ket notation to matrix
+* string to bra-ket notation
 
 ---
 
 ## Options
 
-| convert method    | option                                   |
-|-------------------|------------------------------------------|
-| QC_TO_BRA_KET     | expression{simplify, expand}, print{raw} |
-| QC_TO_MATRIX      | -                                        |
-| MATRIX_TO_QC      | label{str}                               |
-| BRA_KET_TO_MATRIX | -                                        |
+| convert method | option                                   |
+|----------------|------------------------------------------|
+| QC_TO_BRA_KET  | expression{simplify, expand}, print{raw} |
+| QC_TO_MATRIX   | print{raw}                               |
+| MATRIX_TO_QC   | label{str}                               |
+| STR_TO_BRA_KET | print{raw}                               |
 
 ```python
 from qiskit_class_converter import ConversionService
 
 ConversionService(conversion_type="QC_TO_BRA_KET", option={"expression": "simplify"})
 ```
```

### Comparing `qiskit-classroom-converter-0.0.5/pyproject.toml` & `qiskit-classroom-converter-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 
 [tool.setuptools.packages.find]
 include = ['qiskit_class_converter*']
 exclude = ['qiskit_class_converter*tests']
 
 [project]
 name = "qiskit-classroom-converter"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
     { name = "KMU-quantum-classroom" },
 ]
 description = "extend the Qiskit classroom applications."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "qiskit==0.44.0",
     "qiskit-aer==0.12.2",
     "loguru==0.7.0",
     "sympy==1.12",
     "antlr4-python3-runtime==4.11",
-    "tomli==2.0.1; python_version < '3.11'"
+    "ipython==8.14.0",
+    "numpy==1.25.2"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage==7.2.7",
     "pylint==2.17.5",
     "tox==4.6.4",
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/__init__.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 ```
 
 # Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
-* bra-ket notation to matrix
+* string to bra-ket notation
 
 # Options
 
-| convert method    | option                                   |
-|-------------------|------------------------------------------|
-| QC_TO_BRA_KET     | expression{simplify, expand}, print{raw} |
-| QC_TO_MATRIX      | -                                        |
-| MATRIX_TO_QC      | label{str}                               |
-| BRA_KET_TO_MATRIX | -                                        |
+| convert method | option                                   |
+|----------------|------------------------------------------|
+| QC_TO_BRA_KET  | expression{simplify, expand}, print{raw} |
+| QC_TO_MATRIX   | print{raw}                               |
+| MATRIX_TO_QC   | label{str}                               |
+| STR_TO_BRA_KET | print{raw}                               |
 
 """
 #  Licensed to the Apache Software Foundation (ASF) under one
 #  or more contributor license agreements.  See the NOTICE file
 #  distributed with this work for additional information
 #  regarding copyright ownership.  The ASF licenses this file
 #  to you under the Apache License, Version 2.0 (the
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/base.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/braket_notation_to_matrix.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/string_to_braket_notation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Bra-ket Notation to Matrix Converter
+String to Bra-ket Notation
 """
 # from sympy.physics.quantum.represent import represent
 #  Licensed to the Apache Software Foundation (ASF) under one
 #  or more contributor license agreements.  See the NOTICE file
 #  distributed with this work for additional information
 #  regarding copyright ownership.  The ASF licenses this file
 #  to you under the Apache License, Version 2.0 (the
@@ -16,85 +16,87 @@
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 import re
+
+from sympy import latex
 from sympy.parsing.sympy_parser import parse_expr
 from sympy.physics.quantum.dagger import Dagger
-from sympy.physics.quantum.qubit import Qubit #, measure_all
+from sympy.physics.quantum.qubit import Qubit  # , measure_all
 
 from qiskit_class_converter.converters.base import BaseConverter
 
 
-class BraketNotationToMatrixConverter(BaseConverter):
+class StringToBraketNotationConverter(BaseConverter):
     """
     Converter class
     """
 
     # bra-ket regex
     regex_pattern = r"(?P<braket>[<][01]+[|][01]+[>])|(?P<ketbra>[|][01]+[>][<][01]+[|])|\
                     (?P<bra>[<][01]+[|])|(?P<ket>[|][01]+[>])"
     extr = re.compile("[01]+")
 
-    def make_pair(self, symbol, reverse = False):
+    def make_pair(self, symbol, reverse=False):
         """
         make multiple qubit expression
         :return:
         """
 
         temps = self.extr.findall(symbol)
 
         exp1 = Dagger(Qubit(temps[0]))
         exp2 = Qubit(temps[1])
 
-        if reverse :
+        if reverse:
             exp1 = Dagger(exp1)
             exp2 = Dagger(exp2)
 
         return exp1 * exp2
 
-    def make_qubit(self, symbol, is_dagger = False):
+    def make_qubit(self, symbol, is_dagger=False):
         """
         make qubit expression
         :return:
         """
 
         temp = self.extr.search(symbol).group()
         result = Qubit(temp)
-        if is_dagger :
+        if is_dagger:
             result = Dagger(result)
 
         return result
 
     def create_qubits(self, expr_symbols):
         """
         create qubits using symbols
         :return:
         """
 
         local_dict_str = {}
-        local_dict ={}
+        local_dict = {}
 
         dict_num = 97
-        for symbol in expr_symbols :
+        for symbol in expr_symbols:
             val = None
             qubit = None
 
-            if symbol[0] != "": #bra-ket
+            if symbol[0] != "":  # bra-ket
                 val = symbol[0]
                 qubit = self.make_pair(val)
-            elif symbol[1] != "": #ket-bra
+            elif symbol[1] != "":  # ket-bra
                 val = symbol[1]
-                qubit = self.make_pair(val, reverse = True)
-            elif symbol[2] != "": #bra
+                qubit = self.make_pair(val, reverse=True)
+            elif symbol[2] != "":  # bra
                 val = symbol[2]
-                qubit = self.make_qubit(val, is_dagger = True)
-            elif symbol[3] != "": #ket
+                qubit = self.make_qubit(val, is_dagger=True)
+            elif symbol[3] != "":  # ket
                 val = symbol[3]
                 qubit = self.make_qubit(val)
 
             local_dict_str[chr(dict_num)] = val
             local_dict[chr(dict_num)] = qubit
             dict_num += 1
 
@@ -106,16 +108,21 @@
         :return:
         """
         expr_symbols = re.findall(self.regex_pattern, expr_str)
 
         local_dict_str, local_dict = self.create_qubits(expr_symbols)
 
         for key in local_dict:
-            expr_str = expr_str.replace(local_dict_str[key], key,1)
+            expr_str = expr_str.replace(local_dict_str[key], key, 1)
         expr = parse_expr(expr_str, evaluate=False, transformations='all', local_dict=local_dict)
         return expr
 
     def actual_convert_action(self):
-        self.logger.debug("bra-ket notation to matrix")
-        expr = self.parse_braket(self.input_value)
+        self.logger.debug("String to bra-ket notation")
+        # type validate
+        if isinstance(self.input_value, str):
+            expr = self.parse_braket(self.input_value)
+        else:
+            raise TypeError("str is required.")
+        if self.option.get("print", False) == "raw":
+            return latex(expr)
         return expr
-
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/matrix_to_quantum_circuit.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/matrix_to_quantum_circuit.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,24 +14,32 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
+from typing import List
+
+import numpy as np
+
 from qiskit_class_converter.converters.base import BaseConverter
 
 
 class MatrixToQuantumCircuitConverter(BaseConverter):
     """
     Converter class
     """
 
     def actual_convert_action(self):
         self.logger.debug("matrix to quantum circuit")
-        gate = self.qiskit.extensions.UnitaryGate(self.input_value)
+        # type validate
+        if isinstance(self.input_value, (List, np.ndarray)):
+            gate = self.qiskit.extensions.UnitaryGate(self.input_value)
+        else:
+            raise TypeError("List or np.ndarray is required.")
         # parse by unitary circuit. can't describe what circuit is.
         if self.option.get("label", False):
             gate.label = self.option.get("label", "")
         else:
             gate.label = str(self.input_value)
         return gate
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+from typing import List
 
 from loguru import logger
+from qiskit import QuantumCircuit
 from sympy import SympifyError, simplify, expand, latex
 from sympy.parsing.latex import parse_latex
 
 from qiskit_class_converter.converters.base import BaseConverter
 
 
 class QuantumCircuitToBraketNotationConverter(BaseConverter):
@@ -30,15 +32,19 @@
     Converter class
     """
 
     # pylint: disable-next = too-many-return-statements
     def actual_convert_action(self):
         self.logger.debug("quantum circuit to bra-ket notation")
         self.input_value.save_statevector()
-        result = self.qiskit_aer.AerSimulator().run(self.input_value).result()
+        # type validate
+        if isinstance(self.input_value, (List, QuantumCircuit)):
+            result = self.qiskit_aer.AerSimulator().run(self.input_value).result()
+        else:
+            raise TypeError("QuantumCircuit is required.")
         source = result.get_statevector().draw("latex_source")
         try:
             if (self.option.get("expression", False) == "simplify") and \
                     (self.option.get("print", False) == "raw"):
                 return latex(simplify(parse_latex(source)))
             if self.option.get("expression", False) == "simplify":
                 return str(simplify(parse_latex(source)))
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_matrix.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/converters/quantum_circuit_to_matrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,24 +13,42 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+from typing import List
+
+import numpy as np
+from qiskit import QuantumCircuit
+from qiskit.visualization import array_to_latex
 
 from qiskit_class_converter.converters.base import BaseConverter
 
 
 class QuantumCircuitToMatrixConverter(BaseConverter):
     """
     Converter class
     """
+
     def actual_convert_action(self):
         self.logger.debug("quantum circuit to matrix")
         matrix_list = {"gate": []}
-        dag = self.qiskit.converters.circuit_to_dag(self.input_value)
+        # type validate
+        if isinstance(self.input_value, (List, QuantumCircuit)):
+            dag = self.qiskit.converters.circuit_to_dag(self.input_value)
+        else:
+            raise TypeError("QuantumCircuit is required.")
         for layer in dag.layers():
             circuit = self.qiskit.converters.dag_to_circuit(layer['graph'])
             matrix_list["gate"].append(self.qiskit.quantum_info.Operator(circuit).to_matrix())
         matrix_list["result"] = self.qiskit.quantum_info.Operator(self.input_value).to_matrix()
+        if self.option.get("print", False) == "raw":
+            latex_source_list = {"gate": []}
+            for each_matrix in matrix_list["gate"]:
+                latex_source_list["gate"].append(
+                    array_to_latex(array=np.array(each_matrix), source=True))
+            latex_source_list["result"] = array_to_latex(
+                array=np.array(matrix_list["result"]), source=True)
+            return latex_source_list
         return matrix_list
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/converter_service.py` & `qiskit-classroom-converter-0.1.0/qiskit_class_converter/services/converter_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 import typing
 from enum import Enum
 
+import numpy as np
 from qiskit import QuantumCircuit
 
-from qiskit_class_converter.converters.braket_notation_to_matrix \
-    import BraketNotationToMatrixConverter
 from qiskit_class_converter.converters.matrix_to_quantum_circuit \
     import MatrixToQuantumCircuitConverter
 from qiskit_class_converter.converters.quantum_circuit_to_braket_notation \
     import QuantumCircuitToBraketNotationConverter
 from qiskit_class_converter.converters.quantum_circuit_to_matrix \
     import QuantumCircuitToMatrixConverter
+from qiskit_class_converter.converters.string_to_braket_notation \
+    import StringToBraketNotationConverter
 
 
 class ConversionType(Enum):
     """
     Conversion Type
     """
     QC_TO_BRA_KET = QuantumCircuitToBraketNotationConverter
@@ -72,22 +73,25 @@
 ]
 sample_converter = ConversionService(conversion_type="MATRIX_TO_QC")
 result = sample_converter.convert(input_value=input_value)
 # using user's QuantumCircuit object
 quantum_circuit = QuantumCircuit(2, 2)
 quantum_circuit.append(result, [0, 1])
 ```"""
-    BRA_KET_TO_MATRIX = BraketNotationToMatrixConverter
+    STR_TO_BRA_KET = StringToBraketNotationConverter
     """```python
 from qiskit import QuantumCircuit
 from qiskit_class_converter import ConversionService
 
-sample_converter = ConversionService(conversion_type="BRA_KET_TO_MATRIX")
+sample_converter = ConversionService(conversion_type="STR_TO_BRA_KET")
 sample_converter.convert(input_value="|01>")
 ```"""
+    BRA_KET_TO_MATRIX = StringToBraketNotationConverter
+    """.. warning:: BRA_KET_TO_MATRIX was changed to STR_TO_BRA_KET and deprecated. \
+    This naming will be removed in 0.2 and later."""
 
 
 class ConversionService:  # pylint: disable=too-few-public-methods
     """
     Conversion Service class
 
 ```python
@@ -96,26 +100,26 @@
 ConversionService(conversion_type="QC_TO_BRA_KET", option={"expression": "simplify"})
 ```
     """
 
     def __init__(self, conversion_type: typing.Union[str, ConversionType], option=None):
         """
         init function
-        :param conversion_type:  QC_TO_BRA_KET, QC_TO_MATRIX, MATRIX_TO_QC, BRA_KET_TO_MATRIX
+        :param conversion_type:  QC_TO_BRA_KET, QC_TO_MATRIX, MATRIX_TO_QC, STR_TO_BRA_KET
         :param option: See the Options table in this article.
         """
         if option is None:
             self.option = {}
         self.option = option
         if isinstance(conversion_type, str):
             self.__conversion_object = ConversionType[conversion_type.upper()].value
         elif isinstance(conversion_type, ConversionType):
             self.__conversion_object = conversion_type.value
 
-    def convert(self, input_value: typing.Union[list, QuantumCircuit, str]):
+    def convert(self, input_value: typing.Union[list, np.ndarray, QuantumCircuit, str]):
         """
         convert functions
 
             result = sample_converter.convert(input_value=quantum_circuit)
             logger.info(result)
 
         :param input_value: QuantumCircuit or MATRIX or BRA_KET String
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/PKG-INFO` & `qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.5
+Version: 0.1.0
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # qiskit-classroom-converter
 Qiskit classroom Converter
 
@@ -21,26 +21,26 @@
 https://kmu-quantum-classroom.github.io/qiskit-classroom-converter/qiskit_class_converter.html
 
 ## Support convert method
 
 * quantum circuit to bra-ket notation
 * quantum circuit to matrix
 * matrix to quantum circuit
-* bra-ket notation to matrix
+* string to bra-ket notation
 
 ---
 
 ## Options
 
-| convert method    | option                                   |
-|-------------------|------------------------------------------|
-| QC_TO_BRA_KET     | expression{simplify, expand}, print{raw} |
-| QC_TO_MATRIX      | -                                        |
-| MATRIX_TO_QC      | label{str}                               |
-| BRA_KET_TO_MATRIX | -                                        |
+| convert method | option                                   |
+|----------------|------------------------------------------|
+| QC_TO_BRA_KET  | expression{simplify, expand}, print{raw} |
+| QC_TO_MATRIX   | print{raw}                               |
+| MATRIX_TO_QC   | label{str}                               |
+| STR_TO_BRA_KET | print{raw}                               |
 
 ```python
 from qiskit_class_converter import ConversionService
 
 ConversionService(conversion_type="QC_TO_BRA_KET", option={"expression": "simplify"})
 ```
```

### Comparing `qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/SOURCES.txt` & `qiskit-classroom-converter-0.1.0/qiskit_classroom_converter.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 qiskit_class_converter/__init__.py
 qiskit_class_converter/converters/__init__.py
 qiskit_class_converter/converters/base.py
-qiskit_class_converter/converters/braket_notation_to_matrix.py
 qiskit_class_converter/converters/matrix_to_quantum_circuit.py
 qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
 qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+qiskit_class_converter/converters/string_to_braket_notation.py
 qiskit_class_converter/services/__init__.py
 qiskit_class_converter/services/converter_service.py
 qiskit_classroom_converter.egg-info/PKG-INFO
 qiskit_classroom_converter.egg-info/SOURCES.txt
 qiskit_classroom_converter.egg-info/dependency_links.txt
 qiskit_classroom_converter.egg-info/requires.txt
 qiskit_classroom_converter.egg-info/top_level.txt
```

