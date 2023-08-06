# Comparing `tmp/unic-0.1.0.tar.gz` & `tmp/unic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.1.0.tar", max compression
+gzip compressed data, was "unic-0.1.1.tar", max compression
```

## Comparing `unic-0.1.0.tar` & `unic-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.1.0/LICENSE
--rw-r--r--   0        0        0      843 2023-08-02 13:34:57.968063 unic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1623 2023-08-02 13:34:57.957684 unic-0.1.0/README.md
--rw-r--r--   0        0        0      127 2023-08-02 13:34:57.987478 unic-0.1.0/unic/__init__.py
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.1.0/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.1.0/unic/configs/unit/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.987478 unic-0.1.0/unic/timeobject/__init__.py
--rw-r--r--   0        0        0     2056 2023-08-02 13:34:57.987478 unic-0.1.0/unic/timeobject/timeobject.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.1.0/unic/unit/__init__.py
--rw-r--r--   0        0        0     1987 2023-08-02 13:34:58.001500 unic-0.1.0/unic/unit/timeunit.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.1.0/unic/unixtime/__init__.py
--rw-r--r--   0        0        0      889 2023-08-02 13:34:58.004259 unic-0.1.0/unic/unixtime/unixtime.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.1.0/unic/utils/__init__.py
--rw-r--r--   0        0        0      673 2023-08-02 13:34:58.004259 unic-0.1.0/unic/utils/check_parameter.py
--rw-r--r--   0        0        0      391 2023-08-02 13:34:58.004259 unic-0.1.0/unic/utils/config_parser.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 unic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.1.1/LICENSE
+-rw-r--r--   0        0        0      843 2023-08-06 14:15:38.996439 unic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1539 2023-08-05 05:54:33.805710 unic-0.1.1/README.md
+-rw-r--r--   0        0        0      127 2023-08-06 14:15:30.709679 unic-0.1.1/unic/__init__.py
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.1.1/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.1.1/unic/configs/unit/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.987478 unic-0.1.1/unic/timeobject/__init__.py
+-rw-r--r--   0        0        0     2056 2023-08-02 13:34:57.987478 unic-0.1.1/unic/timeobject/timeobject.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.1.1/unic/unit/__init__.py
+-rw-r--r--   0        0        0     1982 2023-08-05 06:11:01.782318 unic-0.1.1/unic/unit/timeunit.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.1.1/unic/unixtime/__init__.py
+-rw-r--r--   0        0        0      889 2023-08-02 13:34:58.004259 unic-0.1.1/unic/unixtime/unixtime.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.1.1/unic/utils/__init__.py
+-rw-r--r--   0        0        0      673 2023-08-02 13:34:58.004259 unic-0.1.1/unic/utils/check_parameter.py
+-rw-r--r--   0        0        0      391 2023-08-02 13:34:58.004259 unic-0.1.1/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 unic-0.1.1/PKG-INFO
```

### Comparing `unic-0.1.0/LICENSE` & `unic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.1.0/pyproject.toml` & `unic-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'unixtime']
```

### Comparing `unic-0.1.0/README.md` & `unic-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,16 @@
     - unixtime / unixtime+timezone → datetime.datetime
     - unixtime / unixtime+timezone → datetime.date
   - Unix Time
     - string(yyyy-mm-dd hh:mm:ss) / string(yyyy-mm-dd hh:mm:ss)+timezone → unixtime
 
 ## Installing
 
-  - Local install using pip.
-
   ```
-  git clone https://github.com/subretu/unic.git
-  pip install ./unic/
+  pip install unic
   ```
 
 
 
 ## Example
 
 ### Time Unit
```

### Comparing `unic-0.1.0/unic/configs/timezone/settings.toml` & `unic-0.1.1/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.1.0/unic/timeobject/timeobject.py` & `unic-0.1.1/unic/timeobject/timeobject.py`

 * *Files identical despite different names*

### Comparing `unic-0.1.0/unic/unit/timeunit.py` & `unic-0.1.1/unic/unit/timeunit.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )
 from unic.utils import config_parser
 from fractions import Fraction
 from typing import Union
 
 
 class TimeUnitModel(BaseModel):
-    # 自動変換を防ぐ型で定義
+    # Prevent automatic conversion
     data: Union[StrictInt, StrictFloat]
     from_unit: StrictStr
     to_unit: StrictStr
 
     @field_validator("from_unit")
     def from_unit_check(cls, v):
         valid_units = ["msec", "sec", "min", "hour"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `unic-0.1.0/unic/unixtime/unixtime.py` & `unic-0.1.1/unic/unixtime/unixtime.py`

 * *Files identical despite different names*

### Comparing `unic-0.1.0/unic/utils/check_parameter.py` & `unic-0.1.1/unic/utils/check_parameter.py`

 * *Files identical despite different names*

### Comparing `unic-0.1.0/PKG-INFO` & `unic-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,unixtime
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
@@ -35,19 +35,16 @@
     - unixtime / unixtime+timezone → datetime.datetime
     - unixtime / unixtime+timezone → datetime.date
   - Unix Time
     - string(yyyy-mm-dd hh:mm:ss) / string(yyyy-mm-dd hh:mm:ss)+timezone → unixtime
 
 ## Installing
 
-  - Local install using pip.
-
   ```
-  git clone https://github.com/subretu/unic.git
-  pip install ./unic/
+  pip install unic
   ```
 
 
 
 ## Example
 
 ### Time Unit
```

