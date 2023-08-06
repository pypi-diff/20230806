# Comparing `tmp/pyobf2-1.3.0.tar.gz` & `tmp/pyobf2-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobf2-1.3.0.tar", max compression
+gzip compressed data, was "pyobf2-1.3.1.tar", max compression
```

## Comparing `pyobf2-1.3.0.tar` & `pyobf2-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1493 2023-05-29 20:30:26.316026 pyobf2-1.3.0/LICENSE
--rw-r--r--   0        0        0    20749 2023-06-03 17:45:28.408096 pyobf2-1.3.0/README.md
--rw-r--r--   0        0        0    12871 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/__init__.py
--rw-r--r--   0        0        0       67 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/__main__.py
--rw-r--r--   0        0        0     5344 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/__init__.py
--rw-r--r--   0        0        0     8438 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/assembler.py
--rw-r--r--   0        0        0      318 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/cfg.py
--rw-r--r--   0        0        0      543 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/log.py
--rw-r--r--   0        0        0    15769 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/renamer.py
--rw-r--r--   0        0        0     2769 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/__init__.py
--rw-r--r--   0        0        0     5454 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/collector.py
--rw-r--r--   0        0        0     2466 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/compileFinalFiles.py
--rw-r--r--   0        0        0     7414 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py
--rw-r--r--   0        0        0     7919 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/encodeStringsTransformer.py
--rw-r--r--   0        0        0     1732 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/floatsToComplex.py
--rw-r--r--   0        0        0     1690 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/fstrToFormatTransformer.py
--rw-r--r--   0        0        0     6416 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/intObfuscatorTransformer.py
--rw-r--r--   0        0        0     1939 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/logicTransformer.py
--rw-r--r--   0        0        0     2335 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/memberRenamerTransformer.py
--rw-r--r--   0        0        0     4944 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/packPyz.py
--rw-r--r--   0        0        0      872 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/removeTypeHintsTransformer.py
--rw-r--r--   0        0        0      876 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/replaceAttribsTransformer.py
--rw-r--r--   0        0        0     3303 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/stringCollectorTransformer.py
--rw-r--r--   0        0        0     2674 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/typeAliasTransformer.py
--rw-r--r--   0        0        0     1215 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/transformers/unicodeNameTransformer.py
--rw-r--r--   0        0        0     8990 2023-05-29 20:30:26.320026 pyobf2-1.3.0/pyobf2/lib/util.py
--rw-r--r--   0        0        0      583 2023-06-03 18:52:45.803711 pyobf2-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    21443 1970-01-01 00:00:00.000000 pyobf2-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1493 2023-05-29 20:30:26.316026 pyobf2-1.3.1/LICENSE
+-rw-r--r--   0        0        0    20749 2023-06-03 17:45:28.408096 pyobf2-1.3.1/README.md
+-rw-r--r--   0        0        0    12871 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/__main__.py
+-rw-r--r--   0        0        0     5344 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/__init__.py
+-rw-r--r--   0        0        0     8438 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/assembler.py
+-rw-r--r--   0        0        0      318 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/cfg.py
+-rw-r--r--   0        0        0      543 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/log.py
+-rw-r--r--   0        0        0    16693 2023-08-06 18:35:04.573642 pyobf2-1.3.1/pyobf2/lib/renamer.py
+-rw-r--r--   0        0        0     2766 2023-08-06 18:24:32.684765 pyobf2-1.3.1/pyobf2/lib/transformers/__init__.py
+-rw-r--r--   0        0        0     5454 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/collector.py
+-rw-r--r--   0        0        0     2466 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/compileFinalFiles.py
+-rw-r--r--   0        0        0     7414 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py
+-rw-r--r--   0        0        0     7919 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/encodeStringsTransformer.py
+-rw-r--r--   0        0        0     1732 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/floatsToComplex.py
+-rw-r--r--   0        0        0     1690 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/fstrToFormatTransformer.py
+-rw-r--r--   0        0        0     6416 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/intObfuscatorTransformer.py
+-rw-r--r--   0        0        0     1939 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/logicTransformer.py
+-rw-r--r--   0        0        0     2332 2023-08-06 18:24:32.668764 pyobf2-1.3.1/pyobf2/lib/transformers/memberRenamerTransformer.py
+-rw-r--r--   0        0        0     4944 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/packPyz.py
+-rw-r--r--   0        0        0      872 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/removeTypeHintsTransformer.py
+-rw-r--r--   0        0        0      876 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/replaceAttribsTransformer.py
+-rw-r--r--   0        0        0     3303 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/stringCollectorTransformer.py
+-rw-r--r--   0        0        0     2674 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/typeAliasTransformer.py
+-rw-r--r--   0        0        0     1215 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/transformers/unicodeNameTransformer.py
+-rw-r--r--   0        0        0     8990 2023-05-29 20:30:26.320026 pyobf2-1.3.1/pyobf2/lib/util.py
+-rw-r--r--   0        0        0      583 2023-08-06 18:36:20.686877 pyobf2-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    21443 1970-01-01 00:00:00.000000 pyobf2-1.3.1/PKG-INFO
```

### Comparing `pyobf2-1.3.0/LICENSE` & `pyobf2-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/README.md` & `pyobf2-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/__init__.py` & `pyobf2-1.3.1/pyobf2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/__init__.py` & `pyobf2-1.3.1/pyobf2/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/assembler.py` & `pyobf2-1.3.1/pyobf2/lib/assembler.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/log.py` & `pyobf2-1.3.1/pyobf2/lib/log.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/renamer.py` & `pyobf2-1.3.1/pyobf2/lib/renamer.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,18 +62,33 @@
             },
         )
         if type(generated_name) != str:
             generated_name = str(generated_name)
         return generated_name
 
     def __init__(self, fmt):
