# Comparing `tmp/python_configuration-0.9.0.tar.gz` & `tmp/python_configuration-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_configuration-0.9.0.tar", max compression
+gzip compressed data, was "python_configuration-0.9.1.tar", max compression
```

## Comparing `python_configuration-0.9.0.tar` & `python_configuration-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-08-04 23:07:27.752618 python_configuration-0.9.0/LICENSE
--rw-r--r--   0        0        0    10396 2023-08-05 03:31:32.197905 python_configuration-0.9.0/README.md
--rw-r--r--   0        0        0    27447 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/__init__.py
--rw-r--r--   0        0        0    12554 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/configuration.py
--rw-r--r--   0        0        0     7369 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/configuration_set.py
--rw-r--r--   0        0        0       43 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/contrib/__init__.py
--rw-r--r--   0        0        0     4880 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/contrib/aws.py
--rw-r--r--   0        0        0     5257 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/contrib/azure.py
--rw-r--r--   0        0        0     5639 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/contrib/gcp.py
--rw-r--r--   0        0        0     5965 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/helpers.py
--rw-r--r--   0        0        0        0 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/py.typed
--rw-r--r--   0        0        0     1849 2023-08-05 03:31:32.197905 python_configuration-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11610 1970-01-01 00:00:00.000000 python_configuration-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 23:07:27.752618 python_configuration-0.9.1/LICENSE
+-rw-r--r--   0        0        0    12343 2023-08-06 05:49:43.464597 python_configuration-0.9.1/README.md
+-rw-r--r--   0        0        0    30234 2023-08-05 04:05:59.266127 python_configuration-0.9.1/config/__init__.py
+-rw-r--r--   0        0        0    13084 2023-08-06 05:49:43.464597 python_configuration-0.9.1/config/configuration.py
+-rw-r--r--   0        0        0     7369 2023-08-05 03:48:03.453541 python_configuration-0.9.1/config/configuration_set.py
+-rw-r--r--   0        0        0       43 2023-08-04 23:07:27.752618 python_configuration-0.9.1/config/contrib/__init__.py
+-rw-r--r--   0        0        0     4890 2023-08-05 16:16:41.413800 python_configuration-0.9.1/config/contrib/aws.py
+-rw-r--r--   0        0        0     5273 2023-08-05 16:16:41.417134 python_configuration-0.9.1/config/contrib/azure.py
+-rw-r--r--   0        0        0     5655 2023-08-05 16:16:41.417134 python_configuration-0.9.1/config/contrib/gcp.py
+-rw-r--r--   0        0        0     4978 2023-08-05 16:16:41.417134 python_configuration-0.9.1/config/contrib/vault.py
+-rw-r--r--   0        0        0     5965 2023-08-04 23:07:27.752618 python_configuration-0.9.1/config/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-04 23:07:27.752618 python_configuration-0.9.1/config/py.typed
+-rw-r--r--   0        0        0     3278 2023-08-06 05:49:43.464597 python_configuration-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 python_configuration-0.9.1/PKG-INFO
```

### Comparing `python_configuration-0.9.0/LICENSE` & `python_configuration-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_configuration-0.9.0/README.md` & `python_configuration-0.9.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 and optionally
 
 * YAML files
 * TOML files
 * Azure Key Vault credentials
 * AWS Secrets Manager credentials
 * GCP Secret Manager credentials
