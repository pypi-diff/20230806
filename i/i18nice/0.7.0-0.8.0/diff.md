# Comparing `tmp/i18nice-0.7.0.tar.gz` & `tmp/i18nice-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i18nice-0.7.0.tar", last modified: Sun Jul 30 20:35:59 2023, max compression
+gzip compressed data, was "i18nice-0.8.0.tar", last modified: Sun Aug  6 18:07:04 2023, max compression
```

## Comparing `i18nice-0.7.0.tar` & `i18nice-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.126722 i18nice-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-30 20:35:51.000000 i18nice-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 20:35:51.000000 i18nice-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8100 2023-07-30 20:35:59.126722 i18nice-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-07-30 20:35:51.000000 i18nice-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.122722 i18nice-0.7.0/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4807 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.122722 i18nice-0.7.0/i18n/loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/python_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/loaders/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/resource_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/translations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-07-30 20:35:51.000000 i18nice-0.7.0/i18n/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 20:35:59.126722 i18nice-0.7.0/i18nice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8100 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-30 20:35:59.000000 i18nice-0.7.0/i18nice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 20:35:58.000000 i18nice-0.7.0/i18nice.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 20:35:59.126722 i18nice-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-30 20:35:51.000000 i18nice-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 18:07:04.660184 i18nice-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-06 18:06:50.000000 i18nice-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-06 18:06:50.000000 i18nice-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8389 2023-08-06 18:07:04.660184 i18nice-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-08-06 18:06:50.000000 i18nice-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 18:07:04.656184 i18nice-0.8.0/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6302 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 18:07:04.656184 i18nice-0.8.0/i18n/loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/loaders/python_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/loaders/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/resource_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/translations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-08-06 18:06:50.000000 i18nice-0.8.0/i18n/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 18:07:04.660184 i18nice-0.8.0/i18nice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8389 2023-08-06 18:07:04.000000 i18nice-0.8.0/i18nice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-08-06 18:07:04.000000 i18nice-0.8.0/i18nice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 18:07:04.000000 i18nice-0.8.0/i18nice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-06 18:07:04.000000 i18nice-0.8.0/i18nice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-06 18:07:04.000000 i18nice-0.8.0/i18nice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 18:07:04.000000 i18nice-0.8.0/i18nice.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-06 18:07:04.660184 i18nice-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-08-06 18:06:50.000000 i18nice-0.8.0/setup.py
```

### Comparing `i18nice-0.7.0/LICENSE` & `i18nice-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i18nice-0.7.0/PKG-INFO` & `i18nice-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18nice
-Version: 0.7.0
+Version: 0.8.0
 Summary: Translation library for Python
 Home-page: https://github.com/Krutyi-4el/i18nice
 Download-URL: https://github.com/Krutyi-4el/i18nice/archive/master.zip
 Author: Daniel Perez
 Author-email: tuvistavie@gmail.com
 Maintainer: Krutyi 4el
 License: MIT
@@ -70,16 +70,23 @@
     i18n.register_loader(MyLoader, ["yml", "yaml"])
 
 ### Memoization
 
 Setting the configuration value `enable_memoization` will disable reloading of files every time when searching for missing translation.
 When translations are loaded, they're always stored in memory, hence it does not affect how existing translations are accessed.
 
-If you want to reload all translations, you can use `i18n.reload_everything()`.
- 
+### Load everything
+
+`i18n.load_everything()` will load every file in `load_path` and subdirectories that matches `filename_format` and `file_format`.
+You can call it with locale argument to load only one locale.
+
+`i18n.unload_everything()` will clear all caches.
+
+`i18n.reload_everything()` is just a shortcut for `unload_everything()` followed by `load_everything()`.
+
 ### Namespaces
 
 #### File namespaces
 In the above example, the translation key is `foo.hi` and not just `hi`. This is because the translation filename format is by default `{namespace}.{locale}.{format}`, so the {namespace} part of the file is used as translation.
 
 To remove `{namespace}` from filename format please change the `filename_format` configuration.
