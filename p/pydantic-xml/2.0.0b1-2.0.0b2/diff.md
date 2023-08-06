# Comparing `tmp/pydantic_xml-2.0.0b1.tar.gz` & `tmp/pydantic_xml-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-2.0.0b1.tar", max compression
+gzip compressed data, was "pydantic_xml-2.0.0b2.tar", max compression
```

## Comparing `pydantic_xml-2.0.0b1.tar` & `pydantic_xml-2.0.0b2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1211 2023-07-30 08:33:00.589908 pydantic_xml-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     3335 2023-07-30 08:33:00.589908 pydantic_xml-2.0.0b1/README.rst
--rw-r--r--   0        0        0      453 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    14764 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      374 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      712 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/errors.py
--rw-r--r--   0        0        0    12352 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/py.typed
--rw-r--r--   0        0        0       36 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0      113 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     3386 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     3290 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     5492 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0    11717 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     5639 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     5081 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/tagged_union.py
--rw-r--r--   0        0        0     1428 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/typed_mapping.py
--rw-r--r--   0        0        0     5135 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2659 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0    10099 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0      322 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1946 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-08-06 15:16:57.924280 pydantic_xml-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0     3335 2023-08-06 15:16:57.924280 pydantic_xml-2.0.0b2/README.rst
+-rw-r--r--   0        0        0      453 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    14764 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      374 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      712 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    12416 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       36 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0      113 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     3386 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     3290 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     5492 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0    11717 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     5639 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     5081 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/tagged_union.py
+-rw-r--r--   0        0        0     1428 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/typed_mapping.py
+-rw-r--r--   0        0        0     5135 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2659 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0    10099 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0      322 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1935 2023-08-06 15:16:57.928280 pydantic_xml-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0b2/PKG-INFO
```

### Comparing `pydantic_xml-2.0.0b1/LICENSE` & `pydantic_xml-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/README.rst` & `pydantic_xml-2.0.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/element/element.py` & `pydantic_xml-2.0.0b2/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/element/native/lxml.py` & `pydantic_xml-2.0.0b2/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/element/native/std.py` & `pydantic_xml-2.0.0b2/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/errors.py` & `pydantic_xml-2.0.0b2/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/model.py` & `pydantic_xml-2.0.0b2/pydantic_xml/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses as dc
 import typing
 from typing import Any, Callable, ClassVar, Dict, Generic, Optional, Tuple, Type, TypeVar, Union
 
 import pydantic as pd
 import pydantic_core as pdc
 from pydantic import BaseModel, RootModel
+from pydantic._internal._model_construction import ModelMetaclass  # noqa
 
 from . import config, errors, utils
 from .element import SearchMode
 from .element.native import XmlElement, etree
 from .serializers.factories.model import BaseModelSerializer
 from .serializers.serializer import Serializer, XmlEntityInfoP
 from .typedefs import EntityLocation
@@ -195,29 +196,29 @@
     :param nsmap: element xml namespace map
     :param kwargs: pydantic field arguments. See :py:class:`pydantic.Field`
     """
 
     return XmlEntityInfo(EntityLocation.WRAPPED, path=path, ns=ns, nsmap=nsmap, wrapped=entity, **kwargs)
 
 
-class XmlModelMeta(type(BaseModel)):  # type: ignore[misc]
+class XmlModelMeta(ModelMetaclass):
     """
     Xml model metaclass.
     """
 
     def __new__(
             mcls,
             name: str,
             bases: Tuple[type],
             namespace: Dict[str, Any],
             **kwargs: Any,
     ) -> Type['BaseXmlModel']:
         is_abstract: bool = kwargs.pop('__xml_abstract__', False)
 
-        cls = super().__new__(mcls, name, bases, namespace, **kwargs)
+        cls = typing.cast(Type['BaseXmlModel'], super().__new__(mcls, name, bases, namespace, **kwargs))
         if not is_abstract:
             cls.__build_serializer__()
 
         return cls
 
 
 ModelT = TypeVar('ModelT', bound='BaseXmlModel')
@@ -360,15 +361,15 @@
 
         return etree.tostring(self.to_xml_tree(skip_empty=skip_empty), **kwargs)
 
 
 RootModelRootType = TypeVar('RootModelRootType')
 
 
-class RootXmlModel(  # type: ignore[misc]
+class RootXmlModel(
     RootModel[RootModelRootType],
     BaseXmlModel,
     Generic[RootModelRootType],
     __xml_abstract__=True,
 ):
     """
     Base pydantic-xml root model.
```

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/tagged_union.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/typed_mapping.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/typed_mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/serializers/serializer.py` & `pydantic_xml-2.0.0b2/pydantic_xml/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pydantic_xml/utils.py` & `pydantic_xml-2.0.0b2/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0b1/pyproject.toml` & `pydantic_xml-2.0.0b2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "2.0.0b1"
+version = "2.0.0b2"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
 keywords = [
-    'pydantic', 'xml', 'serialization', 'deserialization', 'parsing', 'lxml',
+    'pydantic', 'xml', 'serialization', 'deserialization', 'lxml',
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: Public Domain",
     "Topic :: Software Development :: Libraries",
```

### Comparing `pydantic_xml-2.0.0b1/PKG-INFO` & `pydantic_xml-2.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
-Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
+Keywords: pydantic,xml,serialization,deserialization,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
```

