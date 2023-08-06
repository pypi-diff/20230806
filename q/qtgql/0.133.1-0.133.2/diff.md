# Comparing `tmp/qtgql-0.133.1.tar.gz` & `tmp/qtgql-0.133.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.133.1.tar", max compression
+gzip compressed data, was "qtgql-0.133.2.tar", max compression
```

## Comparing `qtgql-0.133.1.tar` & `qtgql-0.133.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1064 2023-08-03 12:33:04.450843 qtgql-0.133.1/LICENSE
--rw-r--r--   0        0        0     1116 2023-08-03 12:33:04.450843 qtgql-0.133.1/README.md
--rw-r--r--   0        0        0     4337 2023-08-03 12:33:37.266615 qtgql-0.133.1/pyproject.toml
--rw-r--r--   0        0        0       29 2023-08-03 12:33:38.110770 qtgql-0.133.1/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     2116 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1708 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3454 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1216 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3855 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3877 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    16194 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0     4441 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/operation/selections_injection.py
--rw-r--r--   0        0        0      864 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0     2208 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/operation/utils.py
--rw-r--r--   0        0        0        0 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     5521 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8761 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0     2019 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4238 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     3013 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1137 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0      513 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/serialize_input_variable.jinja.hpp
--rw-r--r--   0        0        0     5635 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4207 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5264 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     6499 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3225 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    19611 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1753 2023-08-03 12:33:04.462846 qtgql-0.133.1/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.133.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-06 15:19:00.282498 qtgql-0.133.2/LICENSE
+-rw-r--r--   0        0        0     1116 2023-08-06 15:19:00.282498 qtgql-0.133.2/README.md
+-rw-r--r--   0        0        0     4359 2023-08-06 15:19:30.386597 qtgql-0.133.2/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-08-06 15:19:31.158604 qtgql-0.133.2/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     2116 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1708 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3454 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1216 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3855 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:19:00.294499 qtgql-0.133.2/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16208 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4441 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2208 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     5521 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8768 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0     2019 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4238 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     3013 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1137 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0      513 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/serialize_input_variable.jinja.hpp
+-rw-r--r--   0        0        0     5635 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4207 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5264 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     6499 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3225 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    19632 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1753 2023-08-06 15:19:00.298499 qtgql-0.133.2/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.133.2/PKG-INFO
```

### Comparing `qtgql-0.133.1/LICENSE` & `qtgql-0.133.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/README.md` & `qtgql-0.133.2/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/pyproject.toml` & `qtgql-0.133.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.133.1"
+version = "0.133.2"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
@@ -34,14 +34,15 @@
 pygithub = ">=1.58.2"
 githubrelease = ">=1.5.9"
 httpx = ">=0.18.2"
 autopub = "0.3.0"
 mimesis = ">=10.1.0"
 pytest = "7.3.1"
 pytest-cov = ">=4.1.0"
+pre-commit = "^3.3.3"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.5"
 mike = "^1.1.2"
 markdown-include = "^0.8.0"
 mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.22.0"}
```

### Comparing `qtgql-0.133.1/qtgqlcodegen/cli.py` & `qtgql-0.133.2/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/config.py` & `qtgql-0.133.2/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/core/cppref.py` & `qtgql-0.133.2/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.133.2/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/core/template.py` & `qtgql-0.133.2/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/generator.py` & `qtgql-0.133.2/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/operation/definitions.py` & `qtgql-0.133.2/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.133.2/qtgqlcodegen/operation/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     elif named_type := is_named_type_node(node):
         ret = type_info.get_type(named_type.name.value)
 
     if not ret:  # pragma: no cover
         raise NotImplementedError(node, "Type is not supported as a variable ATM")
 
     if is_optional:
-        return QtGqlOptional(of_type=ret)
+        return QtGqlOptional(wrapped_type__=ret)
     return ret
 
 
 def _evaluate_variable(
     type_info: SchemaTypeInfo,
     var: gql_lang.VariableDefinitionNode,
 ) -> QtGqlVariableDefinition:
@@ -152,15 +152,15 @@
             path=path,
         )
 
     if not ret:  # pragma: no cover
         raise NotImplementedError(f"type {concrete_type} not supported yet")
 
     if concrete_type.is_optional:
-        return QtGqlOptional(of_type=ret)
+        return QtGqlOptional(wrapped_type__=ret)
     return ret
 
 
 def _evaluate_field(
     type_info: OperationTypeInfo,
     concrete_field: QtGqlFieldDefinition,
     field_node: gql_lang.FieldNode,
```

### Comparing `qtgql-0.133.1/qtgqlcodegen/operation/selections_injection.py` & `qtgql-0.133.2/qtgqlcodegen/operation/selections_injection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/operation/template.py` & `qtgql-0.133.2/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/operation/utils.py` & `qtgql-0.133.2/qtgqlcodegen/operation/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/schema/definitions.py` & `qtgql-0.133.2/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.133.2/qtgqlcodegen/schema/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     elif interface_def := is_interface_definition(t):
         ret = _evaluate_interface_type(type_info, interface_def)
     if not ret:  # pragma: no cover
         raise NotImplementedError(f"type {t} not supported yet")
 
     if is_optional:
-        return QtGqlOptional(of_type=ret)
+        return QtGqlOptional(wrapped_type__=ret)
     return ret
 
 
 def evaluate_field(
     type_info: SchemaTypeInfo,
     name: str,
     field: gql_def.GraphQLField,
```

### Comparing `qtgql-0.133.1/qtgqlcodegen/schema/template.py` & `qtgql-0.133.2/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake` & `qtgql-0.133.2/qtgqlcodegen/templates/CMakeLists.jinja.cmake`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/serialize_input_variable.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/serialize_input_variable.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.133.2/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.133.2/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.133.2/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/qtgqlcodegen/types.py` & `qtgql-0.133.2/qtgqlcodegen/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,23 +130,23 @@
         raise RuntimeError("the template probobly tried to render this object")
 
 
 @define
 class QtGqlOptional(QtGqlTypeABC):
     """Represents GraphQL types that are not marked with "!"."""
 
-    of_type: QtGqlTypeABC
+    wrapped_type__: QtGqlTypeABC
 
     def __getattr__(self, item):
         if item == "is_optional":
             return True
-        return getattr(self.of_type, item)
+        return getattr(self.wrapped_type__, item)
 
     def __getattribute__(self, name):
-        if name not in ("of_type"):
+        if name not in ("wrapped_type__"):
             raise AttributeError
         else:
             return super().__getattribute__(name)
 
     def type_name(self) -> str:  # pragma: no cover
         raise NotImplementedError
```

### Comparing `qtgql-0.133.1/qtgqlcodegen/utils.py` & `qtgql-0.133.2/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.133.1/PKG-INFO` & `qtgql-0.133.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.133.1
+Version: 0.133.2
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
```

