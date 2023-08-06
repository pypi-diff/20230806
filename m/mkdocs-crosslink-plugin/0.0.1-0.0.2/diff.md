# Comparing `tmp/mkdocs-crosslink-plugin-0.0.1.tar.gz` & `tmp/mkdocs-crosslink-plugin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-crosslink-plugin-0.0.1.tar", last modified: Fri Aug  4 11:01:12 2023, max compression
+gzip compressed data, was "mkdocs-crosslink-plugin-0.0.2.tar", last modified: Sun Aug  6 17:00:44 2023, max compression
```

## Comparing `mkdocs-crosslink-plugin-0.0.1.tar` & `mkdocs-crosslink-plugin-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-04 11:01:12.309883 mkdocs-crosslink-plugin-0.0.1/
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-08-04 17:39:49.000000 mkdocs-crosslink-plugin-0.0.1/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      160 2022-08-04 17:39:49.000000 mkdocs-crosslink-plugin-0.0.1/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     2831 2023-08-04 11:01:12.309935 mkdocs-crosslink-plugin-0.0.1/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     2194 2023-08-04 11:00:54.000000 mkdocs-crosslink-plugin-0.0.1/README.md
--rw-r--r--   0 user       (501) staff       (20)       85 2022-08-04 17:39:49.000000 mkdocs-crosslink-plugin-0.0.1/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)      894 2023-08-04 11:01:12.310171 mkdocs-crosslink-plugin-0.0.1/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-04 11:01:12.306866 mkdocs-crosslink-plugin-0.0.1/src/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-04 11:01:12.308886 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/
--rw-r--r--   0 user       (501) staff       (20)      469 2023-08-04 10:31:13.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4744 2023-08-03 16:52:42.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/config.py
--rw-r--r--   0 user       (501) staff       (20)     2497 2023-07-31 12:38:52.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/file_cache.py
--rw-r--r--   0 user       (501) staff       (20)     1704 2023-07-31 12:38:52.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/plugin.py
--rw-r--r--   0 user       (501) staff       (20)     6690 2023-08-04 10:36:27.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/replacer.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-04 11:01:12.309762 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     2831 2023-08-04 11:01:12.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      560 2023-08-04 11:01:12.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-08-04 11:01:12.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       69 2023-08-04 11:01:12.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2023-08-04 11:01:12.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       24 2023-08-04 11:01:12.000000 mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-06 17:00:44.760403 mkdocs-crosslink-plugin-0.0.2/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2022-08-04 17:39:49.000000 mkdocs-crosslink-plugin-0.0.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      160 2022-08-04 17:39:49.000000 mkdocs-crosslink-plugin-0.0.2/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     3852 2023-08-06 17:00:44.760493 mkdocs-crosslink-plugin-0.0.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3215 2023-08-06 16:59:25.000000 mkdocs-crosslink-plugin-0.0.2/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2022-08-04 17:39:49.000000 mkdocs-crosslink-plugin-0.0.2/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)      894 2023-08-06 17:00:44.760759 mkdocs-crosslink-plugin-0.0.2/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-06 17:00:44.757243 mkdocs-crosslink-plugin-0.0.2/src/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-06 17:00:44.759522 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/
+-rw-r--r--   0 user       (501) staff       (20)      544 2023-08-06 16:25:43.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     8653 2023-08-06 17:00:18.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/config.py
+-rw-r--r--   0 user       (501) staff       (20)     3534 2023-08-06 12:00:49.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/file_cache.py
+-rw-r--r--   0 user       (501) staff       (20)     2077 2023-08-06 16:51:51.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)     1555 2023-08-06 16:50:57.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/profiling.py
+-rw-r--r--   0 user       (501) staff       (20)     8111 2023-08-06 17:00:26.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/replacer.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-08-06 17:00:44.760283 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3852 2023-08-06 17:00:44.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      601 2023-08-06 17:00:44.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-08-06 17:00:44.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       69 2023-08-06 17:00:44.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-08-06 17:00:44.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       24 2023-08-06 17:00:44.000000 mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/top_level.txt
```

### Comparing `mkdocs-crosslink-plugin-0.0.1/LICENSE` & `mkdocs-crosslink-plugin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-crosslink-plugin-0.0.1/README.md` & `mkdocs-crosslink-plugin-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mkdocs-crosslink-plugin
 [![PyPI version](https://img.shields.io/pypi/v/mkdocs-crosslink-plugin)](https://pypi.org/project/mkdocs-crosslink-plugin/)
 ![License](https://img.shields.io/pypi/l/mkdocs-crosslink-plugin)
 ![Python versions](https://img.shields.io/pypi/pyversions/mkdocs-crosslink-plugin)
 
-This package allows you to add links to other MkDocs (or similar page generator) sites.
+This package allows you to add links to other MkDocs sites (or sites created with similar page generator).
 
 ## Usage
 
 First install the PyPI package:
 ```bash
 pip install mkdocs-crosslink-plugin
 ```
@@ -34,22 +34,37 @@
     By default the schema is `x-NAME:FILE_NAME` (so for example `x-alpha:my-image.png`).
 - `source_dir` is the directory containing the Markdown files.
 - `target_url` is the path, where the site corresponding to the `source_dir` files are hosted.
 - `use_directory_urls` should correspond to the target site's `use_directory_urls` settings.
     - If enabled `path/index.md` will be mapped to `path/` and `path/test.md` will be mapped to `path/test/`.
     - If disabled `path/index.md` will be mapped to `path/index.html` and `path/test.md` will be mapped to `path/test.html`.
 
+Starting with version 0.0.2 you can also define multiple crosslinks at once, by using a glob-like syntax.
+Inject a `*` character in the `name`, `source_dir`, and `target_url`.
+The plugin will then look for directories matching the `source_dir` glob, create a crosslink for each one that was not defined before, and replace the `*` in the `name` and `target_url` with the same value that it matched in the `source_dir` value.
+
+Starting with version 0.0.2 there is also a builtin `local` crosslink, which can be used to reference files in the current site, similar to other autolink tools.
 
 On your pages you can reference links and images to other sites with the `x-SITE_NAME:FILE_NAME` syntax.
 For example to load the image `my-image.png` somewhere from the `https://example.com/` (crosslink `example`) you would use the syntax:
 ```markdown
 ![My Image](x-example:my-image.png)
 ```
 
 If multiple files with the exact same name exist, there is currently now way to reference the correct one.
 In the future I plan to let you specify a part of the path to select the correct file.
-
+From 0.0.2 on: For index files (`index.md` or `index.html`) you can reference them by the name of the parent's directory followed by a slash.
+So `/path/to/some/index.md` can be referenced as `some/`.
 
 ## Testing
 
 Some very basic tests are in `docs` (main site), `site_a` (crosslink alpha), and `site_b` (crosslink bravo).
 You can build and serve the test site by running `./build.sh`.
+
+## Notable changes
+
+### Version 0.0.2
+
+- Added builtin `local` crosslink
+- Reference `index.md` as `<PARENT_DIR_NAME>/`
+- Added glob support for crosslinks
+- Added profiling option (`show_profiling_results: True`)
```

### Comparing `mkdocs-crosslink-plugin-0.0.1/setup.cfg` & `mkdocs-crosslink-plugin-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = mkdocs-crosslink-plugin
-version = 0.0.1
+version = 0.0.2
 author = six-two
 author_email = pip@six-two.dev
-description = Simplify linking between different MkDocs pages
+description = Simplify linking between different MkDocs sites
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/mkdocs-crosslink-plugin
 license = MIT License
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
```

### Comparing `mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/file_cache.py` & `mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/file_cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 from pathlib import Path
 import os
+import re
+
+PATH_SEPARATOR_REGEX = re.compile(r"[/\\]+")
 
 class MultiValueDict:
     def __init__(self) -> None:
-        self._data = {}
+        self._data: dict[str,list[str]] = {}
 
     def append(self, key: str, value: str):
         if key in self._data:
             self._data[key].append(value)
         else:
             self._data[key] = [value]
 
@@ -32,32 +35,54 @@
 
         for path in files_root.rglob("*"):
             self._add_file_to_caches(path, files_root)
 
     def _add_file_to_caches(self, path: Path, files_root: Path):
         if path.is_file():
             name = path.name
+            # Relative path with Unix path separators
             path_str = os.path.relpath(path, files_root)
+            path_str = normalize_path_str(path_str)
+
+            # Also register index files with the name of the directory.
+            # So you could reference /some/path/index.md as 'path/'
+            # Otherwise referencing index files is a real pain, since every one has the same name
+            if name == "index.md" or name == "index.html":
+                dir_name = path.parent.name if path.parent != files_root else ""
+                self._caches[0].append(f"{dir_name}/", path_str)
+
             # Add file name to caches
             for cache in self._caches:
                 cache.append(name, path_str)
                 # remove the last extension from the name
                 parts = name.rsplit(".", 1)
                 if len(parts) == 2:
                     name = parts[0]
                 else:
                     # There is nothing left to split off -> exit inner look
                     break
 
-    def get(self, key: str) -> list[str]:
+    def get_matches(self, pattern: str) -> list[str]:
         # Search the caches: first interpret it as a full file name, then as a file name without the last extension, then a filename without the last two extensions, etc
         # So for example "jquery" would match "jquery", "jquery.js", "jquery.min.js", and finally "jquery.min.js.bak" in that order
+        pattern = normalize_path_str(pattern)
+        if pattern.endswith("/"):
+            key = os.path.basename(pattern[:-1]) + "/"
+        else:
+            key = os.path.basename(pattern)
+        
         for cache in self._caches:
             if result := cache.get(key):
                 return result
         
         # No matches found
         return []
     
     def __str__(self) -> str:
         return "<FileCache>" + "".join([f"\t\nLevel {index}: {cache}" for index, cache in enumerate(self._caches)]) + "\n</FileCache>"
 
+
+def normalize_path_str(path: str) -> str:
+    """
+    This removes duplicate path separators and replaces backslashes with forward slashes
+    """
+    return PATH_SEPARATOR_REGEX.sub("/", path)
```

### Comparing `mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/plugin.py` & `mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-from pathlib import Path
-import re
 # pip dependency
 import mkdocs
-from mkdocs.config.config_options import Type
-from mkdocs.plugins import BasePlugin, event_priority
-from mkdocs.config.base import Config
+from mkdocs.plugins import BasePlugin
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.structure.files import Files
 # local files
-from . import warning
-from .file_cache import FileCache
-from .config import parse_crosslinks_list, CrosslinkPluginConfig
+from .config import parse_crosslinks_list, create_local_crosslink, CrosslinkPluginConfig, CrosslinkSite
 from .replacer import Replacer
+from .profiling import Profiler
+
+PROFILER = Profiler()
 
 
 class CrosslinkPlugin(BasePlugin[CrosslinkPluginConfig]):
-    def on_config(self, config: MkDocsConfig, **kwargs) -> Config:
+    @PROFILER.profile
+    def on_config(self, config: MkDocsConfig, **kwargs) -> MkDocsConfig:
         """
         Called once when the config is loaded.
         It will make modify the config and initialize this plugin.
         """
-        self.crosslinks = parse_crosslinks_list(self.config.crosslinks, "crosslinks")
+        self.crosslinks: dict[str,CrosslinkSite] = {}
+        parse_crosslinks_list(self.config.crosslinks, "crosslinks", self.crosslinks)
+
+        # If not already created/overwritten by the user, provide a default value for 'local'
+        local_crosslink = create_local_crosslink(config)
+        if local_crosslink.name not in self.crosslinks:
+            self.crosslinks[local_crosslink.name] = local_crosslink
 
-        self.replacer = Replacer(self.crosslinks, self.config)
+        self.replacer = Replacer(list(self.crosslinks.values()), self.config) # @TODO: make it work with a dict?
         return config
 
 
     # @event_priority(50)
-    # Earlier than most other plugins to update the tags properly. Did not work
     # SEE https://www.mkdocs.org/dev-guide/plugins/#event-priorities
+    @PROFILER.profile
     def on_page_content(self, html: str, page: Page, config: MkDocsConfig, files: Files) -> str:
         """
         The page_content event is called after the Markdown text is rendered to HTML (but before being passed to a template) and can be used to alter the HTML body of the page.
         See: https://www.mkdocs.org/dev-guide/plugins/#on_page_content
         """
         try:
             html = self.replacer.handle_page(page.file.src_path, html)
-                
-
             return html
         except Exception as error:
             raise mkdocs.exceptions.PluginError(str(error))
 
+    def on_post_build(self, config: MkDocsConfig) -> None:
+        if self.config.show_profiling_results:
+            PROFILER.log_stats()
```

### Comparing `mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin/replacer.py` & `mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin/replacer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from pathlib import Path
 import re
+from typing import Optional
 import urllib
 # local files
 from . import warning, debug
 from .file_cache import FileCache
 from .config import CrosslinkSite, CrosslinkPluginConfig
 
 
@@ -34,15 +34,14 @@
         for crosslink in crosslink_list:
             self.full_name[crosslink.name] = f"{config.prefix}{crosslink.name}{config.suffix}"
             self.caches[crosslink.name] = FileCache(crosslink.source_dir)
             debug(f"Cache for '{crosslink.name}': {self.caches[crosslink.name]}")
 
 
     def handle_page(self, file_name: str, html: str) -> str:
-        warning(f"({file_name}) Got page ({len(html)} bytes)")
         file_contents = html
         for regex in self.regexes:
             search_start_pos = 0
 
             # replace / handle all matches
             while match := regex.search(file_contents, search_start_pos):
                 file_contents, search_start_pos = self.handle_potential_occurence(file_name, file_contents, match)
@@ -50,51 +49,79 @@
             # for match in regex.findall(html):
             #     warning(f"Match: '{match}' matched by {regex.pattern}")
         return file_contents
 
 
     def handle_potential_occurence(self, file_name: str, html: str, match: re.Match) -> tuple[str,int]:
         # Return the updated document and the index to start the next search from
-        start, end = match.span()
-        
+        start, end = match.span()        
         url = match.group(1) # 0: full match, 1: first capture group, ...
-        proto_names = [name for name, full_name in self.full_name.items() if url.startswith(full_name)]
 
-        if proto_names:
-            if len(proto_names) > 1:
-                # Best effort match: take the first one (after sorting), similar to file ambiguities
-                proto_names = list(sorted(proto_names))
-                warning(f"({file_name}) Ambiguity resolving '{url}'. Multiple crosslink protocols match: {', '.join(proto_names)}")
-
-            # Perfect, only one fake protocol / is left. So let's replace it
-            crosslink_name = proto_names[0]
+        crosslink_name = self.get_proto_for_url(file_name, url)
+        if crosslink_name:
             new_url = self.resolve_crosslink(file_name, url, crosslink_name)
             new_url_updated = self.update_file_url_if_needed(new_url, crosslink_name)
             debug(f"Resolving: {url} -> {new_url} -> {new_url_updated}")
 
             # update the URL
             updated_tag = html[start:end].replace(url, new_url_updated)
             html = html[:start] + updated_tag + html[end:]
             return (html, start + len(updated_tag))
         else:
             # No matches, seems to be a normal link
             return (html, start + 1)
+    
+    def get_proto_for_url(self, file_name: str, url: str) -> Optional[str]:
+        proto_name_list = [name for name, full_name in self.full_name.items() if url.startswith(full_name)]
+
+        if not proto_name_list:
+            # None of our protocols match, so we return None
+            return None
+        elif len(proto_name_list) == 1:
+            # Perfect, exactly one protocol matches -> return it
+            return proto_name_list[0]
+        else:
+            # Multiple protocols could match
+            # Best effort match: take the first one (after sorting) that can resolve a file, similar to file ambiguities
+            proto_name_list = list(sorted(proto_name_list))
+            warning(f"({file_name}) Ambiguity resolving '{url}'. Multiple crosslink protocols match: {', '.join(proto_name_list)}")
+            for proto_name in proto_name_list:
+                if self.can_resolve_crosslink(url, proto_name):
+                    debug(f"({file_name}) Ambiguity resolution for '{url}' chose protocol '{proto_name}'.")
+                    return proto_name
+            
+            # Ok, this is worse, none of the protocols match. The user must fix it
+            warning(f"({file_name}) Ambiguity resolution for '{url}' found no potential matches'.")
+            return None
+
+    def can_resolve_crosslink(self, crosslink_url: str, crosslink_name: str) -> bool:
+        """
+        This function check, whether a URL could be resolved given the protocol.
+        It can be used in case of protocol ambiguities to check which protocols are more likely (because they can resolve the file)
+        """
+        crosslink_proto = self.full_name[crosslink_name]
+        file_path = crosslink_url[len(crosslink_proto):] # Get everything after the proto.
+        if os.path.isabs(file_path):
+            # Absolute URL should work -> true
+            return True
+        else:
+            cache = self.caches[crosslink_name]
+            results = cache.get_matches(file_path)
+            # We do not care if there is an ambiguity in the file path, just whether there are results
+            return len(results) > 0
 
     def resolve_crosslink(self, file_name: str, crosslink_url: str, crosslink_name: str) -> str:
         base_url = self.crosslinks[crosslink_name].target_url
         crosslink_proto = self.full_name[crosslink_name]
         file_path = crosslink_url[len(crosslink_proto):] # Get everything after the proto.
         if not os.path.isabs(file_path):
-            # Relative path or just a file name. Look it up 
-            # @TODO later: check the path and use it in case of duplicates?
-            name = os.path.basename(file_path)
             cache = self.caches[crosslink_name]
-            results = cache.get(name)
+            results = cache.get_matches(file_path)
             if not results:
-                warning(f"({file_name}) Error resolving '{crosslink_url}'. Could not find a file called '{name}' in {cache.files_root}")
+                warning(f"({file_name}) Error resolving '{crosslink_url}'. Could not find a file matching '{file_path}' in {cache.files_root}")
                 return "#crosslink-error"
             elif len(results) == 1:
                 # Only one result -> use it
                 return join_url(base_url, results[0])
             else:
                 # Multipe results. Send a warning. Since I do not (yet) know which is the best,
                 # I sort them (to make it predictable) and return the first one
```

### Comparing `mkdocs-crosslink-plugin-0.0.1/src/mkdocs_crosslink_plugin.egg-info/SOURCES.txt` & `mkdocs-crosslink-plugin-0.0.2/src/mkdocs_crosslink_plugin.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/mkdocs_crosslink_plugin/__init__.py
 src/mkdocs_crosslink_plugin/config.py
 src/mkdocs_crosslink_plugin/file_cache.py
 src/mkdocs_crosslink_plugin/plugin.py
+src/mkdocs_crosslink_plugin/profiling.py
 src/mkdocs_crosslink_plugin/replacer.py
 src/mkdocs_crosslink_plugin.egg-info/PKG-INFO
 src/mkdocs_crosslink_plugin.egg-info/SOURCES.txt
 src/mkdocs_crosslink_plugin.egg-info/dependency_links.txt
 src/mkdocs_crosslink_plugin.egg-info/entry_points.txt
 src/mkdocs_crosslink_plugin.egg-info/requires.txt
 src/mkdocs_crosslink_plugin.egg-info/top_level.txt
```

