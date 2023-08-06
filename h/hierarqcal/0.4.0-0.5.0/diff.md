# Comparing `tmp/hierarqcal-0.4.0.tar.gz` & `tmp/hierarqcal-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierarqcal-0.4.0.tar", last modified: Mon May 22 12:02:25 2023, max compression
+gzip compressed data, was "hierarqcal-0.5.0.tar", last modified: Sun Aug  6 18:43:21 2023, max compression
```

## Comparing `hierarqcal-0.4.0.tar` & `hierarqcal-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.756121 hierarqcal-0.4.0/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1528 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     4806 2023-05-22 12:02:25.756121 hierarqcal-0.4.0/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     4614 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/
--rw-rw-r--   0 matt      (1000) matt      (1000)      335 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/cirq/
--rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/cirq/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2007 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/cirq/cirq_circuits.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2467 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/cirq/cirq_helper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6869 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/hierarqcal/cirq/tf_helper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    53811 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/core.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/pennylane/
--rw-rw-r--   0 matt      (1000) matt      (1000)       56 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/pennylane/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1464 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/pennylane/pennylane_circuits.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5028 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/pennylane/pennylane_helper.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal/qiskit/
--rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/qiskit/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2391 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/qiskit/qiskit_circuits.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2993 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/qiskit/qiskit_helper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7702 2023-05-22 11:46:28.000000 hierarqcal-0.4.0/hierarqcal/utils.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/hierarqcal.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)     4806 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      636 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)      167 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       11 2023-05-22 12:02:25.000000 hierarqcal-0.4.0/hierarqcal.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       84 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      472 2023-05-22 12:02:25.756121 hierarqcal-0.4.0/setup.cfg
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-22 12:02:25.752121 hierarqcal-0.4.0/tests/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-01-23 08:42:03.000000 hierarqcal-0.4.0/tests/test_core.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1528 2023-01-23 08:42:03.000000 hierarqcal-0.5.0/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5026 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4834 2023-08-06 18:22:14.000000 hierarqcal-0.5.0/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/hierarqcal/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      460 2023-08-06 18:22:14.000000 hierarqcal-0.5.0/hierarqcal/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/hierarqcal/cirq/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       42 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/cirq/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2007 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/cirq/cirq_circuits.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2467 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/cirq/cirq_helper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6869 2023-01-23 08:42:03.000000 hierarqcal-0.5.0/hierarqcal/cirq/tf_helper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    64665 2023-08-06 18:22:14.000000 hierarqcal-0.5.0/hierarqcal/core.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/hierarqcal/pennylane/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       56 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/pennylane/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1464 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/pennylane/pennylane_circuits.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5028 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/pennylane/pennylane_helper.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/hierarqcal/qiskit/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-05-24 15:41:01.000000 hierarqcal-0.5.0/hierarqcal/qiskit/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2431 2023-06-09 06:52:48.000000 hierarqcal-0.5.0/hierarqcal/qiskit/qiskit_circuits.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5083 2023-08-06 18:22:14.000000 hierarqcal-0.5.0/hierarqcal/qiskit/qiskit_helper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    15224 2023-08-06 18:22:14.000000 hierarqcal-0.5.0/hierarqcal/utils.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/hierarqcal.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5026 2023-08-06 18:43:21.000000 hierarqcal-0.5.0/hierarqcal.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      668 2023-08-06 18:43:21.000000 hierarqcal-0.5.0/hierarqcal.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-08-06 18:43:21.000000 hierarqcal-0.5.0/hierarqcal.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)      167 2023-08-06 18:43:21.000000 hierarqcal-0.5.0/hierarqcal.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       11 2023-08-06 18:43:21.000000 hierarqcal-0.5.0/hierarqcal.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       84 2023-01-23 08:42:03.000000 hierarqcal-0.5.0/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      472 2023-08-06 18:43:21.180601 hierarqcal-0.5.0/setup.cfg
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-08-06 18:43:21.176602 hierarqcal-0.5.0/tests/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-06-12 18:04:53.000000 hierarqcal-0.5.0/tests/test_core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     9058 2023-08-06 18:22:14.000000 hierarqcal-0.5.0/tests/test_symbol_management.py
```

### Comparing `hierarqcal-0.4.0/LICENSE.txt` & `hierarqcal-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.4.0/PKG-INFO` & `hierarqcal-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierarqcal
-Version: 0.4.0
+Version: 0.5.0
 Description-Content-Type: text/markdown
 Provides-Extra: cirq
 Provides-Extra: pennylane
 Provides-Extra: qiskit
 License-File: LICENSE.txt
 
 # HierarQcal 
@@ -25,26 +25,26 @@
 
 ## Quick example
 
 #### Building a [Quantum Convolutional Neural Network (QCNN)](https://qiskit.org/ecosystem/machine-learning/tutorials/11_quantum_convolutional_neural_networks.html) with one line of code:
 
 ```python
 from hierarqcal import Qinit, Qcycle, Qmask
-hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("right", mapping=v))*3
+hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("!*", mapping=v))*3
 ```
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_right.png?raw=true" style="border:solid 2px black;">
 
 #### Modular and hierarchical circuit building:
 ```python
 ### Reverse binary tree
 from hierarqcal import Qinit, Qcycle, Qmask
 # motif: level 1
 m1_1 = Qcycle(stride=2)
-m1_2 = Qmask(pattern="left")
+m1_2 = Qmask(global_pattern="*!")
 # motif: level 2
 m2_1 = m1_1 + m1_2
 # motif: level 3
 m3_1 = Qinit(8) + m2_1 * 3
 ```
 $m^3_1\rightarrow \text{QCNN}:$
 