```

### Comparing `i18nice-0.7.0/README.md` & `i18nice-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,23 @@
     i18n.register_loader(MyLoader, ["yml", "yaml"])
 
 ### Memoization
 
 Setting the configuration value `enable_memoization` will disable reloading of files every time when searching for missing translation.
 When translations are loaded, they're always stored in memory, hence it does not affect how existing translations are accessed.
 
-If you want to reload all translations, you can use `i18n.reload_everything()`.
- 
+### Load everything
+
+`i18n.load_everything()` will load every file in `load_path` and subdirectories that matches `filename_format` and `file_format`.
+You can call it with locale argument to load only one locale.
+
+`i18n.unload_everything()` will clear all caches.
+
+`i18n.reload_everything()` is just a shortcut for `unload_everything()` followed by `load_everything()`.
+
 ### Namespaces
 
 #### File namespaces
 In the above example, the translation key is `foo.hi` and not just `hi`. This is because the translation filename format is by default `{namespace}.{locale}.{format}`, so the {namespace} part of the file is used as translation.
 
 To remove `{namespace}` from filename format please change the `filename_format` configuration.
```

### Comparing `i18nice-0.7.0/i18n/config.py` & `i18nice-0.8.0/i18n/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 from importlib import reload as _reload
 
 try:
     __import__("yaml")
     yaml_available = True
 except ImportError:
     yaml_available = False
@@ -16,14 +17,21 @@
 # in case if config is being reloaded
 try:
     from . import load_path
     load_path.clear()
 except ImportError:
     load_path = []
 
+
+FILENAME_VARS = dict.fromkeys(
+    ("namespace", "locale", "format"),
+    r"\w+",
+)
+
+
 settings = {
     'filename_format': '{namespace}.{locale}.{format}',
     'file_format': 'yml' if yaml_available else 'json' if json_available else 'py',
     'available_locales': ['en'],
     'load_path': load_path,
     'locale': 'en',
     'fallback': 'en',
@@ -35,24 +43,32 @@
     'namespace_delimiter': '.',
     'plural_few': 5,
     'skip_locale_root_data': False,
     'enable_memoization': False,
     'argument_delimiter': '|'
 }
 
-def set(key, value):
+def set(key: str, value: Any):
     if key not in settings:
         raise KeyError("Invalid setting: {0}".format(key))
     elif key == 'load_path':
         load_path.clear()
         load_path.extend(value)
         return
+    elif key == 'filename_format':
+        from .formatters import FilenameFormat
+
+        value = FilenameFormat(value, FILENAME_VARS)
 
     settings[key] = value
 
     if key in ('placeholder_delimiter', 'namespace_delimiter'):
         from . import formatters
 
         _reload(formatters)
 
-def get(key):
+def get(key: str) -> Any:
     return settings[key]
+
+
+# initialize FilenameFormat
+set('filename_format', get('filename_format'))
```

### Comparing `i18nice-0.7.0/i18n/formatters.py` & `i18nice-0.8.0/i18n/formatters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from re import escape
-from string import Template
+from re import compile, escape
+from string import Template, Formatter as _Fmt
 
 from . import config, translations
 from .translator import pluralize
-from .errors import I18nInvalidStaticRef
+from .errors import I18nInvalidStaticRef, I18nInvalidFormat
 from .custom_functions import get_function
 
 
 class Formatter(Template):
     delimiter = config.get("placeholder_delimiter")
 
     def __init__(self, translation_key, locale, value, kwargs):
@@ -143,7 +143,47 @@
 
 
 def expand_static_refs(keys, locale):
     for key in keys:
         tr = translations.get(key, locale)
         tr = StaticFormatter(key, locale, tr).format()
         translations.add(key, tr, locale)
