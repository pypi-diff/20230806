# Comparing `tmp/devtools_cli-0.1.2.tar.gz` & `tmp/devtools_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devtools_cli-0.1.2.tar", max compression
+gzip compressed data, was "devtools_cli-0.1.3.tar", max compression
```

## Comparing `devtools_cli-0.1.2.tar` & `devtools_cli-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0       95 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/README.md
--rw-r--r--   0        0        0      294 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/__init__.py
--rw-r--r--   0        0        0      294 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/__init__.py
--rw-r--r--   0        0        0      294 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/info/__init__.py
--rw-r--r--   0        0        0     1724 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/info/main.py
--rw-r--r--   0        0        0      294 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/license/__init__.py
--rw-r--r--   0        0        0     8041 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/license/header.py
--rw-r--r--   0        0        0    11012 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/license/helpers.py
--rw-r--r--   0        0        0     7234 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/license/main.py
--rw-r--r--   0        0        0     2347 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/commands/license/models.py
--rw-r--r--   0        0        0     1007 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/main.py
--rw-r--r--   0        0        0     1810 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/models.py
--rw-r--r--   0        0        0     8089 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/devtools_cli/utils.py
--rw-r--r--   0        0        0     2249 2023-08-05 21:12:09.196237 devtools_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 devtools_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-06 09:10:17.430136 devtools_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0       95 2023-08-06 09:10:17.430136 devtools_cli-0.1.3/README.md
+-rw-r--r--   0        0        0      294 2023-08-06 09:10:17.430136 devtools_cli-0.1.3/devtools_cli/__init__.py
+-rw-r--r--   0        0        0      294 2023-08-06 09:10:17.430136 devtools_cli-0.1.3/devtools_cli/commands/__init__.py
+-rw-r--r--   0        0        0      294 2023-08-06 09:10:17.430136 devtools_cli-0.1.3/devtools_cli/commands/info/__init__.py
+-rw-r--r--   0        0        0     1724 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/commands/info/main.py
+-rw-r--r--   0        0        0      294 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/commands/license/__init__.py
+-rw-r--r--   0        0        0     8027 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/commands/license/header.py
+-rw-r--r--   0        0        0    11012 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/commands/license/helpers.py
+-rw-r--r--   0        0        0     7234 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/commands/license/main.py
+-rw-r--r--   0        0        0     2347 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/commands/license/models.py
+-rw-r--r--   0        0        0     1007 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/main.py
+-rw-r--r--   0        0        0     1810 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/models.py
+-rw-r--r--   0        0        0     8089 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/devtools_cli/utils.py
+-rw-r--r--   0        0        0     2249 2023-08-06 09:10:17.434136 devtools_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 devtools_cli-0.1.3/PKG-INFO
```

### Comparing `devtools_cli-0.1.2/LICENSE` & `devtools_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/commands/info/main.py` & `devtools_cli-0.1.3/devtools_cli/commands/info/main.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/commands/license/header.py` & `devtools_cli-0.1.3/devtools_cli/commands/license/header.py`

 * *Files 8% similar despite different names*

```diff
@@ -217,28 +217,25 @@
 				text=text
 			)
 			self.__headers__.append(data)
 
 	def apply(self, path: Path) -> ApplyResult:
 		"""
 		Applies the previously constructed license header to the file at the specified path.
-		If the file already has a license header, the code first checks if it should skip
-		replacing the existing header if it's identical to the new header, otherwise the old
-		license header will be replaced by the new one. The method is designed to properly
-		handle shebang lines and supports various comment symbols depending on the file suffix.
+		If the file already has a license header which is identical to the one being applied,
+		the method returns 'skipped'. If the file does not have a license header or the new
+		header is different from the old, the function returns 'applied'. If the path is
+		invalid, the method returns 'unsupported'. This method properly handles shebang
+		lines and supports various comment symbols depending on the file suffix.
 
 		Args:
-			path: A file path of type `pathlib.Path` to which the license header should be applied.
-
-		Raises:
-			FileNotFoundError: If the provided path is not a file.
-			NotImplementedError: If the file type is not supported.
+			path: An instance of `pathlib.Path` to which the license header should be applied.
 		"""
-		if not path.is_file():
-			raise FileNotFoundError(f"Cannot apply license header to non-file: {path}")
+		if not path or not path.exists() or not path.is_file():
+			return 'unsupported'
 
 		header: HeaderData | None = None
 		for obj in self.__headers__:
 			if path.suffix in obj.extensions:
 				header = obj
 				break
 
@@ -248,19 +245,21 @@
 		content = path.read_text().splitlines()
 
 		shebang_line = ''
 		if content and content[0].startswith('#!'):
 			shebang_line = content.pop(0) + '\n'
 
 		if content:
-			has_header = content[0].startswith(header.symbols.first)
-			if not has_header and header.symbols.has_alias:
-				header.symbols.use_alias = True
+			has_header = False
+			for _ in range(2 if header.symbols.has_alias else 1):
+				has_header = content[0].startswith(header.symbols.first)
+				if not has_header and header.symbols.has_alias:
+					header.symbols.use_alias = not header.symbols.use_alias
 
-			if content[0].startswith(header.symbols.first):
+			if has_header:
 				end = 0
 				if header.symbols.identical:
 					for i, line in enumerate(content):
 						if line.startswith(header.symbols.first):
 							end += 1
 							continue
 						break
```

### Comparing `devtools_cli-0.1.2/devtools_cli/commands/license/helpers.py` & `devtools_cli-0.1.3/devtools_cli/commands/license/helpers.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/commands/license/main.py` & `devtools_cli-0.1.3/devtools_cli/commands/license/main.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/commands/license/models.py` & `devtools_cli-0.1.3/devtools_cli/commands/license/models.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/main.py` & `devtools_cli-0.1.3/devtools_cli/main.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/models.py` & `devtools_cli-0.1.3/devtools_cli/models.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/devtools_cli/utils.py` & `devtools_cli-0.1.3/devtools_cli/utils.py`

 * *Files identical despite different names*

### Comparing `devtools_cli-0.1.2/pyproject.toml` & `devtools_cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "devtools-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "A toolbox of cross-language utility scripts for efficient software development."
 license = "MIT"
 authors = ["Mattias Aabmets <mattias.aabmets@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/aabmets/devtools-cli"
 keywords = ["toolbox", "cross-language", "utility", "scripts", "software", "development"]
 classifiers = [
```

### Comparing `devtools_cli-0.1.2/PKG-INFO` & `devtools_cli-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devtools-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolbox of cross-language utility scripts for efficient software development.
 Home-page: https://github.com/aabmets/devtools-cli
 License: MIT
 Keywords: toolbox,cross-language,utility,scripts,software,development
 Author: Mattias Aabmets
 Author-email: mattias.aabmets@gmail.com
 Requires-Python: >=3.11,<4.0
```