+* Hashicorp Vault credentials
 
 ## Installing
 
 To install the library:
 
 ```shell
 pip install python-configuration
@@ -272,21 +273,70 @@
 
 When setting the `interpolate` parameter in any `Configuration` instance, the library will perform a string interpolation step using the [str.format](https://docs.python.org/3/library/string.html#formatstrings) syntax.  In particular, this allows to format configuration values automatically:
 
 ```python
 cfg = config_from_dict({
     "percentage": "{val:.3%}",
     "with_sign": "{val:+f}",
-    "val": 1.23456}, interpolate=True)
+    "val": 1.23456,
+    }, interpolate=True)
 
 assert cfg.val == 1.23456
 assert cfg.with_sign == "+1.234560"
 assert cfg.percentage == "123.456%"
 ```
 
+###### Validation
+
+Validation relies on the [jsonchema](https://github.com/python-jsonschema/jsonschema) library, which is automatically installed using the extra `validation`. To use it, call the `validate` method on any `Configuration` instance in a manner similar to what is described on the `jsonschema` library:
+
+```python
+schema = {
+    "type" : "object",
+    "properties" : {
+        "price" : {"type" : "number"},
+        "name" : {"type" : "string"},
+    },
+}
+
+cfg = config_from_dict({"name" : "Eggs", "price" : 34.99})
+assert cfg.validate(schema)
+
+cfg = config_from_dict({"name" : "Eggs", "price" : "Invalid"})
+assert not cfg.validate(schema)
+
+# pass the `raise_on_error` parameter to get the traceback of validation failures
+cfg.validate(schema, raise_on_error=True)
+# ValidationError: 'Invalid' is not of type 'number'
+```
+
+To use the [format](https://python-jsonschema.readthedocs.io/en/latest/validate/#validating-formats) feature of the `jsonschema` library, the extra dependencies must be installed separately as explained in the documentation of `jsonschema`.   
+
+```python
+from jsonschema import Draft202012Validator
+
+schema = {
+    "type" : "object",
+    "properties" : {
+        "ip" : {"format" : "ipv4"},
+    },
+}
+
+cfg = config_from_dict({"ip": "10.0.0.1"})
+assert cfg.validate(schema, format_checker=Draft202012Validator.FORMAT_CHECKER)
+
+cfg = config_from_dict({"ip": "10"})
+assert not cfg.validate(schema, format_checker=Draft202012Validator.FORMAT_CHECKER)
+
+# with the `raise_on_error` parameter:
+c.validate(schema, raise_on_error=True, format_checker=Draft202012Validator.FORMAT_CHECKER)
+# ValidationError: '10' is not a 'ipv4'
+```
+
+
 ## Extras
 
 The `config.contrib` package contains extra implementations of the `Configuration` class used for special cases. Currently the following are implemented:
 
 * `AzureKeyVaultConfiguration` in `config.contrib.azure`, which takes Azure Key Vault
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
@@ -307,14 +357,22 @@
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
 
   ```shell
   pip install python-configuration[gcp]
   ```
 
+* `HashicorpVaultConfiguration` in `config.contrib.vault`, which takes Hashicorp Vault
+  credentials into a `Configuration`-compatible instance. To install the needed dependencies
+  execute
+
+  ```shell
+  pip install python-configuration[vault]
+  ```
+
 ## Features
 
 * Load multiple configuration types
 * Hierarchical configuration
 * Ability to override with environment variables
 * Merge parameters from different configuration types
```

### Comparing `python_configuration-0.9.0/config/__init__.py` & `python_configuration-0.9.1/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -96,55 +96,67 @@
         elif type_ in ("env", "environment"):
             params = list(config_[1:]) + default_args[(len(config_) - 1) :]
             instances.append(config_from_env(*params, **default_kwargs))
         elif type_ == "python":
             if len(config_) < 2:
                 raise ValueError("No path specified for python module")
             params = list(config_[1:]) + default_args[(len(config_) - 2) :]
-            try:
-                instances.append(config_from_python(*params, **default_kwargs))
-            except (FileNotFoundError, ModuleNotFoundError):
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_python(
+                    *params, **default_kwargs, ignore_missing_paths=ignore_missing_paths
+                )
+            )
         elif type_ == "json":
-            try:
-                instances.append(config_from_json(*config_[1:], **default_kwargs))
-            except FileNotFoundError:
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_json(
+                    *config_[1:],
+                    **default_kwargs,
+                    ignore_missing_paths=ignore_missing_paths,
+                )
+            )
         elif yaml and type_ == "yaml":
