# Comparing `tmp/segytools-0.2.1.tar.gz` & `tmp/segytools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segytools-0.2.1.tar", max compression
+gzip compressed data, was "segytools-0.2.2.tar", max compression
```

## Comparing `segytools-0.2.1.tar` & `segytools-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.2.1/LICENSE
--rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.2.1/README.md
--rw-r--r--   0        0        0      870 2023-07-24 10:01:38.982087 segytools-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1274 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/__init__.py
--rw-r--r--   0        0        0     2223 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/datatypes.py
--rw-r--r--   0        0        0     5249 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/segy_abstract_header.py
--rw-r--r--   0        0        0    15798 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/segy_file_header.py
--rw-r--r--   0        0        0     9597 2023-07-24 10:01:38.982087 segytools-0.2.1/src/segytools/segy_header_item.py
--rw-r--r--   0        0        0    36170 2023-07-24 10:01:38.985421 segytools-0.2.1/src/segytools/segy_trace_header.py
--rw-r--r--   0        0        0     3602 2023-07-24 10:01:38.985421 segytools-0.2.1/src/segytools/toolkit.py
--rw-r--r--   0        0        0     1154 2023-07-24 10:01:38.985421 segytools-0.2.1/src/segytools/utils.py
--rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 segytools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.2.2/README.md
+-rw-r--r--   0        0        0      870 2023-08-06 19:40:53.942736 segytools-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1274 2023-07-24 10:01:38.982087 segytools-0.2.2/src/segytools/__init__.py
+-rw-r--r--   0        0        0     2223 2023-07-24 10:01:38.982087 segytools-0.2.2/src/segytools/datatypes.py
+-rw-r--r--   0        0        0     5249 2023-07-24 10:01:38.982087 segytools-0.2.2/src/segytools/segy_abstract_header.py
+-rw-r--r--   0        0        0    15798 2023-07-24 10:01:38.982087 segytools-0.2.2/src/segytools/segy_file_header.py
+-rw-r--r--   0        0        0     9597 2023-07-24 10:01:38.982087 segytools-0.2.2/src/segytools/segy_header_item.py
+-rw-r--r--   0        0        0    36170 2023-07-24 10:01:38.985421 segytools-0.2.2/src/segytools/segy_trace_header.py
+-rw-r--r--   0        0        0     2218 2023-08-06 19:40:13.432737 segytools-0.2.2/src/segytools/toolkit.py
+-rw-r--r--   0        0        0     3596 2023-08-06 19:40:13.432737 segytools-0.2.2/src/segytools/utils.py
+-rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 segytools-0.2.2/PKG-INFO
```

### Comparing `segytools-0.2.1/LICENSE` & `segytools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/README.md` & `segytools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/pyproject.toml` & `segytools-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "segytools"
-version = "0.2.1"
+version = "0.2.2"
 description = "low level toolkit for manipulating and analyzing segy formatted data"
 authors = ["anthonytorlucci <anthonytorlucci@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `segytools-0.2.1/src/segytools/__init__.py` & `segytools-0.2.2/src/segytools/__init__.py`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/src/segytools/datatypes.py` & `segytools-0.2.2/src/segytools/datatypes.py`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/src/segytools/segy_abstract_header.py` & `segytools-0.2.2/src/segytools/segy_abstract_header.py`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/src/segytools/segy_file_header.py` & `segytools-0.2.2/src/segytools/segy_file_header.py`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/src/segytools/segy_header_item.py` & `segytools-0.2.2/src/segytools/segy_header_item.py`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/src/segytools/segy_trace_header.py` & `segytools-0.2.2/src/segytools/segy_trace_header.py`

 * *Files identical despite different names*

### Comparing `segytools-0.2.1/src/segytools/toolkit.py` & `segytools-0.2.2/src/segytools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
-Collection of tools for working with segy data
+Utility functions for segy data.
+"""
 
-Copyright 2022 Anthony Torlucci
+# Copyright 2022 Anthony Torlucci
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 # standard
 import textwrap
 
 # third party
 import numpy
 from ibm2ieee import ibm2float32, ibm2float64
@@ -92,8 +93,7 @@
         trc = numpy.frombuffer(buf, dtype=dt)
     elif fmt.ctype == 'ibm':
         trc = ibm2float64(numpy.frombuffer(buffer=buf, dtype=''.join([byteorder,'u4'])))
     else:
         raise ValueError("fmt is an unsupported DataSampleFormat.")
 
     return trc
-
```

### Comparing `segytools-0.2.1/PKG-INFO` & `segytools-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segytools
-Version: 0.2.1
+Version: 0.2.2
 Summary: low level toolkit for manipulating and analyzing segy formatted data
 License: MIT
 Author: anthonytorlucci
 Author-email: anthonytorlucci@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