+        self.skip_args = False
         self.fmt = fmt
         self.counters = {}
         self.mappings = {}
         self.location_stack = []
+        self.tabu_method_arguments = []
+
+    def go(self, s: AST):
+        for node in walk(s):
+            if isinstance(node, Call) and isinstance(node.func, Name):
+                has_tabu_arg = len(node.keywords) > 0 and any(map(lambda p: p.arg is None, node.keywords))
+                if has_tabu_arg:
+                    # suboptimal condition:
+                    # the user called the method with `method(**args)`. this is dogshit because args is a map we don't
+                    #   know the contents of.
+                    # since the keys of the map could be fucking anything, we can't reliably change them.
+                    # equally suboptimal fix: just don't remap that specific method's parameters :/
+                    self.tabu_method_arguments.append(node.func.id)
+        self.visit(s)
 
     def visit_Global(self, node: Global) -> Any:
         for i in range(len(node.names)):
             x = node.names[i]
             remapped_name = self.remap_name_if_needed(x)
             if remapped_name is not x:  # we have a mapping for this one? good
                 self.put_name_if_absent(x, remapped_name)
@@ -132,30 +147,40 @@
 
     def visit_FunctionDef(self, node: FunctionDef) -> Any:
         name = node.name
         # methods need to be enabled and none of the location elements need to be of a class
         if not any(x.startswith("cl_") for x in self.location_stack):
             self.put_name_if_absent(name, self.mapping_name("method"))
         self.start_visit("mt_" + name)
-        self.generic_visit(node)
-        self.end_visit()
+        if name in self.tabu_method_arguments:
+            before = self.skip_args
+            self.skip_args = True
+            self.generic_visit(node)
+            self.end_visit()
+            self.skip_args = before
+        else:
+            self.generic_visit(node)
+            self.end_visit()
 
     def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
         name = node.name
         self.put_name_if_absent(name, self.mapping_name("method"))
         self.start_visit("mt_" + name)
         self.generic_visit(node)
         self.end_visit()
 
     def visit_arg(self, node: arg) -> Any:
         name = node.arg
-        nn = self.mapping_name("arg")
-        self.put_name_if_absent(name, nn)
+        nn = None
+        if not self.skip_args:
+            nn = self.mapping_name("arg")
+            self.put_name_if_absent(name, nn)
         old_stack = self.end_visit()
