# Comparing `tmp/complex_mathematics-2.2.1.tar.gz` & `tmp/complex_mathematics-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_mathematics-2.2.1.tar", last modified: Fri Aug  4 22:33:42 2023, max compression
+gzip compressed data, was "complex_mathematics-2.3.3.tar", last modified: Sun Aug  6 18:57:41 2023, max compression
```

## Comparing `complex_mathematics-2.2.1.tar` & `complex_mathematics-2.3.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 22:33:42.176585 complex_mathematics-2.2.1/
--rw-rw-rw-   0        0        0     1092 2023-08-04 16:05:05.000000 complex_mathematics-2.2.1/LICENSE
--rw-rw-rw-   0        0        0      398 2023-08-04 22:33:42.174592 complex_mathematics-2.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 22:33:42.122732 complex_mathematics-2.2.1/complex_mathematics/
--rw-rw-rw-   0        0        0     1622 2023-08-04 16:21:52.000000 complex_mathematics-2.2.1/complex_mathematics/__init__.py
--rw-rw-rw-   0        0        0      692 2023-08-04 22:33:07.000000 complex_mathematics-2.2.1/complex_mathematics/algebra.py
--rw-rw-rw-   0        0        0     1354 2023-08-04 15:12:51.000000 complex_mathematics-2.2.1/complex_mathematics/linalg.py
--rw-rw-rw-   0        0        0     1586 2023-08-04 18:10:13.000000 complex_mathematics-2.2.1/complex_mathematics/ml.py
-drwxrwxrwx   0        0        0        0 2023-08-04 22:33:42.170600 complex_mathematics-2.2.1/complex_mathematics.egg-info/
--rw-rw-rw-   0        0        0      398 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-08-04 22:33:42.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-04 22:33:41.000000 complex_mathematics-2.2.1/complex_mathematics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 22:33:42.177583 complex_mathematics-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-08-04 22:33:00.000000 complex_mathematics-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:57:41.271464 complex_mathematics-2.3.3/
+-rw-rw-rw-   0        0        0     1092 2023-08-04 16:05:05.000000 complex_mathematics-2.3.3/LICENSE
+-rw-rw-rw-   0        0        0      393 2023-08-06 18:57:41.270469 complex_mathematics-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1516 2023-08-04 22:36:46.000000 complex_mathematics-2.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 18:57:41.252512 complex_mathematics-2.3.3/complex_mathematics/
+-rw-rw-rw-   0        0        0     1622 2023-08-04 16:21:52.000000 complex_mathematics-2.3.3/complex_mathematics/__init__.py
+-rw-rw-rw-   0        0        0      926 2023-08-06 18:51:14.000000 complex_mathematics-2.3.3/complex_mathematics/algebra.py
+-rw-rw-rw-   0        0        0     1354 2023-08-04 15:12:51.000000 complex_mathematics-2.3.3/complex_mathematics/linalg.py
+-rw-rw-rw-   0        0        0     1586 2023-08-04 18:10:13.000000 complex_mathematics-2.3.3/complex_mathematics/ml.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:57:41.267473 complex_mathematics-2.3.3/complex_mathematics.egg-info/
+-rw-rw-rw-   0        0        0      393 2023-08-06 18:57:41.000000 complex_mathematics-2.3.3/complex_mathematics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-08-06 18:57:41.000000 complex_mathematics-2.3.3/complex_mathematics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 18:57:41.000000 complex_mathematics-2.3.3/complex_mathematics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-06 18:57:41.000000 complex_mathematics-2.3.3/complex_mathematics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-06 18:57:41.000000 complex_mathematics-2.3.3/complex_mathematics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 18:57:41.271464 complex_mathematics-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-08-06 18:57:06.000000 complex_mathematics-2.3.3/setup.py
```

### Comparing `complex_mathematics-2.2.1/LICENSE` & `complex_mathematics-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `complex_mathematics-2.2.1/complex_mathematics/__init__.py` & `complex_mathematics-2.3.3/complex_mathematics/__init__.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-2.2.1/complex_mathematics/algebra.py` & `complex_mathematics-2.3.3/complex_mathematics/algebra.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import re
 import math
 import numpy as np
 
 def quadratic(equation):
-  equation = equation.replace(" ", "")
+    equation = equation.replace(" ", "")
+  
+    pattern = r'(-?\d*)x\^2([-+]?\d*)x([-+]?\d+)'
+    matches = re.match(pattern, equation)
 
-  pattern = r'([-+]?\d*)x\^2([-+]?\d*)x([-+]?\d*)'
-  matches = re.match(pattern, equation)
+    if not matches:
+        raise ValueError("Invalid quadratic equation format. Please provide a valid quadratic equation.")
 
-  a_str, b_str, c_str = matches.groups()
-  
-  a = int(a_str) if a_str and a_str not in ['+', '-'] else (1 if a_str == '' else -1)
-  b = int(b_str) if b_str and b_str not in ['+', '-'] else (1 if b_str == '' else -1)
-  c = int(c_str) if c_str else 0
-
-  try:
-
-    pos = (-b+math.sqrt(b**2-4*a*c))/(2*a)
-    neg = (-b-math.sqrt(b**2-4*a*c))/(2*a)
-    
-  except:
-
-    pos, neg = None, None
-
-  if pos == neg:
-    return np.array([pos])
-    
-  return np.array([pos, neg])
+    a_str, b_str, c_str = matches.groups()
+
+    a = int(a_str) if a_str and a_str not in '+-' else 1 if not a_str or a_str == '+' else -1
+    b = int(b_str) if b_str and b_str not in '+-' else 1 if not b_str or b_str == '+' else -1
+    c = int(c_str) if c_str and c_str not in '+-' else 1 if not c_str or c_str == '+' else -1
+
+    try:
+        pos = (-b + math.sqrt(b**2 - 4*a*c)) / (2*a)
+        neg = (-b - math.sqrt(b**2 - 4*a*c)) / (2*a)
+    except:
+        pos, neg = None, None
+
+    if pos == neg:
+        return np.array([pos])
+
+    return np.array([pos, neg])
```

### Comparing `complex_mathematics-2.2.1/complex_mathematics/linalg.py` & `complex_mathematics-2.3.3/complex_mathematics/linalg.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-2.2.1/complex_mathematics/ml.py` & `complex_mathematics-2.3.3/complex_mathematics/ml.py`

 * *Files identical despite different names*

### Comparing `complex_mathematics-2.2.1/setup.py` & `complex_mathematics-2.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='complex_mathematics',
-    version='2.2.1',
+    version='2.3.3',
     packages=find_packages(),
     install_requires=[
         'numpy', 'scipy'
     ],
     license='MIT',
     author="Arnav Malhotra",
     author_email="emumalhotra@gmail.com",
     description="Many complex math features.",
-    long_description="Many advanced math features and topics like linear algebra, geometry, calculus, algebra, and some machine learning algorithms.",
+    long_description="Many advanced math features and topics like linear algebra, geometry, calculus, algebra, and machine learning algorithms.",
     url="https://github.com/Arnav-MaIhotra/complex_mathematics",
 )
```