-            try:
-                instances.append(config_from_yaml(*config_[1:], **default_kwargs))
-            except FileNotFoundError:
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_yaml(
+                    *config_[1:],
+                    **default_kwargs,
+                    ignore_missing_paths=ignore_missing_paths,
+                )
+            )
         elif toml and type_ == "toml":
-            try:
-                instances.append(config_from_toml(*config_[1:], **default_kwargs))
-            except FileNotFoundError:
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_toml(
+                    *config_[1:],
+                    **default_kwargs,
+                    ignore_missing_paths=ignore_missing_paths,
+                )
+            )
         elif type_ == "ini":
-            try:
-                instances.append(config_from_ini(*config_[1:], **default_kwargs))
-            except FileNotFoundError:
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_ini(
+                    *config_[1:],
+                    **default_kwargs,
+                    ignore_missing_paths=ignore_missing_paths,
+                )
+            )
         elif type_ == "dotenv":
-            try:
-                instances.append(config_from_dotenv(*config_[1:], **default_kwargs))
-            except FileNotFoundError:
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_dotenv(
+                    *config_[1:],
+                    **default_kwargs,
+                    ignore_missing_paths=ignore_missing_paths,
+                )
+            )
         elif type_ == "path":
-            try:
-                instances.append(config_from_path(*config_[1:], **default_kwargs))
-            except FileNotFoundError:
-                if not ignore_missing_paths:
-                    raise
+            instances.append(
+                config_from_path(
+                    *config_[1:],
+                    **default_kwargs,
+                    ignore_missing_paths=ignore_missing_paths,
+                )
+            )
         else:
             raise ValueError(f'Unknown configuration type "{type_}"')
 
     return ConfigurationSet(
         *instances, interpolate=interpolate, interpolate_type=interpolate_type
     )
 
@@ -228,14 +240,15 @@
         self,
         path: str,
         remove_level: int = 1,
         *,
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ):
         """
         Constructor.
 
         :param path: path to read from
         :param remove_level: how many levels to remove from the resulting config
         :param lowercase_keys: whether to convert every key to lower case.
@@ -244,39 +257,47 @@
         self._remove_level = remove_level
         super().__init__(
             {},
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
         )
+        self._ignore_missing_paths = ignore_missing_paths
         self.reload()
 
     def reload(self) -> None:
         """Reload the path."""
-        path = os.path.normpath(self._path)
-        if not os.path.exists(path) or not os.path.isdir(path):
-            raise FileNotFoundError()
-
-        dotted_path_levels = len(path.split("/"))
-        files_keys = (
-            (
-                os.path.join(x[0], y),
-                ".".join(
-                    (x[0].split("/") + [y])[(dotted_path_levels + self._remove_level) :]
-                ),
+        try:
+            path = os.path.normpath(self._path)
+            if not os.path.exists(path) or not os.path.isdir(path):
+                raise FileNotFoundError()
+
+            dotted_path_levels = len(path.split("/"))
+            files_keys = (
+                (
+                    os.path.join(x[0], y),
+                    ".".join(
+                        (x[0].split("/") + [y])[
+                            (dotted_path_levels + self._remove_level) :
+                        ]
+                    ),
+                )
+                for x in os.walk(path)
+                for y in x[2]
+                if not x[0].split("/")[-1].startswith("..")
             )
-            for x in os.walk(path)
-            for y in x[2]
-            if not x[0].split("/")[-1].startswith("..")
-        )
-
-        result = {}
-        for filename, key in files_keys:
-            result[key] = open(filename).read()
 
+            result = {}
+            for filename, key in files_keys:
+                result[key] = open(filename).read()
+        except FileNotFoundError:
+            if self._ignore_missing_paths:
+                result = {}
+            else:
+                raise
         super().__init__(
             result,
             lowercase_keys=self._lowercase,
             interpolate=self._interpolate,
             interpolate_type=self._interpolate_type,
         )
 
@@ -284,14 +305,15 @@
 def config_from_path(
     path: str,
     remove_level: int = 1,
     *,
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ignore_missing_paths: bool = False,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from filesystem path.
 
     :param path: path to read from
     :param remove_level: how many levels to remove from the resulting config
     :param lowercase_keys: whether to convert every key to lower case.
@@ -300,28 +322,30 @@
     """
     return PathConfiguration(
         path,
         remove_level,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
+        ignore_missing_paths=ignore_missing_paths,
     )
 
 
 class FileConfiguration(Configuration):
     """Configuration from a file input."""
 
     def __init__(
         self,
         data: Union[str, TextIO],
         read_from_file: bool = False,
         *,
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ):
         """
         Constructor.
 
         :param data: path to a config file, or its contents
         :param read_from_file: whether to read from a file path or to interpret
                the :attr:`data` as the contents of the file.
@@ -329,32 +353,51 @@
         """
         super().__init__(
             {},
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
         )
