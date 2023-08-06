# Comparing `tmp/z_units-0.1.3.tar.gz` & `tmp/z_units-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z_units-0.1.3.tar", last modified: Sun Jul 30 15:01:30 2023, max compression
+gzip compressed data, was "z_units-0.1.4.tar", last modified: Sun Aug  6 13:33:49 2023, max compression
```

## Comparing `z_units-0.1.3.tar` & `z_units-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.3/LICENSE
--rw-r--r--   0        0        0     2175 2023-07-29 16:04:59.100145 z_units-0.1.3/README.md
--rw-r--r--   0        0        0      480 2023-07-30 15:01:30.134987 z_units-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.3/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.3/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.3/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-07-18 14:59:00.022077 z_units-0.1.3/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1339 2023-07-30 14:56:27.281388 z_units-0.1.3/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-07-30 14:56:27.281388 z_units-0.1.3/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0    19166 2023-07-18 15:04:09.433848 z_units-0.1.3/tests/test_quantity.py
--rw-r--r--   0        0        0      476 2023-06-27 16:02:52.925927 z_units-0.1.3/tests/test_unit.py
--rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.3/z_units/__init__.py
--rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.3/z_units/config.py
--rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.3/z_units/constant.py
--rw-r--r--   0        0        0     5409 2023-07-26 14:34:40.166856 z_units-0.1.3/z_units/quantity.py
--rw-r--r--   0        0        0    23176 2023-07-26 14:34:40.157886 z_units-0.1.3/z_units/unit.py
--rw-r--r--   0        0        0     9258 2023-07-26 14:34:40.161873 z_units-0.1.3/z_units/unit_registry.py
--rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.3/z_units/util.py
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 z_units-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2230 2023-08-06 13:06:52.210501 z_units-0.1.4/README.md
+-rw-r--r--   0        0        0      480 2023-08-06 13:33:49.089383 z_units-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.4/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.4/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.4/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-08-03 13:33:01.511332 z_units-0.1.4/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1378 2023-08-06 12:54:19.106421 z_units-0.1.4/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-08-06 12:54:19.106421 z_units-0.1.4/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0    19648 2023-08-06 12:54:18.804896 z_units-0.1.4/tests/test_quantity.py
+-rw-r--r--   0        0        0      476 2023-06-27 16:02:52.925927 z_units-0.1.4/tests/test_unit.py
+-rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.4/z_units/__init__.py
+-rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.4/z_units/config.py
+-rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.4/z_units/constant.py
+-rw-r--r--   0        0        0     5937 2023-08-03 13:33:01.304806 z_units-0.1.4/z_units/quantity.py
+-rw-r--r--   0        0        0    23176 2023-07-26 14:34:40.157886 z_units-0.1.4/z_units/unit.py
+-rw-r--r--   0        0        0     9258 2023-07-26 14:34:40.161873 z_units-0.1.4/z_units/unit_registry.py
+-rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.4/z_units/util.py
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 z_units-0.1.4/PKG-INFO
```

### Comparing `z_units-0.1.3/LICENSE` & `z_units-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `z_units-0.1.3/README.md` & `z_units-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 >>> f = q.MolarFlow(3)
 >>> f
 <MolarFlow(3, 'kmol/s')>
 f.value, f.unit
 (3, <Unit('kmol/s')>)
 >>> f.to('kmol/h')
 <MolarFlow(10800.0, 'kmol/h')>
+>>> q.Length(100, 'cm') == q.Length(1000, 'mm')
+True
 >>> q.Pressure(15, 'psi').to('MPag')
 <Pressure(0.0020963594, 'MPag')>
 ```
 Related to gauge pressure, local atmospheric pressure (default: 101325 Pa) can be altered:
 
 ```python
 >>> from z_units import config
```

### Comparing `z_units-0.1.3/tests/.pytest_cache/v/cache/nodeids` & `z_units-0.1.4/tests/.pytest_cache/v/cache/nodeids`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {'insert': "[(21, 'test_quantity.py::test_operation')]"}*

```diff
@@ -16,14 +16,15 @@
     "test_quantity.py::test_mass_heat_capacity",
     "test_quantity.py::test_molar_density",
     "test_quantity.py::test_molar_entropy",
     "test_quantity.py::test_molar_flow",
     "test_quantity.py::test_molar_heat",
     "test_quantity.py::test_molar_heat_capacity",
     "test_quantity.py::test_molar_volume",
+    "test_quantity.py::test_operation",
     "test_quantity.py::test_pressure",
     "test_quantity.py::test_standard_gas_flow",
     "test_quantity.py::test_substance",
     "test_quantity.py::test_surface_tension",
     "test_quantity.py::test_temperature",
     "test_quantity.py::test_thermal_conductivity",
     "test_quantity.py::test_time",
```