+
+
+class FilenameFormat(_Fmt):
+    def __init__(self, template: str, variables: dict):
+        super().__init__()
+        self.template = template
+        self.variables = variables
+        self.used_variables = set()
+        self.pattern = compile(super().format(template))
+
+    @property
+    def format(self):
+        return self.template.format
+
+    @property
+    def match(self):
+        return self.pattern.fullmatch
+
+    def __getattr__(self, name: str):
+        if name.startswith("has_"):
+            _, _, var_name = name.partition("_")
+            if var_name in self.variables:
+                return var_name in self.used_variables
+        raise AttributeError(f"{self.__class__.__name__!r} object has no attribute {name!r}")
+
+    def parse(self, s):
+        for text, field, spec, conversion in super().parse(s):
+            if spec or conversion:
+                raise I18nInvalidFormat("Can't apply format spec or conversion in filename format")
+            text = escape(text)
+            if field is not None:
+                try:
+                    text += f"(?P<{field}>{self.variables[field]})"
+                except KeyError as e:
+                    raise I18nInvalidFormat(f"Unknown placeholder in filename format: {e}") from e
+                self.used_variables.add(field)
+            yield text, None, None, None
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.template!r}, {self.variables!r})"
```

### Comparing `i18nice-0.7.0/i18n/loaders/loader.py` & `i18nice-0.8.0/i18n/loaders/loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import io
 import os.path
+from typing import Optional, Dict
 
 from .. import config
 from ..errors import I18nFileLoadError
 
 
 class Loader(object):
     """Base class to load resources"""
 
-    loaded_files = {}
+    loaded_files: Dict[str, Optional[dict]] = {}
 
     def __init__(self):
         super(Loader, self).__init__()
 
-    def load_file(self, filename):
+    def load_file(self, filename: str) -> str:
         try:
             with io.open(filename, 'r', encoding=config.get('encoding')) as f:
                 return f.read()
         except IOError as e:
             raise I18nFileLoadError("error loading file {0}: {1}".format(filename, e.strerror)) from e
 
-    def parse_file(self, file_content):
+    def parse_file(self, file_content: str) -> dict:
         raise NotImplementedError("the method parse_file has not been implemented for class {0}".format(self.__class__.__name__))
 
-    def check_data(self, data, root_data):
+    def check_data(self, data: dict, root_data: Optional[str]) -> bool:
         return True if root_data is None else root_data in data
 
-    def get_data(self, data, root_data):
+    def get_data(self, data: dict, root_data: Optional[str]) -> dict:
         # use .pop to remove used data from cache
         return data if root_data is None else data.pop(root_data)
 
-    def load_resource(self, filename, root_data, remember_content):
+    def load_resource(self, filename: str, root_data: Optional[str], remember_content: bool) -> dict:
         filename = os.path.abspath(filename)
         if filename in self.loaded_files:
             data = self.loaded_files[filename]
             if not data:
                 # cache is missing or exhausted
                 return {}
         else:
```

### Comparing `i18nice-0.7.0/i18n/loaders/python_loader.py` & `i18nice-0.8.0/i18n/loaders/python_loader.py`

 * *Files identical despite different names*

### Comparing `i18nice-0.7.0/i18n/resource_loader.py` & `i18nice-0.8.0/i18n/resource_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os.path
+from typing import Type, Iterable, Optional
 
 from . import config
 from .loaders import Loader, I18nFileLoadError
 from . import translations, formatters
 
 loaders = {}
 
 PLURALS = {"zero", "one", "few", "many"}
 
 
-def register_loader(loader_class, supported_extensions):
+def register_loader(loader_class: Type[Loader], supported_extensions: Iterable[str]):
     if not issubclass(loader_class, Loader):
         raise ValueError("loader class should be subclass of i18n.Loader")
 
     loader = loader_class()
     for extension in supported_extensions:
         loaders[extension] = loader
 
@@ -44,89 +45,127 @@
 
 
 def init_json_loader():
     from .loaders import JsonLoader
     register_loader(JsonLoader, ["json"])
 
 
-def load_config(filename):
+def load_config(filename: str):
     settings_data = load_resource(filename, "settings")
     for key, value in settings_data.items():
         config.set(key, value)
 
 
 def get_namespace_from_filepath(filename):
     namespace = os.path.dirname(filename).strip(os.sep).replace(os.sep, config.get('namespace_delimiter'))
     format = config.get('filename_format')
