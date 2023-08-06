# Comparing `tmp/launart-0.6.4.tar.gz` & `tmp/launart-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launart-0.6.4.tar", last modified: Sat Aug  5 12:55:11 2023, max compression
+gzip compressed data, was "launart-0.7.0.tar", last modified: Sun Aug  6 13:00:28 2023, max compression
```

## Comparing `launart-0.6.4.tar` & `launart-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-08-05 12:54:59.880786 launart-0.6.4/LICENSE
--rw-r--r--   0        0        0      929 2023-08-05 12:54:59.880786 launart-0.6.4/README.md
--rw-r--r--   0        0        0      591 2023-08-05 12:54:59.880786 launart-0.6.4/launart/__init__.py
--rw-r--r--   0        0        0     1099 2023-08-05 12:54:59.880786 launart-0.6.4/launart/_sideload.py
--rw-r--r--   0        0        0     7195 2023-08-05 12:54:59.880786 launart-0.6.4/launart/component.py
--rw-r--r--   0        0        0    21879 2023-08-05 12:54:59.880786 launart-0.6.4/launart/manager.py
--rw-r--r--   0        0        0     1020 2023-08-05 12:54:59.880786 launart-0.6.4/launart/saya.py
--rw-r--r--   0        0        0      713 2023-08-05 12:54:59.880786 launart-0.6.4/launart/service.py
--rw-r--r--   0        0        0     3722 2023-08-05 12:54:59.880786 launart-0.6.4/launart/utilles.py
--rw-r--r--   0        0        0     1552 2023-08-05 12:55:11.857344 launart-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      122 2023-08-05 12:54:59.880786 launart-0.6.4/tests/_saya_mod/empty_sub.py
--rw-r--r--   0        0        0      135 2023-08-05 12:54:59.880786 launart-0.6.4/tests/_saya_mod/fail_sub.py
--rw-r--r--   0        0        0      947 2023-08-05 12:54:59.880786 launart-0.6.4/tests/_saya_mod/ok_sub.py
--rw-r--r--   0        0        0     2062 2023-08-05 12:54:59.880786 launart-0.6.4/tests/fixture.py
--rw-r--r--   0        0        0     4269 2023-08-05 12:54:59.880786 launart-0.6.4/tests/launchable.py
--rw-r--r--   0        0        0    10571 2023-08-05 12:54:59.880786 launart-0.6.4/tests/manager.py
--rw-r--r--   0        0        0     1106 2023-08-05 12:54:59.880786 launart-0.6.4/tests/saya.py
--rw-r--r--   0        0        0     2416 2023-08-05 12:54:59.880786 launart-0.6.4/tests/sideload.py
--rw-r--r--   0        0        0     3033 2023-08-05 12:54:59.880786 launart-0.6.4/tests/utils.py
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 launart-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-06 13:00:11.757793 launart-0.7.0/LICENSE
+-rw-r--r--   0        0        0      929 2023-08-06 13:00:11.757793 launart-0.7.0/README.md
+-rw-r--r--   0        0        0      520 2023-08-06 13:00:11.757793 launart-0.7.0/launart/__init__.py
+-rw-r--r--   0        0        0      913 2023-08-06 13:00:11.757793 launart-0.7.0/launart/_sideload.py
+-rw-r--r--   0        0        0    19050 2023-08-06 13:00:11.757793 launart-0.7.0/launart/manager.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:00:11.757793 launart-0.7.0/launart/ryanvk/__init__.py
+-rw-r--r--   0        0        0      993 2023-08-06 13:00:11.757793 launart-0.7.0/launart/saya.py
+-rw-r--r--   0        0        0     3615 2023-08-06 13:00:11.757793 launart-0.7.0/launart/service.py
+-rw-r--r--   0        0        0     3825 2023-08-06 13:00:11.757793 launart-0.7.0/launart/status.py
+-rw-r--r--   0        0        0     3259 2023-08-06 13:00:11.757793 launart-0.7.0/launart/utilles.py
+-rw-r--r--   0        0        0     1552 2023-08-06 13:00:28.841802 launart-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-08-06 13:00:11.757793 launart-0.7.0/tests/_saya_mod/empty_sub.py
+-rw-r--r--   0        0        0      129 2023-08-06 13:00:11.757793 launart-0.7.0/tests/_saya_mod/fail_sub.py
+-rw-r--r--   0        0        0      662 2023-08-06 13:00:11.757793 launart-0.7.0/tests/_saya_mod/ok_sub.py
+-rw-r--r--   0        0        0     1637 2023-08-06 13:00:11.757793 launart-0.7.0/tests/fixture.py
+-rw-r--r--   0        0        0     3773 2023-08-06 13:00:11.757793 launart-0.7.0/tests/launchable.py
+-rw-r--r--   0        0        0     8666 2023-08-06 13:00:11.757793 launart-0.7.0/tests/manager.py
+-rw-r--r--   0        0        0     1085 2023-08-06 13:00:11.757793 launart-0.7.0/tests/saya.py
+-rw-r--r--   0        0        0     2462 2023-08-06 13:00:11.757793 launart-0.7.0/tests/sideload.py
+-rw-r--r--   0        0        0     1994 2023-08-06 13:00:11.757793 launart-0.7.0/tests/utils.py
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 launart-0.7.0/PKG-INFO
```

### Comparing `launart-0.6.4/LICENSE` & `launart-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launart-0.6.4/README.md` & `launart-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `launart-0.6.4/launart/_sideload.py` & `launart-0.7.0/launart/_sideload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from __future__ import annotations
 
-from collections import ChainMap
 from typing import TYPE_CHECKING, Any, Dict, TypeVar, cast
 
 if TYPE_CHECKING:
-    from launart.manager import U_ManagerStage
+    from launart.status import U_ManagerStage
 
 
 class Override:
     def __init__(self, source: Any, additional: Dict[str, Any]):
         self.__source = source
         self.__additional = additional
 
     @property
     def source(self):
         return self.__source
 
-    @property
-    def __data(self):
-        return ChainMap(self.__additional, vars(self.__source))
-
     def __getattr__(self, item):
-        if item not in self.__data:
-            raise AttributeError(f"'{self.__source.__class__.__name__}' object has no attribute '{item}'")
-        return self.__data[item]
+        if item in self.__additional:
+            return self.__additional[item]
+        return getattr(self.__source, item)
 
 
 T = TypeVar("T")
 
 
 def override(source: T, additional: Dict[str, Any]) -> T:
     return cast(T, Override(source, additional))
```