-        self.put_name_if_absent(old_stack + "_arg_" + name, nn)
+        if not self.skip_args:
+            self.put_name_if_absent(old_stack + "_arg_" + name, nn)
         self.start_visit(old_stack)
 
     def visit_Lambda(self, node: Lambda) -> Any:
         self.start_visit("mt_<lambda>")
         self.generic_visit(node)
         self.end_visit()
 
@@ -396,25 +421,20 @@
         self.start_visit("cl_" + node.name)
         node.name = self.remap_name_if_needed(node.name)
         self.generic_visit(node)
         self.end_visit()
 
     def visit_Call(self, node: Call) -> Any:
         if isinstance(node.func, Name):
-            # self.start_visit("mt_" + node.func.id)
-            # print(self.location_stack)
-            # prev = self.end_visit() if len(self.location_stack) > 0 else None
             for k in node.keywords:
+                if k.arg is None:
+                    continue  # isn't mapped anyway
                 search_str = "mt_" + node.func.id + "_arg_" + k.arg
-                # print(self.location_stack, search_str)
                 res = self.remap_name_if_needed(search_str)
                 if res == search_str:
                     res = k.arg
                 k.arg = res
-            # if prev is not None:
-            #     self.start_visit(prev)
-            # self.end_visit()
         self.generic_visit(node)
 
     def visit_Name(self, node: Name) -> Any:
         node.id = self.remap_name_if_needed(node.id)
         self.generic_visit(node)
```

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/__init__.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         else:
             raise ValueError("Non-constant format specs are not supported")
     return s
 
 
 def optimize_ast(ast1: AST):
     generator = MappingGenerator('f"{kind[0]}{get_counter(kind)}"')
-    generator.visit(ast1)
+    generator.go(ast1)
     MappingApplicator(generator.mappings).visit(ast1)
     for x in ast.walk(ast1):
         if isinstance(x, (AsyncFunctionDef, FunctionDef, ClassDef, Module)):
             clear_docstring(x)
     return ast1
```

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/collector.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/collector.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/compileFinalFiles.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/compileFinalFiles.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/constructDynamicCodeObjTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/encodeStringsTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/encodeStringsTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/floatsToComplex.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/floatsToComplex.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/fstrToFormatTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/fstrToFormatTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/intObfuscatorTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/intObfuscatorTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/logicTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/logicTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/memberRenamerTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/memberRenamerTransformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 "https://docs.python.org/3/reference/lexical_analysis.html#identifiers",
                 "f'{kind}{get_counter(kind)}'",
             ),
         )
 
     def transform(self, ast: AST, current_file_name, all_asts, all_file_names) -> AST:
         generator = MappingGenerator(self.config["rename_format"].value)
-        generator.visit(ast)
+        generator.go(ast)
         # generator.print_mappings()
         MappingApplicator(generator.mappings).visit(ast)
         if all_asts is not None:
             mappings1 = {}
             this_file_name = os.path.abspath(current_file_name)
             for x in generator.mappings.keys():
                 n = x.split(".")
```

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/packPyz.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/packPyz.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/removeTypeHintsTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/removeTypeHintsTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/replaceAttribsTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/replaceAttribsTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/stringCollectorTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/stringCollectorTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/typeAliasTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/typeAliasTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/transformers/unicodeNameTransformer.py` & `pyobf2-1.3.1/pyobf2/lib/transformers/unicodeNameTransformer.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyobf2/lib/util.py` & `pyobf2-1.3.1/pyobf2/lib/util.py`

 * *Files identical despite different names*

### Comparing `pyobf2-1.3.0/pyproject.toml` & `pyobf2-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobf2"
-version = "1.3.0"
+version = "1.3.1"
 description = "An in-place obfuscator for python 3.11"
 authors = ["0x150 <99053360+0x3C50@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/0x3C50/pyobf2"
 repository = "https://github.com/0x3C50/pyobf2"
 keywords = ["obfuscator", "obfuscator-api"]
```

### Comparing `pyobf2-1.3.0/PKG-INFO` & `pyobf2-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobf2
-Version: 1.3.0
+Version: 1.3.1
 Summary: An in-place obfuscator for python 3.11
 Home-page: https://github.com/0x3C50/pyobf2
 Keywords: obfuscator,obfuscator-api
 Author: 0x150
 Author-email: 99053360+0x3C50@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