### Comparing `z_units-0.1.3/tests/test_quantity.py` & `z_units-0.1.4/tests/test_quantity.py`

 * *Files 5% similar despite different names*

```diff
@@ -430,7 +430,21 @@
     assert isclose(x.to('ppm').value, 1e6, rel_tol=1e-4)
 
 
 def test_dimensionless():
     x = q.Dimensionless(1)
     assert x.unit.symbol == ''
     assert x.unit == x.base_unit
+
+
+def test_operation():
+    x = q.Length(1)
+    assert x == q.Length(1)
+    assert x != q.Length(2)
+    assert x < q.Length(2)
+    assert x <= q.Length(1)
+    assert x == q.Length(1000, 'mm')
+    assert q.Length(100, 'cm') == q.Length(1000, 'mm')
+    assert q.Length(200, 'cm') != q.Length(1000, 'mm')
+    assert q.Length(200, 'cm') >= q.Length(1000, 'mm')
+    assert q.Length(1, 'cm') * 100 == q.Length(1, 'm')
+    assert 200 * q.Length(1, 'mm') == q.Length(2, 'dm')
```

### Comparing `z_units-0.1.3/z_units/config.py` & `z_units-0.1.4/z_units/config.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.3/z_units/quantity.py` & `z_units-0.1.4/z_units/quantity.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,19 @@
             self._unit = self.unit_registry.base_unit
         else:
             self._unit = self.unit_registry.get_unit(str(unit))
 
     def to(self, unit: Union[str, Unit]):
         if self.value is None:
             return None
+        unit = self.unit_registry.get_unit(str(unit))
+        if unit == self.unit:
+            return self
         ref_value = self._unit.to_base_unit(self.value)
-        value = self.unit_registry.get_unit(str(unit)).from_base_unit(ref_value)
+        value = unit.from_base_unit(ref_value)
         return self.__class__(value, unit)
 
     @property
     def unit_registry(self) -> UnitRegistry:
         return self.get_unit_registry()
 
     def get_unit_registry(self):
@@ -39,15 +42,15 @@
         return self.unit_registry.base_unit
 
     @property
     def units(self) -> List[Unit]:
         return self.unit_registry.units
 
     def to_base(self):
-        return self.to(self.base_unit.symbol)
+        return self.to(self.base_unit)
 
     def __repr__(self):
         if isinstance(self.value, float):
             return f"<{self.__class__.__name__}({self.value:.9}, '{self.unit.symbol}')>"
         return f"<{self.__class__.__name__}({self.value}, '{self.unit.symbol}')>"
 
     def __str__(self):
@@ -67,14 +70,28 @@
             return self.__class__(self.value * other, self.unit)
 
         return NotImplemented
 
     def __rmul__(self, other):
         return self * other
 
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return self.to_base().value == other.to_base().value
+
+        return False
+
+    def __gt__(self, other):
+        if isinstance(other, self.__class__):
+            return self.to_base().value > other.to_base().value
+
+    def __ge__(self, other):
+        if isinstance(other, self.__class__):
+            return self.to_base().value >= other.to_base().value
+
     @property
     def unit(self) -> Unit:
         return self._unit
 
 
 class Length(Quantity):
     def get_unit_registry(self):
```

### Comparing `z_units-0.1.3/z_units/unit.py` & `z_units-0.1.4/z_units/unit.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.3/z_units/unit_registry.py` & `z_units-0.1.4/z_units/unit_registry.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.3/z_units/util.py` & `z_units-0.1.4/z_units/util.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.3/PKG-INFO` & `z_units-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z-units
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple unit converter for chemical engineers
 Author-Email: zenius <zenius@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zxzenius/z-units
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -30,14 +30,16 @@
 >>> f = q.MolarFlow(3)
 >>> f
 <MolarFlow(3, 'kmol/s')>
 f.value, f.unit
 (3, <Unit('kmol/s')>)
 >>> f.to('kmol/h')
 <MolarFlow(10800.0, 'kmol/h')>
+>>> q.Length(100, 'cm') == q.Length(1000, 'mm')
+True
 >>> q.Pressure(15, 'psi').to('MPag')
 <Pressure(0.0020963594, 'MPag')>
 ```
 Related to gauge pressure, local atmospheric pressure (default: 101325 Pa) can be altered:
 
 ```python
 >>> from z_units import config
```