-        self._reload(data, read_from_file)
-        self._data = data if read_from_file and isinstance(data, str) else None
+        self._filename = data if read_from_file and isinstance(data, str) else None
+        self._ignore_missing_paths = ignore_missing_paths
+        self._reload_with_check(data, read_from_file)
+
+    def _reload_with_check(
+        self,
+        data: Union[str, TextIO],
+        read_from_file: bool = False,
+    ) -> None:  # pragma: no cover
+        try:
+            self._reload(data, read_from_file)
+        except FileNotFoundError:
+            if not self._ignore_missing_paths:
+                raise
+            self._config = self._flatten_dict({})
 
     def _reload(
-        self, data: Union[str, TextIO], read_from_file: bool = False
+        self,
+        data: Union[str, TextIO],
+        read_from_file: bool = False,
     ) -> None:  # pragma: no cover
         raise NotImplementedError()
 
     def reload(self) -> None:
         """Reload the configuration."""
-        if self._data:  # pragma: no branch
-            self._reload(self._data, True)
+        if self._filename:  # pragma: no branch
+            self._reload_with_check(self._filename, True)
 
 
 class JSONConfiguration(FileConfiguration):
     """Configuration from a JSON input."""
 
-    def _reload(self, data: Union[str, TextIO], read_from_file: bool = False) -> None:
+    def _reload(
+        self,
+        data: Union[str, TextIO],
+        read_from_file: bool = False,
+    ) -> None:
         """Reload the JSON data."""
         if read_from_file:
             if isinstance(data, str):
                 result = json.load(open(data, "rt"))
             else:
                 result = json.load(data)
         else:
@@ -365,31 +408,34 @@
 def config_from_json(
     data: Union[str, TextIO],
     read_from_file: bool = False,
     *,
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ignore_missing_paths: bool = False,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from a JSON file.
 
     :param data: path to a JSON file or contents
     :param read_from_file: whether to read from a file path or to interpret
            the :attr:`data` as the contents of the JSON file.
     :param lowercase_keys: whether to convert every key to lower case.
     :param interpolate: whether to apply string interpolation when looking for items
+    :param ignore_missing_paths: if true it will not throw on missing paths
     :return: a :class:`Configuration` instance
     """
     return JSONConfiguration(
         data,
         read_from_file,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
+        ignore_missing_paths=ignore_missing_paths,
     )
 
 
 class INIConfiguration(FileConfiguration):
     """Configuration from an INI file input."""
 
     def __init__(
@@ -397,22 +443,24 @@
         data: Union[str, TextIO],
         read_from_file: bool = False,
         *,
         section_prefix: str = "",
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ):
         self._section_prefix = section_prefix
         super().__init__(
             data=data,
             read_from_file=read_from_file,
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
+            ignore_missing_paths=ignore_missing_paths,
         )
 
     def _reload(self, data: Union[str, TextIO], read_from_file: bool = False) -> None:
         """Reload the INI data."""
         import configparser
 
         lowercase = self._lowercase
@@ -442,32 +490,35 @@
     data: Union[str, TextIO],
     read_from_file: bool = False,
     *,
     section_prefix: str = "",
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ignore_missing_paths: bool = False,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from an INI file.
 
     :param data: path to an INI file or contents
     :param read_from_file: whether to read from a file path or to interpret
            the :attr:`data` as the contents of the INI file.
     :param lowercase_keys: whether to convert every key to lower case.
     :param interpolate: whether to apply string interpolation when looking for items
+    :param ignore_missing_paths: if true it will not throw on missing paths
     :return: a :class:`Configuration` instance
     """
     return INIConfiguration(
         data,
         read_from_file,
         section_prefix=section_prefix,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
+        ignore_missing_paths=ignore_missing_paths,
     )
 
 
 class DotEnvConfiguration(FileConfiguration):
     """Configuration from a .env type file input."""
 
     def __init__(
@@ -476,23 +527,25 @@
         read_from_file: bool = False,
         prefix: str = "",
         separator: str = "__",
         *,
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ):
         self._prefix = prefix
         self._separator = separator
         super().__init__(
             data=data,
             read_from_file=read_from_file,
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
+            ignore_missing_paths=ignore_missing_paths,
         )
 
     def _reload(
         self,
         data: Union[str, TextIO],
         read_from_file: bool = False,
     ) -> None:
@@ -525,33 +578,36 @@
     read_from_file: bool = False,
     prefix: str = "",
     separator: str = "__",
     *,
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ignore_missing_paths: bool = False,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from a .env type file.
 
     :param data: path to a .env type file or contents
     :param read_from_file: whether to read from a file path or to interpret
            the :attr:`data` as the contents of the INI file.
     :param lowercase_keys: whether to convert every key to lower case.
     :param interpolate: whether to apply string interpolation when looking for items
+    :param ignore_missing_paths: if true it will not throw on missing paths
     :return: a :class:`Configuration` instance
     """
     return DotEnvConfiguration(
         data,
         read_from_file,
         prefix=prefix,
         separator=separator,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
+        ignore_missing_paths=ignore_missing_paths,
     )
 
 
 class PythonConfiguration(Configuration):
     """Configuration from a python module."""
 
     def __init__(
@@ -559,63 +615,73 @@
         module: Union[str, ModuleType],
         prefix: str = "",
         separator: str = "_",
         *,
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ):
         """
         Constructor.
 
         :param module: a module or path string
         :param prefix: prefix to use to filter object names
         :param separator: separator to replace by dots
         :param lowercase_keys: whether to convert every key to lower case.
         """
-        if isinstance(module, str):
-            if module.endswith(".py"):
-                import importlib.util
-                from importlib import machinery
-
-                spec = cast(
-                    machinery.ModuleSpec,
-                    importlib.util.spec_from_file_location(module, module),
-                )
-                module = importlib.util.module_from_spec(spec)
-                spec.loader = cast(InspectLoader, spec.loader)
-                spec.loader.exec_module(module)
-            else:
-                import importlib
+        try:
+            if isinstance(module, str):
+                if module.endswith(".py"):
+                    import importlib.util
+                    from importlib import machinery
+
+                    spec = cast(
+                        machinery.ModuleSpec,
+                        importlib.util.spec_from_file_location(module, module),
+                    )
+                    module = importlib.util.module_from_spec(spec)
+                    spec.loader = cast(InspectLoader, spec.loader)
+                    spec.loader.exec_module(module)
+                else:
+                    import importlib
+
+                    module = importlib.import_module(module)
+            self._module: Optional[ModuleType] = module
+            self._prefix = prefix
+            self._separator = separator
+        except (FileNotFoundError, ModuleNotFoundError):
+            if not ignore_missing_paths:
+                raise
+            self._module = None
 
-                module = importlib.import_module(module)
-        self._module = module
-        self._prefix = prefix
-        self._separator = separator
         super().__init__(
             {},
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
         )
         self.reload()
 
     def reload(self) -> None:
         """Reload the path."""
-        variables = [
-            x
-            for x in dir(self._module)
-            if not x.startswith("__") and x.startswith(self._prefix)
-        ]
-        result = {
-            k[len(self._prefix) :]
-            .replace(self._separator, ".")
-            .strip("."): getattr(self._module, k)
-            for k in variables
-        }
+        if self._module is not None:
+            variables = [
+                x
+                for x in dir(self._module)
+                if not x.startswith("__") and x.startswith(self._prefix)
+            ]
+            result = {
+                k[len(self._prefix) :]
+                .replace(self._separator, ".")
+                .strip("."): getattr(self._module, k)
+                for k in variables
+            }
+        else:
+            result = {}
         super().__init__(
             result,
             lowercase_keys=self._lowercase,
             interpolate=self._interpolate,
             interpolate_type=self._interpolate_type,
         )
 
@@ -624,14 +690,15 @@
     module: Union[str, ModuleType],
     prefix: str = "",
     separator: str = "_",
     *,
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ignore_missing_paths: bool = False,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from the objects in a Python module.
 
     :param module: a module or path string
     :param prefix: prefix to use to filter object names
     :param separator: separator to replace by dots
@@ -642,14 +709,15 @@
     return PythonConfiguration(
         module,
         prefix,
         separator,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
+        ignore_missing_paths=ignore_missing_paths,
     )
 
 
 def config_from_dict(
     data: Mapping,
     *,
     lowercase_keys: bool = False,
@@ -715,30 +783,33 @@
     def config_from_yaml(
         data: Union[str, TextIO],
         read_from_file: bool = False,
         *,
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ) -> Configuration:
         """
         Return a Configuration instance from YAML files.
 
         :param data: string or file
         :param read_from_file: whether `data` is a file or a YAML formatted string
         :param lowercase_keys: whether to convert every key to lower case.
         :param interpolate: whether to apply string interpolation when looking for items
+        :param ignore_missing_paths: if true it will not throw on missing paths
         :return: a Configuration instance
         """
         return YAMLConfiguration(
             data,
             read_from_file,
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
+            ignore_missing_paths=ignore_missing_paths,
         )
 
 
 if toml is not None:  # pragma: no branch
 
     class TOMLConfiguration(FileConfiguration):
         """Configuration from a TOML input."""
@@ -748,22 +819,24 @@
             data: Union[str, TextIO],
             read_from_file: bool = False,
             *,
             section_prefix: str = "",
             lowercase_keys: bool = False,
             interpolate: InterpolateType = False,
             interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+            ignore_missing_paths: bool = False,
         ):
             self._section_prefix = section_prefix
             super().__init__(
                 data=data,
                 read_from_file=read_from_file,
                 lowercase_keys=lowercase_keys,
                 interpolate=interpolate,
                 interpolate_type=interpolate_type,
+                ignore_missing_paths=ignore_missing_paths,
             )
 
         def _reload(
             self, data: Union[str, TextIO], read_from_file: bool = False
         ) -> None:
             """Reload the TOML data."""
             if read_from_file:
@@ -788,25 +861,28 @@
         data: Union[str, TextIO],
         read_from_file: bool = False,
         *,
         section_prefix: str = "",
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ignore_missing_paths: bool = False,
     ) -> Configuration:
         """
         Return a Configuration instance from TOML files.
 
         :param data: string or file
         :param read_from_file: whether `data` is a file or a TOML formatted string
         :param lowercase_keys: whether to convert every key to lower case.
         :param interpolate: whether to apply string interpolation when looking for items
+        :param ignore_missing_paths: if true it will not throw on missing paths
         :return: a Configuration instance
         """
         return TOMLConfiguration(
             data,
             read_from_file,
             section_prefix=section_prefix,
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
+            ignore_missing_paths=ignore_missing_paths,
         )
```

### Comparing `python_configuration-0.9.0/config/configuration.py` & `python_configuration-0.9.1/config/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -387,14 +387,29 @@
         Reload the configuration.
 
         This method is not implemented for simple Configuration objects and is
         intended only to be used in subclasses.
         """
         raise NotImplementedError()
 
+    def validate(
+        self, schema: Any, raise_on_error: bool = False, **kwargs: Mapping[str, Any]
+    ) -> bool:
+        try:
+            from jsonschema import validate, ValidationError
+        except ImportError:  # pragma: no cover
+            raise RuntimeError("Validation requires the `jsonschema` library.")
+        try:
+            validate(self.as_dict(), schema, **kwargs)
+        except ValidationError as err:
+            if raise_on_error:
+                raise err
+            return False
+        return True
+
     @contextmanager
     def dotted_iter(self) -> Iterator["Configuration"]:
         """
         Context manager for dotted iteration.
 
         This context manager changes all the iterator-related functions
         to include every nested (dotted) key instead of just the top level.
```

### Comparing `python_configuration-0.9.0/config/configuration_set.py` & `python_configuration-0.9.1/config/configuration_set.py`

 * *Files identical despite different names*

### Comparing `python_configuration-0.9.0/config/contrib/aws.py` & `python_configuration-0.9.1/config/contrib/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Configuration from AWS Secrets Manager."""
+"""Configuration instances from AWS Secrets Manager."""
 
 import json
 import time
 from typing import Any, Dict, Optional
 
 import boto3
```

### Comparing `python_configuration-0.9.0/config/contrib/azure.py` & `python_configuration-0.9.1/config/contrib/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Configuration from Azure KeyVaults."""
+"""Configuration instances from Azure KeyVaults."""
 
 import time
 from typing import Any, Dict, ItemsView, KeysView, Optional, Union, ValuesView, cast
 
 from azure.core.exceptions import ResourceNotFoundError
 from azure.identity import ClientSecretCredential
 from azure.keyvault.secrets import SecretClient
@@ -84,15 +84,15 @@
             raise KeyError(item)
         else:
             return secret
 
     def __getattr__(self, item: str) -> Any:  # noqa: D105
         secret = self._get_secret(item)
         if secret is None:
-            raise KeyError(item)
+            raise AttributeError(item)
         else:
             return secret
 
     def get(self, key: str, default: Any = None) -> Union[dict, Any]:
         """
         Get the configuration values corresponding to :attr:`key`.
```

### Comparing `python_configuration-0.9.0/config/contrib/gcp.py` & `python_configuration-0.9.1/config/contrib/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Configuration from GCP Secret Manager."""
+"""Configuration instances from GCP Secret Manager."""
 
 import time
 from typing import Any, Dict, ItemsView, KeysView, Optional, Union, ValuesView, cast
 
 from google.api_core.client_options import ClientOptions
 from google.api_core.exceptions import NotFound
 from google.auth.credentials import Credentials
@@ -85,15 +85,15 @@
             raise KeyError(item)
         else:
             return secret
 
     def __getattr__(self, item: str) -> Any:  # noqa: D105
         secret = self._get_secret(item)
         if secret is None:
-            raise KeyError(item)
+            raise AttributeError(item)
         else:
             return secret
 
     def get(self, key: str, default: Any = None) -> Union[dict, Any]:
         """
         Get the configuration values corresponding to :attr:`key`.
```

### Comparing `python_configuration-0.9.0/config/helpers.py` & `python_configuration-0.9.1/config/helpers.py`

 * *Files identical despite different names*

### Comparing `python_configuration-0.9.0/PKG-INFO` & `python_configuration-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-configuration
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library to load configuration parameters from multiple sources and formats
 Home-page: https://github.com/tr11/python-configuration
 License: MIT
 Keywords: configuration,settings,json,yaml,toml,ini
 Author: Tiago Requeijo
 Author-email: tiago.requeijo.dev@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -13,19 +13,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: gcp
 Provides-Extra: toml
+Provides-Extra: validation
+Provides-Extra: vault
 Provides-Extra: yaml
 Requires-Dist: azure-identity (>=1.13.0,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0) ; extra == "azure"
 Requires-Dist: boto3 (>=1.28.20,<2.0.0) ; extra == "aws"
 Requires-Dist: google-cloud-secret-manager (>=2.16.3,<3.0.0) ; extra == "gcp"
+Requires-Dist: hvac (>=1.1.1,<2.0.0) ; extra == "vault"
+Requires-Dist: jsonschema (>=4.18.6,<5.0.0) ; extra == "validation"
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
 Requires-Dist: toml (>=0.10.0,<0.11.0) ; extra == "toml"
 Project-URL: Repository, https://github.com/tr11/python-configuration
 Description-Content-Type: text/markdown
 
 # python-configuration
 > A library to load configuration parameters hierarchically from multiple sources and formats
@@ -51,14 +55,15 @@
 and optionally
 
 * YAML files
 * TOML files
 * Azure Key Vault credentials
 * AWS Secrets Manager credentials
 * GCP Secret Manager credentials
+* Hashicorp Vault credentials
 
 ## Installing
 
 To install the library:
 
 ```shell
 pip install python-configuration
@@ -301,21 +306,70 @@
 
 When setting the `interpolate` parameter in any `Configuration` instance, the library will perform a string interpolation step using the [str.format](https://docs.python.org/3/library/string.html#formatstrings) syntax.  In particular, this allows to format configuration values automatically:
 
 ```python
 cfg = config_from_dict({
     "percentage": "{val:.3%}",
     "with_sign": "{val:+f}",
-    "val": 1.23456}, interpolate=True)
+    "val": 1.23456,
+    }, interpolate=True)
 
 assert cfg.val == 1.23456
 assert cfg.with_sign == "+1.234560"
 assert cfg.percentage == "123.456%"
 ```
 
+###### Validation
+
+Validation relies on the [jsonchema](https://github.com/python-jsonschema/jsonschema) library, which is automatically installed using the extra `validation`. To use it, call the `validate` method on any `Configuration` instance in a manner similar to what is described on the `jsonschema` library:
+
+```python
+schema = {
+    "type" : "object",
+    "properties" : {
+        "price" : {"type" : "number"},
+        "name" : {"type" : "string"},
+    },
+}
+
+cfg = config_from_dict({"name" : "Eggs", "price" : 34.99})
+assert cfg.validate(schema)
+
+cfg = config_from_dict({"name" : "Eggs", "price" : "Invalid"})
+assert not cfg.validate(schema)
+
+# pass the `raise_on_error` parameter to get the traceback of validation failures
+cfg.validate(schema, raise_on_error=True)
+# ValidationError: 'Invalid' is not of type 'number'
+```
+
+To use the [format](https://python-jsonschema.readthedocs.io/en/latest/validate/#validating-formats) feature of the `jsonschema` library, the extra dependencies must be installed separately as explained in the documentation of `jsonschema`.   
+
+```python
+from jsonschema import Draft202012Validator
+
+schema = {
+    "type" : "object",
+    "properties" : {
+        "ip" : {"format" : "ipv4"},
+    },
+}
+
+cfg = config_from_dict({"ip": "10.0.0.1"})
+assert cfg.validate(schema, format_checker=Draft202012Validator.FORMAT_CHECKER)
+
+cfg = config_from_dict({"ip": "10"})
+assert not cfg.validate(schema, format_checker=Draft202012Validator.FORMAT_CHECKER)
+
+# with the `raise_on_error` parameter:
+c.validate(schema, raise_on_error=True, format_checker=Draft202012Validator.FORMAT_CHECKER)
+# ValidationError: '10' is not a 'ipv4'
+```
+
+
 ## Extras
 
 The `config.contrib` package contains extra implementations of the `Configuration` class used for special cases. Currently the following are implemented:
 
 * `AzureKeyVaultConfiguration` in `config.contrib.azure`, which takes Azure Key Vault
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
@@ -336,14 +390,22 @@
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
 
   ```shell
   pip install python-configuration[gcp]
   ```
 
+* `HashicorpVaultConfiguration` in `config.contrib.vault`, which takes Hashicorp Vault
+  credentials into a `Configuration`-compatible instance. To install the needed dependencies
+  execute
+
+  ```shell
+  pip install python-configuration[vault]
+  ```
+
 ## Features
 
 * Load multiple configuration types
 * Hierarchical configuration
 * Ability to override with environment variables
 * Merge parameters from different configuration types
```