@@ -83,17 +83,24 @@
 We welcome contributions to the project. Please see the [contribution guidelines](https://github.com/matt-lourens/hierarqcal/blob/master/CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) for more information.
 
 ## License
 BSD 3-Clause "New" or "Revised" License, see [LICENSE](https://github.com/matt-lourens/hierarqcal/blob/master/LICENSE.txt) for more information.
 
 ## Citation
 ```latex
-@article{lourens2023hierarchical,
-      title={Hierarchical quantum circuit representations for neural architecture search},
-      url = {https://arxiv.org/abs/2210.15073},
-      author={Matt Lourens and Ilya Sinayskiy and Daniel K. Park and Carsten Blank and Francesco Petruccione},
-      year={2023},
-      eprint={2210.15073},
-      archivePrefix={arXiv},
-      primaryClass={quant-ph}
+@article{lourensHierarchicalQuantumCircuit2023,
+  title = {Hierarchical Quantum Circuit Representations for Neural Architecture Search},
+  author = {Lourens, Matt and Sinayskiy, Ilya and Park, Daniel K. and Blank, Carsten and Petruccione, Francesco},
+  date = {2023-08-05},
+  journaltitle = {npj Quantum Information},
+  shortjournal = {npj Quantum Inf},
+  volume = {9},
+  number = {1},
+  pages = {1--15},
+  publisher = {{Nature Publishing Group}},
+  issn = {2056-6387},
+  doi = {10.1038/s41534-023-00747-z},
+  url = {https://www.nature.com/articles/s41534-023-00747-z},
+  issue = {1},
+  langid = {english},
 }
 ```
```

### Comparing `hierarqcal-0.4.0/README.md` & `hierarqcal-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 ## Quick example
 
 #### Building a [Quantum Convolutional Neural Network (QCNN)](https://qiskit.org/ecosystem/machine-learning/tutorials/11_quantum_convolutional_neural_networks.html) with one line of code:
 
 ```python
 from hierarqcal import Qinit, Qcycle, Qmask
-hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("right", mapping=v))*3
+hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("!*", mapping=v))*3
 ```
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_right.png?raw=true" style="border:solid 2px black;">
 
 #### Modular and hierarchical circuit building:
 ```python
 ### Reverse binary tree
 from hierarqcal import Qinit, Qcycle, Qmask
 # motif: level 1
 m1_1 = Qcycle(stride=2)
-m1_2 = Qmask(pattern="left")
+m1_2 = Qmask(global_pattern="*!")
 # motif: level 2
 m2_1 = m1_1 + m1_2
 # motif: level 3
 m3_1 = Qinit(8) + m2_1 * 3
 ```
 $m^3_1\rightarrow \text{QCNN}:$
 
@@ -74,17 +74,24 @@
 We welcome contributions to the project. Please see the [contribution guidelines](https://github.com/matt-lourens/hierarqcal/blob/master/CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) for more information.
 
 ## License
 BSD 3-Clause "New" or "Revised" License, see [LICENSE](https://github.com/matt-lourens/hierarqcal/blob/master/LICENSE.txt) for more information.
 
 ## Citation
 ```latex
-@article{lourens2023hierarchical,
-      title={Hierarchical quantum circuit representations for neural architecture search},
-      url = {https://arxiv.org/abs/2210.15073},
-      author={Matt Lourens and Ilya Sinayskiy and Daniel K. Park and Carsten Blank and Francesco Petruccione},
-      year={2023},
-      eprint={2210.15073},
-      archivePrefix={arXiv},
-      primaryClass={quant-ph}
+@article{lourensHierarchicalQuantumCircuit2023,
+  title = {Hierarchical Quantum Circuit Representations for Neural Architecture Search},
+  author = {Lourens, Matt and Sinayskiy, Ilya and Park, Daniel K. and Blank, Carsten and Petruccione, Francesco},
+  date = {2023-08-05},
+  journaltitle = {npj Quantum Information},
+  shortjournal = {npj Quantum Inf},
+  volume = {9},
+  number = {1},
+  pages = {1--15},
+  publisher = {{Nature Publishing Group}},
+  issn = {2056-6387},
+  doi = {10.1038/s41534-023-00747-z},
+  url = {https://www.nature.com/articles/s41534-023-00747-z},
+  issue = {1},
+  langid = {english},
 }
 ```
```

### Comparing `hierarqcal-0.4.0/hierarqcal/cirq/cirq_circuits.py` & `hierarqcal-0.5.0/hierarqcal/cirq/cirq_circuits.py`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.4.0/hierarqcal/cirq/cirq_helper.py` & `hierarqcal-0.5.0/hierarqcal/cirq/cirq_helper.py`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.4.0/hierarqcal/cirq/tf_helper.py` & `hierarqcal-0.5.0/hierarqcal/cirq/tf_helper.py`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.4.0/hierarqcal/core.py` & `hierarqcal-0.5.0/hierarqcal/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,44 +16,63 @@
 import warnings
 from copy import copy, deepcopy
 from collections import deque, namedtuple
 import numpy as np
 import itertools as it
 import sympy as sp
 
+CircuitInstruction = namedtuple(
+    "CircuitInstruction", ["gate_name", "symbol_info", "sub_bits"]
+)
+
 
 class Primitive_Types(Enum):
     """
     Enum for primitive types.
     """
 
     CYCLE = "cycle"
     MASK = "mask"
+    SPLIT = "split"
     PERMUTE = "permute"
     INIT = "init"
+    PIVOT = "pivot"
+    BASE_MOTIF = "base_motif"
 
 
 class Qunitary:
     """
     Base class for all unitary operations, the main purpose is to store the operation, its arity and parameters (symbols) for later use.
     # TODO add support for function as matrix
+    # TODO add share_weights parameter
     """
 
     def __init__(self, function=None, n_symbols=0, arity=2, symbols=None):
         """
         Args:
             function (function, optional): Function to apply. If None, then the default from :py:class:`Default_Mappings` is used.
             n_symbols (int, optional): Number of symbols that function uses. Defaults to 0.
             arity (int, optional): Number of qubits that function acts upon. Two means 2-qubit unitaries, three means 3-qubits unitaries and so on. Defaults to 2.
             symbols (list, optional): List of symbol values (rotation angles). Elements can be either sympy symbols, complex numbers, or qiskit parameters. Defaults to None.
         """
         self.function = function
-        self.n_symbols = n_symbols
-        self.arity = arity
-        self.symbols = None
+        if isinstance(self.function, str):
+            (
+                circuit_instructions,
+                unique_bits,
+                unique_params,
+            ) = self.get_circ_info_from_string(function)
+            self.circuit_instructions = circuit_instructions
+            self.n_symbols = len(unique_params)
+            self.arity = len(unique_bits)
+        else:
+            self.circuit_instructions = None
+            self.n_symbols = len(symbols) if not (symbols is None) else n_symbols
+            self.arity = arity
+        self.symbols = symbols
         self.edge = None
 
     def __call__(self, *args, **kwargs):
         return self.function(*args, **kwargs)
 
     def get_symbols(self):
         """
@@ -76,86 +95,205 @@
                 f"Number of symbols must be {self.n_symbols} for this function"
             )
         self.symbols = symbols
 
     def set_edge(self, edge):
         self.edge = edge
 
+    def get_circ_info_from_string(self, input_str):
+        """
+        Takes a string that represents a circuit function, and
+        breaks down the string into a set of circuit instructions.
+
+        Args:
+            `input_str` (str)
+        Returns:
+            `substr_list` (list): a list of circuit instructions, where each entry
+            represents a distinct gate operation.
+            Each entry is a list of three components: [gate_name,symbol_info, sub_bits]
+                1. `gate_name` (str) is the name of the Qiskit gate being implemented.
+                2. `symbol_info` (list) keeps track of whether the gate is parametrized, and
+                        if so, whether it is the same parameter as another gate.
+                3. `sub_bits` (list of ints) keeps track of the bits the gates are applied on.
+            `unique_bits` (list of ints): set of qubits
+            `unique_params` (list of strs): set of gate parameters
+
+        Workflow:
+            Step 1: partition the string into lists of individual gate instructions
+                    in the form `{gate_string}(parameters)^{bits}`
+            Step 2: split each substring into the gate string, the relevant
+                    parameters, and the bits it acts on
+            Step 3: convert the bits, the gate string, and the relevant parameters
+                    into integers/functions
+        """
+
+        # Step 1 #
+
+        # Split the input string based on ';' into a list where each entry is a gate instruction
+        substrings = input_str.split(";")
+        # Remove any leading or trailing whitespaces from each substring
+        substrings = [substring.strip() for substring in substrings]
+
+        # Steps 2,3 #
+
+        circuit_instructions = []
+        unique_bits = []
+        unique_params = []
+        for substring in substrings:
+            instruction = []
+
+            # Separating the parameters, gates, and bits in the substring
+            start_index = substring.find("{")
+            end_index = substring.find("}")
+
+            param_start_index = substring.find("(")
+            param_end_index = substring.find(")")
+
+            bits_start_index = substring.find("^")
+            bits_end_index = len(substring)
+
+            # getting gate string
+            if start_index == -1:
+                gate_string = substring[start_index + 1 : param_start_index]
+            else:
+                gate_string = substring[start_index + 1 : end_index]
+            instruction.append(gate_string.lower())
+
+            # getting param string and index
+            params_string = substring[param_start_index + 1 : param_end_index]
+            if params_string == "":
+                instruction.append([0, 0, 0])
+            else:
+                param_list = params_string.split(",")
+                p_list = []
+                p_inds = []
+                for param_entry in param_list:
+                    # Remove any leading or trailing whitespaces from each substring
+                    p_entry = param_entry.strip()
+                    p_list.append(p_entry)
+                    # Check if the param is a duplicate and if not, add to unique_params
+                    if p_entry not in unique_params:
+                        unique_params.append(p_entry)
+                        isinlist = False
+                    else:
+                        isinlist = True
+                    # Find location of param in unique_params
+                    param_indx = np.where(np.array(unique_params) == p_entry)[0][0]
+                    p_inds.append(param_indx)
+
+                instruction.append([len(p_list), p_inds, isinlist])
+
+            # getting list of bits
+            bits_string = substring[bits_start_index + 1 : bits_end_index]
+            bits = []
+            for bit in bits_string:
+                bit = int(bit)
+                bits.append(bit)
+                if bit not in unique_bits:
+                    unique_bits.append(bit)
+            instruction.append(bits)
+
+            # add to list of circuit instructions
+            circuit_instruction = CircuitInstruction(
+                instruction[0], instruction[1], instruction[2]
+            )
+            circuit_instructions.append(circuit_instruction)
+
+        return circuit_instructions, unique_bits, unique_params
+
 
 class Default_Mappings(Enum):
     """
     Enum for default mappings
     """
 
     CYCLE = Qunitary(n_symbols=1, arity=2)
+    PIVOT = Qunitary(n_symbols=1, arity=2)
     MASK = None
+    SPLIT = None
+    BASE_MOTIF = None
     PERMUTE = Qunitary(n_symbols=1, arity=2)
 
 
 class Qmotif:
     """
     Hierarchical circuit architectures are created by stacking motifs, the lowest level motifs (primitives) are building blocks for higher level ones. Examples of primitives are cycles (:py:class:`Qcycle`), masks (:py:class:`Qmask_Base`), and permutations (:py:class:`Qpermute`). Each motif is a directed graph with nodes Q representing qubits and edges E unitary operations applied between them. The direction of an edge is the order of interaction for the unitary. Each instance has pointers to its predecessor and successor.
 
     Attributes:
         Q (list, optional): Qubit labels of the motif. Defaults to [].
         E (list, optional): Edges of the motif. Defaults to [].
         Q_avail (list, optional): Available qubits of the motif. This is calculated by the previous motif in the stack. Defaults to [].
-        edge_order (list, optional): Order of unitaries applied. Defaults to [1].
+        edge_order (list, optional): Order of unitaries applied. Defaults to [1], [-1] will reverse the order, [5,6] does the 5th and 6th edge first and then the rest in the normal order.
         next (:py:class:`Qmotif`, optional): Next motif in the stack. Defaults to None.
         prev (Qmotif, optional): Previous motif in the stack. Defaults to None.
         mapping (:py:class:`Qunitary` or :py:class:`Qhierarchy`, optional): Either a :py:class:`Qunitary` instance or a :py:class:`Qhierarchy` that will be converted to an :py:class:`Qunitary` object. Defaults to None.
-        symbols (list, optional): List of symbol values (rotation angles). Each element in the list can be a sympy symbol, complex number, or qiskit parameter. Defaults to None.
+        symbol_fn (lambda): TODO
         is_default_mapping (bool, optional): Flag to determine if default mapping is used. Defaults to True.
         is_operation (bool, optional): Flag to determine if the motif is an operation. Defaults to True.
         share_weights (bool, optional): Flag to determine if weights are shared within a motif. Defaults to True.
     """
 
     def __init__(
         self,
         Q=[],
         E=[],
         Q_avail=[],
         edge_order=[1],
         next=None,
         prev=None,
         mapping=None,
-        symbols=None,
+        symbol_fn=lambda x, ns, ne: x,
         is_default_mapping=True,
         is_operation=True,
         share_weights=True,
+        type=Primitive_Types.BASE_MOTIF,
     ) -> None:
         # Meta information
         self.is_operation = is_operation
         self.is_default_mapping = is_default_mapping
+        self.type = type
         # graph
         self.Q = Q
         self.Q_avail = Q_avail
         self.E = E
         self.edge_order = edge_order
         # higher level graph
         self.mapping = mapping
-        self.symbols = symbols
+        self.symbol_fn = symbol_fn
         self.share_weights = share_weights
         self.edge_mapping = (
             []
         )  # TODO docstring, edgemapping only gets set when the motif gets edges generated
         self.n_symbols = 0
         # pointers
         self.prev = prev
         self.next = next
         # Handle mappings
         if self.is_default_mapping:
             self.arity = 2
         else:
             if isinstance(self.mapping, Qhierarchy):
                 # If mapping was specified as sub-hierarchy, convert it to a qunitary
+                if any(
+                    [
+                        isinstance(symbol, sp.Symbol)
+                        for symbol in self.mapping.get_symbols()
+                    ]
+                ):
+                    # if any symbols are symbolic, then we scrap them TODO ensure if we want to do this
+                    new_symbols = None
+                else:
+                    # If they are numeric
+                    new_symbols = list(self.mapping.get_symbols())
+
                 new_mapping = Qunitary(
                     function=None,
                     n_symbols=self.mapping.n_symbols,
                     arity=len(self.mapping.tail.Q),
+                    symbols=new_symbols,
                 )
                 new_mapping.function = self.mapping.get_unitary_function()
                 self.mapping = new_mapping
             self.arity = self.mapping.arity
 
     def __add__(self, other):
         """
@@ -177,25 +315,43 @@
             other (int): Number of times to repeat motif.
 
         Returns:
             Qmotifs: A tuple of motifs: (self, self, ..., self), where each is a new object copied from the original.
         """
         return Qmotifs((deepcopy(self) for i in range(other)))
 
+    def __call__(self, Q, E=[], remaining_q=None, is_operation=True, **kwargs):
+        self.set_Q(Q)
+        mapping = kwargs.get("mapping", None)
+        if mapping:
+            self.set_mapping(mapping)
+        if len(E) > 0:
+            self.set_E(E)
+        if remaining_q:
+            self.set_Qavail(remaining_q)
+        else:
+            self.set_Qavail(Q)
+        self.set_is_operation(is_operation)
+        start_idx = kwargs.get("start_idx", 0)
+        self.set_symbols(start_idx=start_idx)
+
     def append(self, other):
         """
         Append an other motif to the current one: self + other = (self, other).
 
         Args:
             other (Qmotif): Motif to append to current motif (self).
 
         Returns:
             Qmotifs: A 2-tuple of motifs: (self, other) in the order they were added. The tuples contain copies of the original motifs.
         """
-        return Qmotifs((deepcopy(self), deepcopy(other)))
+        if isinstance(other, Sequence):
+            return Qmotifs((deepcopy(self),) + deepcopy(other))
+        else:
+            return Qmotifs((deepcopy(self), deepcopy(other)))
 
     def set_Q(self, Q):
         """
         Set the qubit labels Q of the motif.
 
         Args:
             Q (list(int or string)): List of qubit labels.
@@ -210,17 +366,21 @@
             E (list(tuples)): List of edges, where each edge is a tuple of qubit labels (self.Q).
         """
         if 0 in self.edge_order:
             # Raise error if 0 is in edge order
             raise ValueError(
                 "Edge order can't contain 0, as there is no 0th edge. Use 1 instead, edge order is based on ordering, that is [1] means first edge comes first [2,8] means second edge comes first, then 8th edge comes second. There is no 0th edge"
             )
-        E_ordered = [E[i - 1] for i in self.edge_order if i - 1 < len(E)]
-        E_rest = [edge for edge in E if edge not in E_ordered]
-        Ep_l = E_ordered + E_rest
+        if -1 in self.edge_order:
+            # Reverse edge order if -1 is in edge order
+            Ep_l = [E[i] for i in range(len(E) - 1, -1, -1)]
+        else:
+            E_ordered = [E[i - 1] for i in self.edge_order if i - 1 < len(E)]
+            E_rest = [edge for edge in E if edge not in E_ordered]
+            Ep_l = E_ordered + E_rest
         self.E = Ep_l
 
     def set_arity(self, arity):
         """
         Set the arity of the motif (qubits per unitary/ nodes per edge).
 
         Args:
@@ -320,52 +480,116 @@
         Set the symbol's.
 
         Args:
             symbols (list): List of symbols to set.
             start_idx (int): Starting index of symbols, this is used when :py:class:Qhierarchy updates the stack, it loops through each motif counting symbols, at each motif it updates the symbols (inderectly calls this function) and send the current count as starting inde so that correct sympy symbol indices are used.
         """
         if not (self.mapping is None) and len(self.E) > 0:
+            symbol_fn = self.symbol_fn
             if symbols is None:
-                if isinstance(next(self.get_symbols(), False), sp.Symbol) or len(list(self.get_symbols()))==0:
+                if (
+                    isinstance(next(self.get_symbols(), False), sp.Symbol)
+                    or len(list(self.get_symbols())) == 0
+                ):
                     # If no new symbols are provided and current symbols are still symbolic or no symbols exist
                     # Generate symbols, this is used when Qhierarchy updates the stack.
-                    symbols = sp.symbols(
-                        f"x_{start_idx}:{start_idx + self.mapping.n_symbols*(len(self.E) if not(self.share_weights) else 1)}"
-                    )
+                    if self.mapping.symbols is None:
+                        # If no symbols exist in the mapping
+                        symbols = sp.symbols(
+                            f"x_{start_idx}:{start_idx + self.mapping.n_symbols*(len(self.E) if not(self.share_weights) else 1)}"
+                        )
+                    else:
+                        symbols = self.mapping.symbols
+                        if len(symbols) != self.mapping.n_symbols * (
+                            len(self.E) if not (self.share_weights) else 1
+                        ):
+                            # If old symbols don't match current setup
+                            symbols = [
+                                symbol
+                                for _ in range(
+                                    (len(self.E) if not (self.share_weights) else 1)
+                                )
+                                for symbol in symbols
+                            ]
                 else:
                     # If no new symbols are provided but old symbols exist
                     symbols = list(self.get_symbols())
                     if len(symbols) != self.mapping.n_symbols * (
                         len(self.E) if not (self.share_weights) else 1
                     ):
-                        # If old sybmbols don't match current setup
+                        # If old symbols don't match current setup
                         symbols = sp.symbols(
                             f"x_{start_idx}:{start_idx + self.mapping.n_symbols*(len(self.E) if not(self.share_weights) else 1)}"
                         )
                         raise Warning(
                             f"Number of symbols {len(symbols)} does not match number of symbols in motif {self.mapping.n_symbols*(len(self.E) if not(self.share_weights) else 1)}, symbolic ones will be generated"
-                        )                        
+                        )
             else:
+                # Don't apply symbol fn (just identity) if symbols are set explicitly
+                symbol_fn = lambda x, ns, ne: x
                 if len(symbols) != self.mapping.n_symbols * (
                     len(self.E) if not (self.share_weights) else 1
                 ):
                     raise ValueError(
                         f"Number of symbols {len(symbols)} does not match number of symbols in motif {self.mapping.n_symbols*(len(self.E) if not(self.share_weights) else 1)}"
                     )
             self.edge_mapping = []
             idx = 0
+            n_edge = 1
             for edge in self.E:
                 tmp_mapping = deepcopy(self.mapping)
                 tmp_mapping.set_edge(edge)
-                tmp_mapping.set_symbols(symbols[idx : idx + self.mapping.n_symbols])
+                tmp_mapping.set_symbols(
+                    [
+                        symbol_fn(symbols[idx], idx + 1, n_edge)
+                        for idx in range(idx, idx + self.mapping.n_symbols, 1)
+                    ]
+                )
                 if not (self.share_weights):
                     idx += self.mapping.n_symbols
                 self.edge_mapping.append(tmp_mapping)
+                n_edge += 1
             self.n_symbols = len(symbols)
 
+    def cycle(self, Q, stride=1, step=1, offset=0, boundary="periodic", arity=2):
+        """
+        The cycle pattern
+        """
+        nq_available = len(Q)
+        if boundary == "open":
+            mod_nq = lambda x: x % nq_available
+            E = [
+                tuple(
+                    (
+                        Q[i + j * stride]
+                        for j in range(arity)
+                        if i + j * stride < nq_available
+                    )
+                )
+                for i in range(offset, nq_available, step)
+            ]
+            # Remove all that is not "complete"
+            E = [edge for edge in E if len(edge) == arity]
+
+        else:
+            mod_nq = lambda x: x % nq_available
+            E = [
+                tuple((Q[mod_nq(i + j * stride)] for j in range(arity)))
+                for i in range(offset, nq_available, step)
+            ]
+            # Remove all that is not "complete", i.e. contain duplicates
+            E = [edge for edge in E if len(set(edge)) == arity]
+        if (
+            len(E) == arity
+            and sum([len(set(E[0]) - set(E[k])) == 0 for k in range(arity)]) == arity
+        ):
+            # If there are only as many edges as qubits, and they are the same, then we can keep only one of them
+            E = [E[0]]
+        return E
+
 
 class Qmotifs(tuple):
     """
     A tuple of motifs, this is the data structure for storing sequences motifs. It subclasses tuple, so all tuple methods are available.
     """
 
     # TODO mention assumption that only operators should be used i.e. +, *
@@ -403,15 +627,15 @@
             return Qmotifs((deepcopy(item) for i in range(other) for item in self))
         else:
             raise ValueError("Only integers are allowed for multiplication")
 
 
 class Qcycle(Qmotif):
     """
-    A cycle motif, spreads unitaries in a ladder structure accross the circuit
+    A cycle motif, spreads unitaries in a ladder structure across the circuit
     TODO implement open boundary for dense and pooling also + tests
     """
 
     def __init__(
         self,
         stride=1,
         step=1,
@@ -426,25 +650,26 @@
 
         Args:
             stride (int, optional): Stride of the cycle. Defaults to 1.
             step (int, optional): Step of the cycle. Defaults to 1.
             offset (int, optional): Offset of the cycle. Defaults to 0.
 
         """
-        self.type = Primitive_Types.CYCLE
         self.stride = stride
         self.step = step
         self.offset = offset
         self.boundary = boundary
         # Specify sequence of gates:
         mapping = kwargs.get("mapping", None)
         is_default_mapping = True if mapping is None else False
         # motif_symbols = None # TODO maybe allow symbols to be intialised
         # Initialize graph
-        super().__init__(is_default_mapping=is_default_mapping, **kwargs)
+        super().__init__(
+            is_default_mapping=is_default_mapping, type=Primitive_Types.CYCLE, **kwargs
+        )
 
     def __call__(self, Qc_l, *args, **kwargs):
         """
         Call the motif, this generates the edges and qubits of the motif (directed graph) based on it's available qubits.
         Each time a motif in the stack changes, a loop runs through the stack from the beginning and calls each motif to update the graph (the available qubits, the edges etc).
 
         Args:
@@ -455,70 +680,29 @@
                 * mapping (tuple(function, int)): TODO update this docstring, it's not a tuple anymore.
                     Function mapping is specified as a tuple, where the first argument is a function and the second is the number of symbols it uses. A symbol here refers to an variational paramater for a quantum circuit, i.e. crz(theta, q0, q1) <- theta is a symbol for the gate.
 
         Returns:
             Qconv: Returns the updated version of itself, with correct nodes and edges.
         """
         # Determine cycle operation
-        nq_available = len(Qc_l)
-        if self.stride % nq_available == 0:
+        if self.stride % len(Qc_l) == 0:
             # TODO make this clear in documentation
             # warnings.warn(
             #     f"Stride and number of available qubits can't be the same, received:\nstride: {self.stride}\n available qubits:{nq_available}. Defaulting to stride of 1"
             # )
             self.stride = 1
-        if self.boundary == "open":
-            mod_nq = lambda x: x % nq_available
-            Ec_l = [
-                tuple(
-                    (
-                        Qc_l[i + j * self.stride]
-                        for j in range(self.arity)
-                        if i + j * self.stride < nq_available
-                    )
-                )
-                for i in range(self.offset, nq_available, self.step)
-            ]
-            # Remove all that is not "complete"
-            Ec_l = [edge for edge in Ec_l if len(edge) == self.arity]
-
-        else:
-            mod_nq = lambda x: x % nq_available
-            Ec_l = [
-                tuple((Qc_l[mod_nq(i + j * self.stride)] for j in range(self.arity)))
-                for i in range(self.offset, nq_available, self.step)
-            ]
-            # Remove all that is not "complete", i.e. contain duplicates
-            Ec_l = [edge for edge in Ec_l if len(set(edge)) == self.arity]
-        if (
-            len(Ec_l) == self.arity
-            and sum([len(set(Ec_l[0]) - set(Ec_l[k])) == 0 for k in range(self.arity)])
-            == self.arity
-        ):
-            # If there are only as many edges as qubits, and they are the same, then we can keep only one of them
-            Ec_l = [Ec_l[0]]
-        self.set_Q(Qc_l)
-        # Set order of edges
-        # if 0 in self.edge_order: TODO check if this is removable
-        #     # Raise error if 0 is in edge order
-        #     raise ValueError(
-        #         "Edge order can't contain 0, as there is no 0th edge. Use 1 instead, edge order is based on ordering, that is [1] means first edge comes first [2,8] means second edge comes first, then 8th edge comes second. There is no 0th edge"
-        #     )
-        # Ec_l_ordered = [Ec_l[i - 1] for i in self.edge_order if i - 1 < len(Ec_l)]
-        # Ec_l_rest = [edge for edge in Ec_l if edge not in Ec_l_ordered]
-        # Ec_l = Ec_l_ordered + Ec_l_rest
-        # All qubits are still available for the next operation
-        self.set_Qavail(Qc_l)
-        mapping = kwargs.get("mapping", None)
-        if mapping:
-            self.set_mapping(mapping)
-        # It is important that set_E gets called last, as sets of symbol creation for the motif
-        self.set_E(Ec_l)
-        start_idx = kwargs.get("start_idx", 0)
-        self.set_symbols(start_idx=start_idx)
+        E = self.cycle(
+            Qc_l,
+            stride=self.stride,
+            step=self.step,
+            offset=self.offset,
+            boundary=self.boundary,
+            arity=self.arity,
+        )
+        super().__call__(Qc_l, E=E, **kwargs)
 
         return self
 
     def __eq__(self, other):
         if isinstance(other, Qcycle):
             self_attrs = vars(self)
             other_attrs = vars(other)
@@ -532,21 +716,24 @@
 
 class Qpermute(Qmotif):
     """
     A dense motif, it connects unitaries to all possible combinations of qubits (all possible edges given Q) in the quantum circuit.
     """
 
     def __init__(self, combinations=True, **kwargs):
-        self.type = Primitive_Types.PERMUTE
         self.combinations = combinations
         # Specify sequence of gates:
         mapping = kwargs.get("mapping", None)
         is_default_mapping = True if mapping is None else False
         # Initialize graph
-        super().__init__(is_default_mapping=is_default_mapping, **kwargs)
+        super().__init__(
+            is_default_mapping=is_default_mapping,
+            type=Primitive_Types.PERMUTE,
+            **kwargs,
+        )
 
     def __call__(self, Qc_l, *args, **kwargs):
         """
         Call the motif, this is used to generate the edges and qubits of the motif (directed graph) based on it's available qubits.
         Each time a motif in the stack changes, a loop runs through the stack from the beginning and calls each motif to update the graph (the available qubits, the edges etc).
 
         Args:
@@ -563,205 +750,277 @@
         # All possible wire combinations
         if self.combinations:
             Ec_l = list(it.combinations(Qc_l, r=self.arity))
         else:
             Ec_l = list(it.permutations(Qc_l, r=self.arity))
         if len(Ec_l) == 2 and Ec_l[0][0:] == Ec_l[1][1::-1]:
             Ec_l = [Ec_l[0]]
-        self.set_Q(Qc_l)
-        self.set_Qavail(Qc_l)
-        mapping = kwargs.get("mapping", None)
-        if mapping:
-            self.set_mapping(mapping)
-        # It is important that set_E gets called last, as sets of symbol creation for the motif
-        self.set_E(Ec_l)
-        start_idx = kwargs.get("start_idx", 0)
-        self.set_symbols(start_idx=start_idx)
+
+        super().__call__(Qc_l, E=Ec_l, **kwargs)
         return self
 
     def __eq__(self, other):
         if isinstance(other, Qpermute):
             self_attrs = vars(self)
             other_attrs = vars(other)
             for attr, value in self_attrs.items():
                 if attr not in other_attrs or other_attrs[attr] != value:
                     return False
             return True
         return False
 
-
-class Qmask_Base(Qmotif):
+class Qsplit(Qmotif):
     def __init__(
         self,
-        pattern="right",  # nearest_circle, nearest_tower, nearest_square, right, left, up, down, lambda function
+        global_pattern="1*",
+        merge_within="1*",
+        merge_between=None,  # either this or third item in strides
+        mask=False,
+        strides=[1, 1, 0],
+        steps=[1, 1, 1],
+        offsets=[0, 0, 0],
+        boundaries=["open", "open", "periodic"],
+        type=Primitive_Types.SPLIT,
         **kwargs,
-    ):
-        """
-        TODO Provide topology for nearest neighbor pooling., options, circle, tower, square
-        TODO Open, Periodic boundary
-        """
-        self.type = Primitive_Types.MASK
-        self.pattern = pattern
-        super().__init__(**kwargs)
-
-    def __call__(self, Q, E, remaining_q, is_operation, **kwargs):
+    ) -> None:
+        # If strides, steps or offsets are provided as integers, convert to list that repeats that integer
+        if isinstance(strides, int):
+            strides = [strides] * 3
+        if isinstance(strides, int):
+            steps = [steps] * 3
+        if isinstance(offsets, int):
+            offsets = [offsets] * 3
+        # Set attributes
+
+        self.global_pattern = global_pattern
+        self.merge_within = merge_within
+        self.merge_between = merge_between
+        self.mask = mask
+        self.strides = strides
+        self.steps = steps
+        self.offsets = offsets
+        self.boundaries = boundaries
         mapping = kwargs.get("mapping", None)
-        start_idx = kwargs.get("start_idx", 0)
-        self.set_Q(Q)
-        self.set_Qavail(remaining_q)
-        if mapping:
-            self.set_mapping(mapping)
-        self.set_is_operation(is_operation)
-        self.set_E(E)
-        self.set_symbols(start_idx=start_idx)
+        is_default_mapping = True if mapping is None else False
+        # Initialize Qmotif
+        super().__init__(is_default_mapping=is_default_mapping, type=type, **kwargs)
 
-    def get_mask_pattern_fn(self, mask_pattern, Qp_l=[]):
-        """
-        Get the pattern function for the pooling operation.
+    def __call__(self, Q, E=[], remaining_q=None, is_operation=True, **kwargs):
+        super().__call__(
+            Q, E=E, remaining_q=remaining_q, is_operation=is_operation, **kwargs
+        )
+        return self
 
-        Args:
-            mask_pattern (str or lambda): The pattern type, can be "left", "right", "even", "odd", "inside" or "outside" which corresponds to a specific pattern (see comments in code below).
-                                            The string can also be a bit string, i.e. "01000" which pools the 2nd qubit.
-                                            If a lambda function is passed, it is used as the pattern function, it should work as follow: mask_pattern_fn([0,1,2,3,4,5,6,7]) -> [0,1,2,3], i.e.
-                                            the function returns a sublist of the input list based on some pattern. What's nice about passing a function is that it can be list length independent,
-                                            meaning the same kind of pattern will be applied as the list grows or shrinks.
-            Qp_l (list): List of available qubits.
-        """
-        if isinstance(mask_pattern, str):
-            # Mapping words to the pattern type
-            if mask_pattern == "left":
-                # 0 1 2 3 4 5 6 7
-                # x x x x
-                mask_pattern_fn = lambda arr: arr[0 : len(arr) // 2 : 1]
-            elif mask_pattern == "right":
-                # 0 1 2 3 4 5 6 7
-                #         x x x x
-                mask_pattern_fn = lambda arr: arr[len(arr) // 2 : len(arr) : 1]
-            elif mask_pattern == "even":
-                # 0 1 2 3 4 5 6 7
-                # x   x   x   x
-                mask_pattern_fn = lambda arr: arr[0::2]
-            elif mask_pattern == "odd":
-                # 0 1 2 3 4 5 6 7
-                #   x   x   x   x
-                mask_pattern_fn = lambda arr: arr[1::2]
-            elif mask_pattern == "inside":
-                # 0 1 2 3 4 5 6 7
-                #     x x x x
-                mask_pattern_fn = (
-                    lambda arr: arr[
-                        len(arr) // 2
-                        - len(arr) // 4 : len(arr) // 2
-                        + len(arr) // 4 : 1
-                    ]
-                    if len(arr) > 2
-                    else [arr[1]]
-                )  # inside
-            elif mask_pattern == "outside":
-                # 0 1 2 3 4 5 6 7
-                # x x         x x
-                mask_pattern_fn = (
-                    lambda arr: [
-                        item
-                        for item in arr
-                        if not (
-                            item
-                            in arr[
-                                len(arr) // 2
-                                - len(arr) // 4 : len(arr) // 2
-                                + len(arr) // 4 : 1
-                            ]
-                        )
-                    ]
-                    if len(arr) > 2
-                    else [arr[0]]
-                )  # outside
-            else:
-                # Assume pattern is in form contains a string specifying which indices to remove
-                # For example "01001" removes idx 1 and 4 or qubit 2 and 5
-                # The important thing here is for pool pattern to be the same length as the current number of qubits
-                if len(mask_pattern) == len(Qp_l):
-                    mask_pattern_fn = lambda arr: [
-                        item
-                        for item, indicator in zip(arr, mask_pattern)
-                        if indicator == "1"
-                    ]
+    def wildcard_populate(self, pattern, length):
+        # Wildcard pattern
+        n_stars = pattern.count("*")
+        n_excl = pattern.count("!")
+        # base = pattern.replace("*", "0" * zero_per_star)
+        # base = base.replace("!", "1" * zero_per_star)
+        base = pattern
+        max_it = length
+        do_star = True if n_stars > 0 else False
+        just_changed = False
+        stars_found = 0
+        excls_found = 0
+        while len(base) < (length + n_stars + n_excl) and max_it > 0:
+            """
+            TODO refactor this code so that it is more readable. The idea is this:
+            There are two possible wild cards, excl: ! and star: *. ! fills with 1's and * fills with 0's. We want to distribute 0's and 1's as evenly as we can based on the provided pattern. Some examples, if we have 8 qubits:
+            1*1 -> 10000001
+            0!0 -> 01111110
+            *! -> 00001111
+            *1* -> 00001000
+            The algorithm alternates between finding a star and an excl and inserts a 0 or 1 next to it. The first iteration checks for a star (since we need to pick one), therefore it has a kind of precedence, but only effects the first insertion. From there it alternates between star and excl.
+
+            We have another alternation which is between using find and rfind, this is to handle the case when there's 2 stars or 2 exclamations. I don't think 3 wild cards make sense TODO think about this.
+            """
+            if do_star:
+                if stars_found % 2 == 0:
+                    idx = base.find("*")
                 else:
-                    # Attempt to use the pattern as a base pattern
-                    # TODO explain in docs and maybe print a warning
-                    # For example "101" will be used as "10110110" if there are 8 qubits
-                    if any("*" == c for c in mask_pattern):
-                        # Wildcard pattern
-                        n_ones = mask_pattern.count("1")
-                        n_stars = mask_pattern.count("*")
-                        n_zeros = len(Qp_l) - n_ones
-                        zero_per_star = n_zeros // n_stars
-                        base = mask_pattern.replace("*", "0" * zero_per_star)
-                        max_it = len(Qp_l)
-                        while len(base) < len(Qp_l) and max_it > 0:
-                            # get index of first 0
-                            idx = base.find("0")
-                            # Insert 0 next to it
-                            base = base[:idx] + "0" + base[idx:]
-                            max_it -= 1
-                        # if n_zeros <= 0:
-                        #     # We go as far as we can with a pattern and then fill everything with 0s if we can't fit the pattern
-                        #     base = "0" * len(Qp_l)
-                        # else:
-                        #     base = mask_pattern.replace("*", "0" * n_zeros)
-                        mask_pattern_fn = lambda arr: [
-                            item
-                            for item, indicator in zip(arr, base)
-                            if indicator == "1"
-                        ]
-                    else:
-                        # If there are no wildcard characters, then we assume that the pattern is a base pattern
-                        # and we will repeat it until it is the same length as the current number of qubits
-                        base = mask_pattern * (len(Qp_l) // len(mask_pattern))
-                        base = base[: len(Qp_l)]
-                        mask_pattern_fn = lambda arr: [
-                            item
-                            for item, indicator in zip(arr, base)
-                            if indicator == "1"
-                        ]
+                    idx = base.rfind("*")
+                stars_found += 1
+                # Insert 0 next to it
+                base = base[:idx] + "0" + base[idx:]
+                do_star = False if n_excl > 0 else True
+                just_changed = True
+            if (not do_star) and (not just_changed):
+                if excls_found % 2 == 0:
+                    idx = base.find("!")
+                else:
+                    idx = base.rfind("!")
+                excls_found += 1
+                # Insert 1 next to it
+                base = base[:idx] + "1" + base[idx:]
+                do_star = True if n_stars > 0 else False
+            just_changed = False
+            max_it -= 1
+        base = base.replace("*", "")
+        base = base.replace("!", "")
+        return base
+
+    def get_pattern_fn(self, pattern, length):
+        # If pattern is a string then convert it to a lambda function
+        if isinstance(pattern, str):
+            # If pattern contains wild cards, then we need to populate it
+            if any(("*" == c) or ("!" == c) for c in pattern):
+                pattern = self.wildcard_populate(pattern, length)
+            if len(pattern) < length:
+                # If there are no wildcard characters, then we assume that the pattern is a base pattern and we will repeat it until it is the same length as the current number of qubits
+                base = pattern * (length // len(pattern))
+                pattern = base[:length]
+            # Pattern is now a string of 1's and 0's and have length >= lengthor some predefined string
+            if all(c in ["0", "1"] for c in pattern):
+                pattern_fn = lambda arr: [
+                    item for item, indicator in zip(arr, pattern) if indicator == "1"
+                ]
+            else:
+                # Pattern must be predefined string
+                pattern_fn = self.get_predefined_pattern_fn(pattern)
+        # If pattern is already in lambda function form, then just use it
+        else:
+            # Check if pattern is function
+            if callable(pattern):
+                pattern_fn = pattern
+            else:
+                raise Exception("Pattern must be a string or a lambda function")
+        return pattern_fn
 
+    def cycle_between_splits(
+        self, E_a, E_b, stride=0, step=1, offset=0, boundary="open"
+    ):
+        if boundary == "open":
+            E = [
+                (
+                    E_a[i],
+                    E_b[(i + stride)],
+                )
+                for i in range(offset, len(E_a), step)
+                if (i + stride) < len(E_b)
+            ]
+        elif boundary == "periodic":
+            E = [
+                (
+                    E_a[i],
+                    E_b[(i + stride) % len(E_b)],
+                )
+                for i in range(offset, len(E_a), step)
+            ]
         else:
-            mask_pattern_fn = mask_pattern
-        return mask_pattern_fn
+            raise Exception("Boundary must be either open or periodic")
+        return E
 
+    def merge_within_splits(self, E, merge_pattern):
+        E_out = []
+        for e in E:
+            i_0 = 0
+            i_1 = 0
+            dummy = tuple()
+            for char in merge_pattern:
+                if char == "1":
+                    dummy += (e[0][i_0],)
+                    i_0 += 1
+                elif char == "0":
+                    dummy += (e[1][i_1],)
+                    i_1 += 1
+                else:
+                    raise Exception("Merge pattern must be a string of 0's and 1's")
+            E_out.append(dummy)
+        return E_out
+
+    def get_predefined_pattern_fn(self, pattern):
+        # Mapping words to the pattern type
+        if pattern == "left":
+            # 0 1 2 3 4 5 6 7
+            # x x x x
+            pattern_fn = lambda arr: arr[0 : len(arr) // 2 : 1]
+        elif pattern == "right":
+            # 0 1 2 3 4 5 6 7
+            #         x x x x
+            pattern_fn = lambda arr: arr[len(arr) // 2 : len(arr) : 1]
+        elif pattern == "even":
+            # 0 1 2 3 4 5 6 7
+            # x   x   x   x
+            pattern_fn = lambda arr: arr[0::2]
+        elif pattern == "odd":
+            # 0 1 2 3 4 5 6 7
+            #   x   x   x   x
+            pattern_fn = lambda arr: arr[1::2]
+        elif pattern == "inside":
+            # 0 1 2 3 4 5 6 7
+            #     x x x x
+            pattern_fn = (
+                lambda arr: arr[
+                    len(arr) // 2 - len(arr) // 4 : len(arr) // 2 + len(arr) // 4 : 1
+                ]
+                if len(arr) > 2
+                else [arr[1]]
+            )  # inside
+        elif pattern == "outside":
+            # 0 1 2 3 4 5 6 7
+            # x x         x x
+            pattern_fn = (
+                lambda arr: [
+                    item
+                    for item in arr
+                    if not (
+                        item
+                        in arr[
+                            len(arr) // 2
+                            - len(arr) // 4 : len(arr) // 2
+                            + len(arr) // 4 : 1
+                        ]
+                    )
+                ]
+                if len(arr) > 2
+                else [arr[0]]
+            )  # outside
+        else:
+            raise ValueError(f"{pattern} - Pattern not recognized")
+        return pattern_fn
 
-class Qmask(Qmask_Base):
+class Qmask(Qsplit):
     """
     A masking motif, it masks qubits based on some pattern TODO some controlled operation where the control is not used for the rest of the circuit).
     This motif changes the available qubits for the next motif in the stack.
     """
 
     def __init__(
         self,
-        pattern="right",  # right, left, up, down, 1*1*1, lambda function
-        connection_type="cycle",  # nearest_circle, nearest_tower, nearest_square,
-        stride=0,
-        step=1,
-        offset=0,
-        boundary="periodic",
+        global_pattern="1*",
+        merge_within="1*",
+        merge_between=None,
+        strides=[1, 1, 0],
+        steps=[1, 1, 1],
+        offsets=[0, 0, 0],
+        boundaries=["open", "open", "periodic"],
         **kwargs,
     ):
         """
-        TODO Provide topology for nearest neighbor pooling., options, circle, tower, square
-        TODO Open, Periodic boundary
+        TODO allow strides,steps,offsets to be one value and repeat what was given
         """
-        self.connection_type = connection_type
-        self.stride = stride
-        self.step = step
-        self.offset = offset
-        self.boundary = boundary
-        mapping = kwargs.get("mapping", None)
-        is_default_mapping = True if mapping is None else False
-        # Initialize graph
-        super().__init__(pattern, is_default_mapping=is_default_mapping, **kwargs)
+        if isinstance(strides, int):
+            strides = [strides] * 3
+        if isinstance(strides, int):
+            steps = [steps] * 3
+        if isinstance(offsets, int):
+            offsets = [offsets] * 3
+        super().__init__(
+            global_pattern=global_pattern,
+            merge_within=merge_within,
+            merge_between=merge_between,
+            strides=strides,
+            steps=steps,
+            offsets=offsets,
+            boundaries=boundaries,
+            mask=True,
+            type=Primitive_Types.MASK,
+            **kwargs,
+        )
 
     def __call__(self, Qp_l, *args, **kwargs):
         """
         Call the motif, this is used to generate the edges and qubits of the motif (directed graph) based on it's available qubits.
         Each time a motif in the stack changes, a loop runs through the stack from the beginning and calls each motif to update the graph (the available qubits, the edges etc).
 
         Args:
@@ -774,154 +1033,74 @@
 
         Returns:
             Qpool: Returns the updated version of itself, with correct nodes and edges.
         """
         # The idea is to mask qubits based on some pattern
         # This can be done with or without applying a unitary. Applying a unitary "preserves" their information (usually through some controlled unitary)
         # This enables patterns of: pooling in quantum neural networks, coarse graining or entanglers or just plain masking
-        # The logic is as follows:
-        # First check if there are more than 1 qubit available, since we don't want to make our last available qubit unavailable.
-        # Then check if there is a associated untitary, if there is:
-        #   If arity is 2 we have some predifined patterns + the general pattern functionality
-        #       Predifined: right, left, inside, outside, even, odd, nearest_circle, nearest_tower
-        #   If arity is more, then we just have general pattern functionality
-        # General pattern works as follows:
-        #   Provided a binary string of length arity, concatenate it to itself until it is of length len(Qp_l)
-        #   Then use this binary string to mask the qubits, where 1 means mask and 0 means keep
-        # Stride, Step, Offset manages the connectivity of masked and unmasked qubits, generally we want unmasked ones to be the target
-        # of masked ones, so that we enable deffered measurement.
-        # The most general usage is providing your own pattern function
-        # TODO add this to docs and explain how to provide own pattern function.
+        # Default is mask without a mapping, making it non operational
         is_operation = False
+        # Defaults for when nothing happens (this gets changed if conditions are met, i.e. there are qubits to mask etc)
+        Ep_l = []
+        remaining_q = Qp_l
+        # If there are qubits to mask
         if len(Qp_l) > 1:
-            # Check if predifined pattern was provided
-            self.mask_pattern_fn = self.get_mask_pattern_fn(self.pattern, Qp_l)
+            # Get global pattern function based on the pattern attribute
+            self.mask_pattern_fn = self.get_pattern_fn(self.global_pattern, len(Qp_l))
+            # Apply pattern function on all available qubits
             measured_q = self.mask_pattern_fn(Qp_l)
             remaining_q = [q for q in Qp_l if not (q in measured_q)]
-            Ep_l = []
-            # Check if there is a unitary associated with the motif
-            if not (self.mapping is None):
+            if len(remaining_q) == 0:
+                # Don't do anything if all qubits were removed
+                remaining_q = Qp_l
+            elif not (self.mapping is None):
+                # there is a operation associated with the motif
                 is_operation = True
-                # All below generates edges for associated unitaries
-                if isinstance(self.pattern, str) and not (
-                    all((c in ("0", "1") for c in self.pattern))
-                ):
-                    if len(remaining_q) > 0:
-                        # TODO add nearest neighbor modulo nq
-                        if self.connection_type == "nearest_circle":
-                            Ep_l = [
-                                (
-                                    Qp_l[Qp_l.index(i)],
-                                    min(
-                                        remaining_q,
-                                        key=lambda x: abs(Qp_l.index(i) - Qp_l.index(x))
-                                        % len(remaining_q)
-                                        // 2,
-                                    ),
-                                )
-                                for i in measured_q
-                            ]
-                        elif self.connection_type == "nearest_tower":
-                            Ep_l = [
-                                (
-                                    Qp_l[Qp_l.index(i)],
-                                    min(
-                                        remaining_q,
-                                        key=lambda x: abs(
-                                            Qp_l.index(i) - Qp_l.index(x)
-                                        ),
-                                    ),
-                                )
-                                for i in measured_q
-                            ]
-                        else:
-                            Ep_l = [
-                                (
-                                    measured_q[i],
-                                    remaining_q[(i + self.stride) % len(remaining_q)],
-                                )
-                                for i in range(len(measured_q))
-                            ]
-                    else:
-                        # No qubits were pooled
-                        Ep_l = []
-                        remaining_q = Qp_l
-                else:
-                    # General pattern functionality:
-                    # TODO maybe generalize better arity > 2, currently my idea is that the pattern string should completely
-                    # specify the form of the n qubit unitary, that is length of pattern string should equal arity.
-                    if isinstance(self.pattern, str):
-                        if len(self.pattern) != self.arity:
-                            raise ValueError(
-                                f"Pattern string should be of length arity {self.arity}, if it is a string."
-                            )
-                        nq_available = len(Qp_l)
-                    if self.stride % nq_available == 0:
-                        self.stride = 1  # TODO test if this is neccesary
-                    # We generate edges the same way as convolutions
-                    if self.boundary == "open":
-                        mod_nq = lambda x: x % nq_available
-                        Ep_l = [
-                            tuple(
-                                (
-                                    Qp_l[i + j * self.stride]
-                                    for j in range(self.arity)
-                                    if i + j * self.stride < nq_available
-                                )
-                            )
-                            for i in range(self.offset, nq_available, self.step)
-                        ]
-                        # Remove all that is not "complete"
-                        Ep_l = [edge for edge in Ep_l if len(edge) == self.arity]
-
-                    else:
-                        mod_nq = lambda x: x % nq_available
-                        Ep_l = [
-                            tuple(
-                                (
-                                    Qp_l[mod_nq(i + j * self.stride)]
-                                    for j in range(self.arity)
-                                )
-                            )
-                            for i in range(self.offset, nq_available, self.step)
-                        ]
-                        # Remove all that is not "complete", i.e. contain duplicates
-                        Ep_l = [edge for edge in Ep_l if len(set(edge)) == self.arity]
-                    if (
-                        len(Ep_l) == self.arity
-                        and sum(
-                            [
-                                len(set(Ep_l[0]) - set(Ep_l[k])) == 0
-                                for k in range(self.arity)
-                            ]
-                        )
-                        == self.arity
-                    ):
-                        # If there are only as many edges as qubits, and they are the same, then we can keep only one of them
-                        Ep_l = [Ep_l[0]]
-                    # Then we apply the pattern to record which edges go away
-                    self.mask_pattern_fn = self.get_mask_pattern_fn(self.pattern, Qp_l)
-                    measured_q = [
-                        qubit for edge in Ep_l for qubit in self.mask_pattern_fn(edge)
-                    ]
-                    remaining_q = [q for q in Qp_l if not (q in measured_q)]
+                # Populate merge pattern
+                merge_within_pop = self.wildcard_populate(self.merge_within, self.arity)
+                # Count the number of 1s in the merge pattern
+                arity_m = merge_within_pop.count("1")
+                arity_r = self.arity - arity_m
+                # Generate edges for measured split
+                E_m = self.cycle(
+                    measured_q,
+                    stride=self.strides[0],
+                    step=self.steps[0],
+                    offset=self.offsets[0],
+                    boundary=self.boundaries[0],
+                    arity=arity_m,
+                )
+                # Generate edges for remaining split
+                E_r = self.cycle(
+                    remaining_q,
+                    stride=self.strides[1],
+                    step=self.steps[1],
+                    offset=self.offsets[1],
+                    boundary=self.boundaries[1],
+                    arity=arity_r,
+                )
+                # Generate edges for measured to remaining
+                if not (self.merge_between == None):
+                    # If there is a merge_between pattern
+                    pattern_fn = self.get_pattern_fn(self.merge_between, len(E_r))
+                    E_r = pattern_fn(E_r)
+
+                E_b = self.cycle_between_splits(
+                    E_a=E_m,
+                    E_b=E_r,
+                    stride=self.strides[2],
+                    step=self.steps[2],
+                    offset=self.offsets[2],
+                    boundary=self.boundaries[2],
+                )
+                # Merge the two splits based on merge pattern
+                Ep_l = self.merge_within_splits(E_b, merge_within_pop)
 
-        else:
-            # raise ValueError(
-            #     "Pooling operation not added, Cannot perform pooling on 1 qubit"
-            # )
-            # No qubits were pooled
-            # TODO make clear in documentation, no pooling is done if 1 qubit remain
-            Ep_l = []
-            remaining_q = Qp_l
-        if len(remaining_q)==0:
-            # Don't do anything if all qubits were removed
-            remaining_q=Qp_l
         super().__call__(
-            Q=Qp_l, E=Ep_l, remaining_q=remaining_q, is_operation=is_operation, **kwargs
+            Qp_l, E=Ep_l, remaining_q=remaining_q, is_operation=is_operation, **kwargs
         )
         return self
 
     def __eq__(self, other):
         if isinstance(other, Qmask):
             self_attrs = vars(self)
             other_attrs = vars(other)
@@ -931,57 +1110,236 @@
                     if attr not in other_attrs or other_attrs[attr] != value:
                         return False
 
             return True
         return False
 
 
-class Qunmask(Qmask_Base):
+class Qunmask(Qsplit):
     def __init__(
         self,
         *args,
         **kwargs,
     ):
         """
         TODO possibility to give masking motif to undo
         """
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, type=Primitive_Types.MASK, **kwargs)
 
     def __call__(self, Qp_l, *args, **kwargs):
         """
         TODO
         """
-        if self.pattern == "previous":
+        if self.global_pattern == "previous":
             current = self
             unmasked_q = []
             unmask_counts = 0
+            q_old = kwargs.get("q_initial", [])
             while current is not None:
                 current = current.prev
                 if isinstance(current, Qmask) and unmask_counts <= 0:
-                    unmasked_q = current.prev.Q
+                    unmasked_q = current.Q
+                    q_old = current.Q
                     current = None
 
                 if isinstance(current, Qunmask):
                     unmask_counts += 1
                 if isinstance(current, Qmask):
                     unmask_counts -= 1
         else:
             q_old = kwargs.get("q_initial", [])
-            self.mask_pattern_fn = self.get_mask_pattern_fn(self.pattern, q_old)
+            self.mask_pattern_fn = self.get_pattern_fn(self.global_pattern, len(q_old))
             unmasked_q = self.mask_pattern_fn(q_old)
         is_operation = False
         Ep_l = []
         unique_unmasked = [q for q in unmasked_q if q not in Qp_l]
-        new_avail_q = Qp_l + unique_unmasked
+        new_avail_q = [q for q in q_old if q in Qp_l + unique_unmasked]
         super().__call__(
-            Q=Qp_l, E=Ep_l, remaining_q=new_avail_q, is_operation=is_operation, **kwargs
+            Qp_l, E=Ep_l, remaining_q=new_avail_q, is_operation=is_operation, **kwargs
         )
         return self
 
 
+class Qpivot(Qsplit):
+    """
+    The pivot connects the set of available qubits sequentially to a fixed set of qubits. The global pattern determine the pivot points while the merge pattern determines how the qubits are passed to the mapping.
+    """
+
+    def __init__(
+        self,
+        global_pattern="1*",
+        merge_within="1*",
+        merge_between=None,
+        strides=[1, 1, 0],
+        steps=[1, 1, 1],
+        offsets=[0, 0, 0],
+        boundaries=["open", "open", "periodic"],
+        **kwargs,
+    ):
+        """
+        Allow strides,steps,offsets and boundaries to be one value and repeat what was given
+        """
+        if isinstance(strides, int):
+            strides = [strides] * 3
+        if isinstance(strides, int):
+            steps = [steps] * 3
+        if isinstance(offsets, int):
+            offsets = [offsets] * 3
+        if isinstance(boundaries, str):
+            offsets = [offsets] * 3
+
+        super().__init__(
+            global_pattern=global_pattern,
+            merge_within=merge_within,
+            merge_between=merge_between,
+            strides=strides,
+            steps=steps,
+            offsets=offsets,
+            boundaries=boundaries,
+            mask=False,
+            type=Primitive_Types.PIVOT,
+            **kwargs,
+        )
+
+    def __call__(self, Qp_l, *args, **kwargs):
+        """
+
+        Args:
+            Qp_l (list): List of available qubits.
+            *args: Variable length argument list.
+            **kwargs: Arbitrary keyword arguments, such as:
+                * mapping (tuple(function, int)):
+                    Function mapping is specified as a tuple, where the first argument is a function and the second is the number of symbols it uses. A symbol here refers to an variational paramater for a quantum circuit, i.e. crz(theta, q0, q1) <- theta is a symbol for the gate.
+
+        Returns:
+        """
+
+        # Pivot must have a mapping
+        # TODO add a defualt mapping?
+        if self.mapping is None:
+            raise Exception("Pivot must have a mapping")
+
+        # Count the number of 1s in the merge pattern
+        arity_p = self.merge_within.count("1")
+        arity_r = self.arity - arity_p
+
+        # Get global pattern function based on the pattern attribute
+        self.pivot_pattern_fn = self.get_pattern_fn(
+            self.global_pattern.replace("1", "1" * arity_p), len(Qp_l)
+        )
+        pivot_q = [
+            p
+            for i in range((len(self.pivot_pattern_fn(Qp_l)) + arity_p - 1) // arity_p)
+            for p in self.pivot_pattern_fn(Qp_l)[i * arity_p : (i + 1) * arity_p]
+        ]
+
+        remaining_q = [q for q in Qp_l if not (q in pivot_q)]
+
+        E_p = self.cycle(
+            pivot_q,
+            stride=self.strides[0],
+            step=self.steps[0],
+            offset=self.offsets[0],
+            boundary=self.boundaries[0],
+            arity=arity_p,
+        )
+
+        if arity_r > 0:
+            # Generate edges for remaining split
+            E_r = self.cycle(
+                remaining_q,
+                stride=self.strides[1],
+                step=self.steps[1],
+                offset=self.offsets[1],
+                boundary=self.boundaries[1],
+                arity=arity_r,
+            )
+
+            # If E_r empty then there were not enough qubits to satisfiy the arity
+            if len(E_r) > 0:
+                # Duplicate items in E_p to match length of E_r such that each unique item in E_p can be matched to an equal number of items in E_r
+                max_it = 0  # prevent infinite loop
+                E_tmp = E_p.copy()
+                N = len(E_r)
+                while len(E_tmp + E_p) <= N and max_it < N:
+                    E_tmp += E_p
+                    max_it += 1
+                E_p = E_tmp.copy()
+
+                # Reorder E_p so that like pivots are grouped together, i.e. remaining avaliable qubits are assigned first to the first pivot point, then the second and so on.
+                E_tmp = []
+                for i in range(N):
+                    E_tmp += E_p[i::N]
+                E_p = E_tmp.copy()
+
+                # TODO what could merge_between be used for?
+                if not (self.merge_between == None):
+                    pass
+
+                E_b = self.cycle_between_splits(
+                    E_a=E_r,
+                    E_b=E_p,
+                    stride=self.strides[2],
+                    step=self.steps[2],
+                    offset=self.offsets[2],
+                    boundary=self.boundaries[2],
+                )
+
+                E_b = [(e[1], e[0]) for e in E_b]
+
+                # Merge the two splits based on merge pattern
+                merge_within_pop = self.wildcard_populate(self.merge_within, self.arity)
+                Ep_l = self.merge_within_splits(E_b, merge_within_pop)
+            else:
+                Ep_l = []
+        else:
+            Ep_l = E_p
+
+        super().__call__(Qp_l, E=Ep_l, remaining_q=Qp_l, is_operation=True, **kwargs)
+        return self
+
+    def cycle_between_splits(
+        self, E_a, E_b, stride=0, step=1, offset=0, boundary="open"
+    ):
+        if boundary == "open":
+            E = [
+                (
+                    E_a[i],
+                    E_b[(i + stride)],
+                )
+                for i in range(offset, len(E_a), step)
+                if (i + stride) < len(E_b)
+            ]
+        elif boundary == "periodic":
+            E = [
+                (
+                    E_a[i],
+                    E_b[(i + stride) % len(E_b)],
+                )
+                for i in range(offset, len(E_a), step)
+            ]
+        else:
+            raise Exception("Boundary must be either open or periodic")
+
+        return E
+
+    def __eq__(self, other):
+        if isinstance(other, Qmask):
+            self_attrs = vars(self)
+            other_attrs = vars(other)
+
+            for attr, value in self_attrs.items():
+                if not (attr == "mask_pattern_fn"):
+                    if attr not in other_attrs or other_attrs[attr] != value:
+                        return False
+
+            return True
+        return False
+
+
 class Qhierarchy:
     """
     The main class that manages the "stack" of motifs, it handles the interaction between successive motifs and when a motifs are added to the stack,
     it updates all the others accordingly. An object of this class fully captures the architectural information of a hierarchical quantum circuit.
     It also handles function (unitary operation) mappings.
     """
 
@@ -1096,19 +1454,21 @@
 
             return get_circuit_cirq(self, symbols, **kwargs)
         else:
             if not (symbols is None):
                 self.set_symbols(symbols)
             # Default backend
             # TODO set default mapping
+            state = self.tail(self.tail.Q).state
             for layer in self:
                 for unitary in layer.edge_mapping:
                     state = unitary.function(
                         bits=unitary.edge, symbols=unitary.symbols, state=state
                     )
+            return state
 
     def get_symbols(self):
         return (symbol for layer in self for symbol in layer.get_symbols())
 
     def set_symbols(self, symbols):
         idx = 0
         for layer in self:
@@ -1124,14 +1484,19 @@
         def unitary_function(bits, symbols=None, **kwargs):
             self.update_Q(bits)
             if not (symbols is None):
                 self.set_symbols(symbols)
             return_object = None
             for layer in self:
                 for unitary in layer.edge_mapping:
+                    if isinstance(unitary.function, str):
+                        get_circuit_from_string = kwargs.get(
+                            "get_circuit_from_string", None
+                        )
+                        unitary = get_circuit_from_string(unitary)
                     return_object = unitary.function(
                         unitary.edge, unitary.symbols, **kwargs
                     )
             return return_object
 
         return unitary_function
 
@@ -1142,18 +1507,18 @@
         Args:
             motif (Qmotif): The motif to add to the stack.
 
         Returns:
             Qhierarchy: A new Qhierarchy object with the new motif added to the stack.
         """
         motif = deepcopy(motif)
-        new_hierarchy = deepcopy(self)
-        new_hierarchy.head.set_next(motif)
-        new_hierarchy.head.next.set_prev(new_hierarchy.head)
-        new_hierarchy.head = new_hierarchy.head.next
+        # old_head = deepcopy(self.head) TODO test
+        self.head.set_next(motif)
+        self.head.next.set_prev(self.head)
+        self.head = self.head.next
 
         if motif.is_operation & motif.is_default_mapping:
             mapping = None
             mappings = self.function_mappings.get(motif.type, None)
             if mappings:
                 # If function mapping was provided
                 mapping = mappings[
@@ -1162,28 +1527,26 @@
                 self.mapping_counter.update(
                     {motif.type: self.mapping_counter.get(motif.type) + 1}
                 )
                 motif.is_default_mapping = False
             else:
                 # If no function mapping was provided
                 mapping = getattr(Default_Mappings, motif.type.name).value
-            new_hierarchy.head(
-                self.head.Q_avail, mapping=mapping, q_initial=self.tail.Q
-            )
+            self.head(self.head.prev.Q_avail, mapping=mapping, q_initial=self.tail.Q)
             # self.update_symbols(motif) TODO
 
         else:
             n_symbols = len([_ for _ in self.get_symbols()])
-            new_hierarchy.head(
-                self.head.Q_avail, start_idx=n_symbols, q_initial=self.tail.Q
+            self.head(
+                self.head.prev.Q_avail, start_idx=n_symbols, q_initial=self.tail.Q
             )
             # self.update_symbols(motif) TODO
 
-        new_hierarchy.n_symbols = len([_ for _ in new_hierarchy.get_symbols()])
-        return new_hierarchy
+        self.n_symbols = len([_ for _ in self.get_symbols()])
+        return self
 
     def extend(self, motifs):
         """
         Add and update a list of motifs to the current stack of motifs call each to generate their nodes and edges according to the action of the previous motifs in the stack.
 
         Args:
             motifs (Qmotifs): A tuple of motifs to add to the stack.
@@ -1255,32 +1618,47 @@
 
 class Qinit(Qmotif):
     """
     Qinit motif, represents a freeing up qubit for the QCNN, that is making qubits available for future operations. All Qhierarchy objects start with a Qinit motif.
     It is a special motif that has no edges and is not an operation.
     """
 
-    def __init__(self, Q, **kwargs) -> None:
+    def __init__(self, Q, state=None, tensors=None, **kwargs) -> None:
         if isinstance(Q, Sequence):
             Qinit = Q
         elif type(Q) == int:
             Qinit = [i + 1 for i in range(Q)]
-        self.type = Primitive_Types.INIT
+        self.state = state
+        self.tensors = tensors
         # Initialize graph
-        super().__init__(Q=Qinit, Q_avail=Qinit, is_operation=False, **kwargs)
+        super().__init__(
+            Q=Qinit,
+            Q_avail=Qinit,
+            is_operation=False,
+            type=Primitive_Types.INIT,
+            **kwargs,
+        )
 
     def __add__(self, other):
         """
         Add a motif, motifs or hierarchy to the stack with self.Qinit available qubits.
         """
         return Qhierarchy(self) + other
 
     def __call__(self, Q, *args, **kwargs):
         """
         Calling TODO add explanation just returns the object. Kwargs and Args are ignored, it just ensures that Qinit can be called the same way operational motifs can.
         """
+        if self.tensors is not None:
+            """
+            If tensors are provided, the state is initialized as the tensor product of all the tensors.
+            """
+            dimensions = [len(self.tensors[0])]
+            state = self.tensors[0]
+            for tensor in self.tensors[1:]:
+                state = np.array(np.kron(state, tensor))
+                dimensions += [len(tensor)]
+            self.dimensions = dimensions
+            self.state = state.reshape(dimensions)
         self.set_Q(Q)
         self.set_Qavail(Q)
         return self
-
-
-# %%
```

### Comparing `hierarqcal-0.4.0/hierarqcal/pennylane/pennylane_circuits.py` & `hierarqcal-0.5.0/hierarqcal/pennylane/pennylane_circuits.py`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.4.0/hierarqcal/pennylane/pennylane_helper.py` & `hierarqcal-0.5.0/hierarqcal/pennylane/pennylane_helper.py`

 * *Files identical despite different names*

### Comparing `hierarqcal-0.4.0/hierarqcal/qiskit/qiskit_circuits.py` & `hierarqcal-0.5.0/hierarqcal/qiskit/qiskit_circuits.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from qiskit.circuit import Parameter, QuantumCircuit, QuantumRegister
 
 
 # Default cycle circuit
-def U2(bits, symbols=None, circuit=None):
+def U2(bits, symbols=None, circuit=None, **kwargs):
     """
     Default cycle circuit, a simple 2 qubit circuit with a single parameter.
 
     Args:
         bits (list(string or int)): List of qubit indices/labels, if int then the qubits will be named :code:`f"q{bits[0]}" and f"q{bits[1]}"`
         symbols (tuple(Parameter)): Tuple of symbol values (rotation angles) as a Qiskit Parameter object, can be symbolic or numeric.
         circuit (qiskit.QuantumCircuit): QuantumCircuit object to add operations to, if None then a new QuantumCircuit object will be created.
@@ -16,24 +16,24 @@
     """
     # Assume bits are strings and in the correct QASM format
     q0, q1 = QuantumRegister(1, bits[0]), QuantumRegister(1, bits[1])
     circuit.crz(symbols[0], q0, q1)
     return circuit
 
 
-def U3(bits, symbols=None, circuit=None):
+def U3(bits, symbols=None, circuit=None, **kwargs):
     # Assume bits are strings and in the correct QASM format
     q0, q1, q2 = QuantumRegister(1, bits[0]), QuantumRegister(1, bits[1]), QuantumRegister(1, bits[2])
     circuit.crz(symbols[0], q0, q1)
     circuit.crx(symbols[1], q2, q1)
     return circuit
 
 
 # Default mask circuit
-def V2(bits, symbols=None, circuit=None):
+def V2(bits, symbols=None, circuit=None, **kwargs):
     """
     Default mask circuit, a simple 2 qubit circuit with no parameters and a controlled controlled operation.
 
     Args:
         bits (list(string or int)): List of qubit indices/labels, if int then the qubit will be named :code:`f"q{bits[0]}" and f"q{bits[1]}"`
         symbols (tuple(Parameter)): Tuple of symbol values (rotation angles) as a Qiskit Parameter object, can be symbolic or numeric.
         circuit (qiskit.QuantumCircuit): QuantumCircuit object to add operations to, if None then a new QuantumCircuit object will be created.
@@ -43,15 +43,15 @@
     """
     # Assume bits are strings and in the correct QASM format
     q0, q1 = QuantumRegister(1, bits[0]), QuantumRegister(1, bits[1])
     circuit.cnot(q0, q1)
     return circuit
 
 
-def V4(bits, symbols=None, circuit=None):
+def V4(bits, symbols=None, circuit=None, **kwargs):
     q0, q1, q2, q3 = (
         QuantumRegister(1, bits[0]),
         QuantumRegister(1, bits[1]),
         QuantumRegister(1, bits[2]),
         QuantumRegister(1, bits[3]),
     )
     circuit.cnot(q0, q1)
```

### Comparing `hierarqcal-0.4.0/hierarqcal.egg-info/PKG-INFO` & `hierarqcal-0.5.0/hierarqcal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierarqcal
-Version: 0.4.0
+Version: 0.5.0
 Description-Content-Type: text/markdown
 Provides-Extra: cirq
 Provides-Extra: pennylane
 Provides-Extra: qiskit
 License-File: LICENSE.txt
 
 # HierarQcal 
@@ -25,26 +25,26 @@
 
 ## Quick example
 
 #### Building a [Quantum Convolutional Neural Network (QCNN)](https://qiskit.org/ecosystem/machine-learning/tutorials/11_quantum_convolutional_neural_networks.html) with one line of code:
 
 ```python
 from hierarqcal import Qinit, Qcycle, Qmask
-hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("right", mapping=v))*3
+hierq = Qinit(8) + (Qcycle(mapping=u) + Qmask("!*", mapping=v))*3
 ```
 
 <img src="https://github.com/matt-lourens/hierarqcal/blob/master/img/rbt_right.png?raw=true" style="border:solid 2px black;">
 
 #### Modular and hierarchical circuit building:
 ```python
 ### Reverse binary tree
 from hierarqcal import Qinit, Qcycle, Qmask
 # motif: level 1
 m1_1 = Qcycle(stride=2)
-m1_2 = Qmask(pattern="left")
+m1_2 = Qmask(global_pattern="*!")
 # motif: level 2
 m2_1 = m1_1 + m1_2
 # motif: level 3
 m3_1 = Qinit(8) + m2_1 * 3
 ```
 $m^3_1\rightarrow \text{QCNN}:$
 
@@ -83,17 +83,24 @@
 We welcome contributions to the project. Please see the [contribution guidelines](https://github.com/matt-lourens/hierarqcal/blob/master/CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md) for more information.
 
 ## License
 BSD 3-Clause "New" or "Revised" License, see [LICENSE](https://github.com/matt-lourens/hierarqcal/blob/master/LICENSE.txt) for more information.
 
 ## Citation
 ```latex
-@article{lourens2023hierarchical,
-      title={Hierarchical quantum circuit representations for neural architecture search},
-      url = {https://arxiv.org/abs/2210.15073},
-      author={Matt Lourens and Ilya Sinayskiy and Daniel K. Park and Carsten Blank and Francesco Petruccione},
-      year={2023},
-      eprint={2210.15073},
-      archivePrefix={arXiv},
-      primaryClass={quant-ph}
+@article{lourensHierarchicalQuantumCircuit2023,
+  title = {Hierarchical Quantum Circuit Representations for Neural Architecture Search},
+  author = {Lourens, Matt and Sinayskiy, Ilya and Park, Daniel K. and Blank, Carsten and Petruccione, Francesco},
+  date = {2023-08-05},
+  journaltitle = {npj Quantum Information},
+  shortjournal = {npj Quantum Inf},
+  volume = {9},
+  number = {1},
+  pages = {1--15},
+  publisher = {{Nature Publishing Group}},
+  issn = {2056-6387},
+  doi = {10.1038/s41534-023-00747-z},
+  url = {https://www.nature.com/articles/s41534-023-00747-z},
+  issue = {1},
+  langid = {english},
 }
 ```
```

### Comparing `hierarqcal-0.4.0/hierarqcal.egg-info/SOURCES.txt` & `hierarqcal-0.5.0/hierarqcal.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 hierarqcal/cirq/tf_helper.py
 hierarqcal/pennylane/__init__.py
 hierarqcal/pennylane/pennylane_circuits.py
 hierarqcal/pennylane/pennylane_helper.py
 hierarqcal/qiskit/__init__.py
 hierarqcal/qiskit/qiskit_circuits.py
 hierarqcal/qiskit/qiskit_helper.py
-tests/test_core.py
+tests/test_core.py
+tests/test_symbol_management.py
```