-    if '{namespace}' in format:
-        try:
-            splitted_filename = os.path.basename(filename).split('.')
-            if namespace:
-                namespace += config.get('namespace_delimiter')
-            namespace += splitted_filename[format.split(".").index('{namespace}')]
-        except ValueError as e:
-            raise I18nFileLoadError("incorrect file format.") from e
+    if format.has_namespace:
+        filename_match = format.match(os.path.basename(filename))
+        if namespace:
+            namespace += config.get('namespace_delimiter')
+        namespace += filename_match.group("namespace")
     return namespace
 
 
 def load_translation_file(filename, base_directory, locale=None):
     if locale is None:
         locale = config.get('locale')
     skip_locale_root_data = config.get('skip_locale_root_data')
     root_data = None if skip_locale_root_data else locale
     # if the file isn't dedicated to one locale and may contain other `root_data`s
-    remember_content = "{locale}" not in config.get("filename_format") and root_data
+    remember_content = not config.get("filename_format").has_locale and root_data
     translations_dic = load_resource(os.path.join(base_directory, filename), root_data, remember_content)
     namespace = get_namespace_from_filepath(filename)
     loaded = load_translation_dic(translations_dic, namespace, locale)
     formatters.expand_static_refs(loaded, locale)
 
 
-def reload_everything():
+def load_everything(locale: Optional[str] = None):
+    for directory in config.get("load_path"):
+        recursive_load_everything(directory, "", locale)
+
+
+def unload_everything():
     translations.clear()
     Loader.loaded_files.clear()
 
 
+def reload_everything():
+    unload_everything()
+    load_everything()
+
+
 def load_translation_dic(dic, namespace, locale):
-    loaded = set()
+    loaded = []
     if namespace:
         namespace += config.get('namespace_delimiter')
     for key, value in dic.items():
         full_key = namespace + key
         if type(value) == dict and len(PLURALS.intersection(value)) < 2:
-            loaded.update(load_translation_dic(value, full_key, locale))
+            loaded.extend(load_translation_dic(value, full_key, locale))
         else:
             translations.add(full_key, value, locale)
-            loaded.add(full_key)
+            loaded.append(full_key)
     return loaded
 
 
-def load_directory(directory, locale):
-    for f in os.listdir(directory):
-        path = os.path.join(directory, f)
-        if os.path.isfile(path) and path.endswith(config.get('file_format')):
-            if '{locale}' in config.get('filename_format') and not locale in f:
-                continue
-            load_translation_file(f, directory, locale)
-
-
 def search_translation(key, locale=None):
     if locale is None:
         locale = config.get('locale')
     splitted_key = key.split(config.get('namespace_delimiter'))
     namespace = splitted_key[:-1]
-    if not namespace and '{namespace}' not in config.get('filename_format'):
-        for directory in config.get('load_path'):
-            load_directory(directory, locale)
-    else:
-        for directory in config.get('load_path'):
-            recursive_search_dir(namespace, '', directory, locale)
+    for directory in config.get("load_path"):
+        recursive_search_dir(namespace, "", directory, locale)
 
 
 def recursive_search_dir(splitted_namespace, directory, root_dir, locale):
     namespace = splitted_namespace[0] if splitted_namespace else ""
     seeked_file = config.get('filename_format').format(namespace=namespace, format=config.get('file_format'), locale=locale)
     dir_content = os.listdir(os.path.join(root_dir, directory))
     if seeked_file in dir_content:
         load_translation_file(os.path.join(directory, seeked_file), root_dir, locale)
     elif namespace in dir_content:
         recursive_search_dir(splitted_namespace[1:], os.path.join(directory, namespace), root_dir, locale)
