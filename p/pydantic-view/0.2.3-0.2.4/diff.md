# Comparing `tmp/pydantic_view-0.2.3.tar.gz` & `tmp/pydantic_view-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.2.3.tar", max compression
+gzip compressed data, was "pydantic_view-0.2.4.tar", max compression
```

## Comparing `pydantic_view-0.2.3.tar` & `pydantic_view-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.949673 pydantic_view-0.2.3/LICENSE
--rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.636831 pydantic_view-0.2.3/README.md
--rw-r--r--   0        0        0      183 2023-05-10 12:31:33.233976 pydantic_view-0.2.3/pydantic_view/__init__.py
--rw-r--r--   0        0        0     8425 2023-06-01 22:01:42.960775 pydantic_view-0.2.3/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      876 2023-06-01 22:17:43.001200 pydantic_view-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.949673 pydantic_view-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.636831 pydantic_view-0.2.4/README.md
+-rw-r--r--   0        0        0      183 2023-08-03 13:00:41.628542 pydantic_view-0.2.4/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     9259 2023-08-06 14:58:24.557644 pydantic_view-0.2.4/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      876 2023-08-06 14:58:24.558011 pydantic_view-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.4/PKG-INFO
```

### Comparing `pydantic_view-0.2.3/LICENSE` & `pydantic_view-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.3/README.md` & `pydantic_view-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.3/pydantic_view/pydantic_view.py` & `pydantic_view-0.2.4/pydantic_view/pydantic_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class CustomDict(dict):
     pass
 
 
 def view(
     name: str,
     base: List[str] = None,
+    root: str = None,
     include: Set[str] = None,
     exclude: Set[str] = None,
     optional: Set[str] = None,
     optional_not_none: Set[str] = None,
     fields: Dict[str, Union[Type, FieldInfo, Tuple[Type, FieldInfo]]] = None,
     recursive: bool = None,
     extra: Extra = None,
@@ -103,15 +104,33 @@
                 __validators__[attr_name] = root_validator(
                     *attr._view_root_validator_args,
                     **attr._view_root_validator_kwds,
                 )(attr)
 
         view_cls_name = f"{cls.__name__}{name}"
 
-        __cls_kwargs__ = {}
+        if base is None:
+            metaclass_bases = []
+            for item in set([__base__, *__base__.__bases__]):
+                if issubclass(item, BaseModel):
+                    item = item.__class__
+                if item not in metaclass_bases:
+                    metaclass_bases.append(item)
+
+            class Metaclass(*metaclass_bases):
+                def __subclasscheck__(self, subclass):
+                    if getattr(subclass, "__view_name__", None) == name:
+                        return cls.__subclasscheck__(subclass.__view_root_cls__)
+                    return super().__subclasscheck__(subclass)
+
+            __cls_kwargs__ = {"metaclass": Metaclass}
+
+        else:
+            __cls_kwargs__ = {}
+
         if extra:
             __cls_kwargs__["extra"] = extra
 
         view_cls = create_model(
             view_cls_name,
             __module__=cls.__module__,
             __base__=(__base__,),
@@ -201,15 +220,20 @@
                             ),
                         )
 
                     return getattr(obj.__dict__, f"_{view_cls_name}")
 
                 return view_cls
 
-        setattr(cls, name, ViewDesc())
+        o = cls
+        if root:
+            for item in root.split("."):
+                o = getattr(o, item)
+
+        setattr(o, name, ViewDesc())
 
         if "__pydantic_view_kwds__" not in cls.__dict__:
             setattr(cls, "__pydantic_view_kwds__", {})
 
         cls.__pydantic_view_kwds__[name] = view_kwds
 
         return cls
```

### Comparing `pydantic_view-0.2.3/pyproject.toml` & `pydantic_view-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.2.3"
+version = "0.2.4"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.2.3/PKG-INFO` & `pydantic_view-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.2.3
+Version: 0.2.4
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