### Comparing `launart-0.6.4/pyproject.toml` & `launart-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launart"
-version = "0.6.4"
+version = "0.7.0"
 description = "Component lifetime manager for runtime."
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "statv>=0.2.2",
     "loguru>=0.6.0",
```

### Comparing `launart-0.6.4/tests/saya.py` & `launart-0.7.0/tests/saya.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-
 import pytest
 from graia.saya import Saya
 from graia.saya.behaviour.entity import Behaviour
 from graia.saya.schema import BaseSchema
 
 from launart.manager import Launart
 from launart.saya import LaunartBehaviour
@@ -26,14 +25,14 @@
 
     empty_mod = saya.require("tests._saya_mod.empty_sub")
 
     with pytest.raises(TypeError):
         saya.require("tests._saya_mod.fail_sub")
 
     channel = saya.require("tests._saya_mod.ok_sub")
-    assert "launchable.test.saya" in mgr.launchables
-    assert "service.test.saya" in mgr.launchables
+    assert "lc.test.saya" in mgr.components
+    assert "service.test.saya" in mgr.components
     saya.uninstall_channel(channel)
-    assert "launchable.test.saya" not in mgr.launchables
-    assert "service.test.saya" not in mgr.launchables
+    assert "lc.test.saya" not in mgr.components
+    assert "service.test.saya" not in mgr.components
 
     saya.uninstall_channel(empty_mod)
```

### Comparing `launart-0.6.4/tests/utils.py` & `launart-0.7.0/tests/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
-
 import asyncio
 from typing import Any, cast
 
 import pytest
 
 from launart._sideload import Override, override
-from launart.component import RequirementResolveFailed, resolve_requirements
-from launart.utilles import priority_strategy, wait_fut
-from tests.fixture import component_standalone, interface
+from launart.utilles import wait_fut, resolve_requirements, RequirementResolveFailed
+from tests.fixture import component_standalone
 
 
 def test_resolve_success():
     dataset = [
         component_standalone("a", []),
         component_standalone("b", ["a"]),
         component_standalone("c", ["a", "b"]),
@@ -31,46 +29,14 @@
         component_standalone("a", ["b"]),
         component_standalone("b", ["a"]),
     ]
     with pytest.raises(RequirementResolveFailed):
         resolve_requirements(dataset)
 
 
-def test_priority_strategy():
-    def spit(v: Any) -> Any:
-        return v
-
-    with pytest.raises(TypeError):
-        priority_strategy([1, 2, 3], spit)
-    with pytest.raises(TypeError):
-        priority_strategy([(1, 2), 3], spit)
-
-    i = [interface() for _ in range(10)]
-
-    s1 = {i[0], i[1]}
-    s2 = {i[1], i[2]}
-    s3 = {i[2], i[3]}
-
-    d1 = {i[0]: 1, i[1]: 2}
-    d2 = {i[1]: 1, i[2]: 2}
-    d3 = {i[2]: 1, i[3]: 2}
-
-    assert priority_strategy([s1, s3], spit) == {i[0]: s1, i[1]: s1, i[2]: s3, i[3]: s3}
-
-    assert priority_strategy([d1, d2, d3], spit) == {i[0]: d1, i[1]: d1, i[2]: d2, i[3]: d3}
-
-    assert priority_strategy([d1, d3, d2], spit) == {i[0]: d1, i[1]: d1, i[2]: d2, i[3]: d3}
-
-    assert priority_strategy([(d1, d2), d3], spit) == {i[0]: (d1, d2), i[1]: (d1, d2), i[2]: (d1, d2), i[3]: d3}
-
-    with pytest.raises(ValueError):
-        priority_strategy([s1, s2], spit)
-    with pytest.raises(ValueError):
-        priority_strategy([s1, d1], spit)
-
 
 def test_override():
     class MyOrigin:
         data: dict
 
         def __init__(self, d: dict) -> None:
             self.data = d
```

### Comparing `launart-0.6.4/PKG-INFO` & `launart-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launart
-Version: 0.6.4
+Version: 0.7.0
 Summary: Component lifetime manager for runtime.
 Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: statv>=0.2.2
 Requires-Dist: loguru>=0.6.0
 Requires-Dist: creart>=0.3.0
```