+
+
+def recursive_load_everything(root_dir, directory, locale):
+    dir_ = os.path.join(root_dir, directory)
+    for f in os.listdir(dir_):
+        path = os.path.join(dir_, f)
+        if os.path.isfile(path):
+            if os.path.splitext(path)[1][1:] != config.get("file_format"):
+                continue
+            format_match = config.get("filename_format").match(f)
+            if not format_match:
+                continue
+            requested_locale = locale
+            file_locale = format_match.groupdict().get("locale", requested_locale)
+            if requested_locale is None:
+                requested_locale = file_locale
+            if requested_locale is not None:
+                if requested_locale == file_locale:
+                    load_translation_file(
+                        os.path.join(directory, f),
+                        root_dir,
+                        requested_locale,
+                    )
+            elif not config.get("skip_locale_root_data"):
+                file_content = load_resource(path, None, False)
+                for l, dic in file_content.items():
+                    if isinstance(dic, dict):
+                        load_translation_dic(
+                            dic,
+                            get_namespace_from_filepath(os.path.join(directory, f)),
+                            l,
+                        )
+            else:
+                raise I18nFileLoadError(
+                    f"Cannot identify locales for {path!r}:"
+                    " filename_format doesn't include locale"
+                    " and skip_locale_root_data is set to True"
+                )
+        elif os.path.isdir(path):
+            recursive_load_everything(
+                root_dir,
+                os.path.join(directory, f),
+                locale,
+            )
```

### Comparing `i18nice-0.7.0/i18n/translator.py` & `i18nice-0.8.0/i18n/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from . import config
 from . import resource_loader
 from . import translations, formatters
 
 
-def t(key, **kwargs):
-    locale = kwargs.pop('locale', config.get('locale'))
-    if translations.has(key, locale):
+def t(key: str, **kwargs) -> str:
+    locale = kwargs.pop('locale', None) or config.get('locale')
+    try:
         return translate(key, locale=locale, **kwargs)
-    else:
+    except KeyError:
         resource_loader.search_translation(key, locale)
         if translations.has(key, locale):
             return translate(key, locale=locale, **kwargs)
         elif locale != config.get('fallback'):
             return t(key, locale=config.get('fallback'), **kwargs)
     if 'default' in kwargs:
         return kwargs['default']
@@ -38,15 +38,15 @@
             self.locale,
             super().__getitem__(key),
             self.kwargs,
         ).format()
 
 
 def translate(key, **kwargs):
-    locale = kwargs.pop('locale', config.get('locale'))
+    locale = kwargs.pop('locale', None) or config.get('locale')
     translation = translations.get(key, locale=locale)
     if isinstance(translation, tuple):
         return LazyTranslationTuple(key, locale, translation, kwargs)
     else:
         return formatters.TranslationFormatter(key, locale, translation, kwargs).format()
```

### Comparing `i18nice-0.7.0/i18nice.egg-info/PKG-INFO` & `i18nice-0.8.0/i18nice.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18nice
-Version: 0.7.0
+Version: 0.8.0
 Summary: Translation library for Python
 Home-page: https://github.com/Krutyi-4el/i18nice
 Download-URL: https://github.com/Krutyi-4el/i18nice/archive/master.zip
 Author: Daniel Perez
 Author-email: tuvistavie@gmail.com
 Maintainer: Krutyi 4el
 License: MIT
@@ -70,16 +70,23 @@
     i18n.register_loader(MyLoader, ["yml", "yaml"])
 
 ### Memoization
 
 Setting the configuration value `enable_memoization` will disable reloading of files every time when searching for missing translation.
 When translations are loaded, they're always stored in memory, hence it does not affect how existing translations are accessed.
 
-If you want to reload all translations, you can use `i18n.reload_everything()`.
- 
+### Load everything
+
+`i18n.load_everything()` will load every file in `load_path` and subdirectories that matches `filename_format` and `file_format`.
+You can call it with locale argument to load only one locale.
+
+`i18n.unload_everything()` will clear all caches.
+
+`i18n.reload_everything()` is just a shortcut for `unload_everything()` followed by `load_everything()`.
+
 ### Namespaces
 
 #### File namespaces
 In the above example, the translation key is `foo.hi` and not just `hi`. This is because the translation filename format is by default `{namespace}.{locale}.{format}`, so the {namespace} part of the file is used as translation.
 
 To remove `{namespace}` from filename format please change the `filename_format` configuration.
```

### Comparing `i18nice-0.7.0/setup.py` & `i18nice-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='i18nice',
-    version='0.7.0',
+    version='0.8.0',
     description='Translation library for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Daniel Perez',
     author_email='tuvistavie@gmail.com',
     maintainer="Krutyi 4el",
     url='https://github.com/Krutyi-4el/i18nice',
```

