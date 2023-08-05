# Comparing `tmp/beet-0.9.3.tar.gz` & `tmp/beet-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beet-0.9.3.tar", last modified: Mon Feb 22 01:49:40 2021, max compression
+gzip compressed data, was "beet-0.9.4.tar", last modified: Tue Feb 23 23:49:49 2021, max compression
```

## Comparing `beet-0.9.3.tar` & `beet-0.9.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1073 2021-02-22 01:49:11.438037 beet-0.9.3/LICENSE
--rw-r--r--   0        0        0     6432 2021-02-22 01:49:11.442037 beet-0.9.3/README.md
--rw-r--r--   0        0        0      427 2021-02-22 01:49:35.069856 beet-0.9.3/beet/__init__.py
--rw-r--r--   0        0        0       44 2021-02-22 01:49:11.442037 beet-0.9.3/beet/__main__.py
--rw-r--r--   0        0        0        0 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/__init__.py
--rw-r--r--   0        0        0      547 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/function_header.py
--rw-r--r--   0        0        0     1225 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/inline_function.py
--rw-r--r--   0        0        0     1244 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     3039 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/lantern_load.py
--rw-r--r--   0        0        0      338 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/minify_function.py
--rw-r--r--   0        0        0      752 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/minify_json.py
--rw-r--r--   0        0        0     1274 2021-02-22 01:49:11.442037 beet-0.9.3/beet/contrib/render.py
--rw-r--r--   0        0        0        0 2021-02-22 01:49:11.442037 beet-0.9.3/beet/core/__init__.py
--rw-r--r--   0        0        0     5999 2021-02-22 01:49:11.442037 beet-0.9.3/beet/core/cache.py
--rw-r--r--   0        0        0     5384 2021-02-22 01:49:11.442037 beet-0.9.3/beet/core/container.py
--rw-r--r--   0        0        0     8787 2021-02-22 01:49:11.442037 beet-0.9.3/beet/core/file.py
--rw-r--r--   0        0        0      894 2021-02-22 01:49:11.442037 beet-0.9.3/beet/core/utils.py
--rw-r--r--   0        0        0     3113 2021-02-22 01:49:11.442037 beet-0.9.3/beet/core/watch.py
--rw-r--r--   0        0        0        0 2021-02-22 01:49:11.442037 beet-0.9.3/beet/library/__init__.py
--rw-r--r--   0        0        0    15979 2021-02-22 01:49:11.442037 beet-0.9.3/beet/library/base.py
--rw-r--r--   0        0        0    11170 2021-02-22 01:49:11.442037 beet-0.9.3/beet/library/data_pack.py
--rw-r--r--   0        0        0     5493 2021-02-22 01:49:11.442037 beet-0.9.3/beet/library/resource_pack.py
--rw-r--r--   0        0        0      343 2021-02-22 01:49:11.442037 beet-0.9.3/beet/library/utils.py
--rw-r--r--   0        0        0        0 2021-02-22 01:49:11.442037 beet-0.9.3/beet/py.typed
--rw-r--r--   0        0        0        0 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/__init__.py
--rw-r--r--   0        0        0     6807 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/cli.py
--rw-r--r--   0        0        0     5849 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/config.py
--rw-r--r--   0        0        0     3510 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/context.py
--rw-r--r--   0        0        0     3036 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/helpers.py
--rw-r--r--   0        0        0     3904 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/pipeline.py
--rw-r--r--   0        0        0    10195 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/project.py
--rw-r--r--   0        0        0     4038 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/template.py
--rw-r--r--   0        0        0     1769 2021-02-22 01:49:11.442037 beet-0.9.3/beet/toolchain/utils.py
--rw-r--r--   0        0        0     1485 2021-02-22 01:49:35.081856 beet-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     7655 2021-02-22 01:49:40.147811 beet-0.9.3/setup.py
--rw-r--r--   0        0        0     7420 2021-02-22 01:49:40.148382 beet-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-02-23 23:49:15.286186 beet-0.9.4/LICENSE
+-rw-r--r--   0        0        0     6360 2021-02-23 23:49:15.286186 beet-0.9.4/README.md
+-rw-r--r--   0        0        0      427 2021-02-23 23:49:42.630642 beet-0.9.4/beet/__init__.py
+-rw-r--r--   0        0        0       44 2021-02-23 23:49:15.286186 beet-0.9.4/beet/__main__.py
+-rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/__init__.py
+-rw-r--r--   0        0        0      547 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/function_header.py
+-rw-r--r--   0        0        0     1225 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/inline_function.py
+-rw-r--r--   0        0        0     1244 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     3039 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/lantern_load.py
+-rw-r--r--   0        0        0      338 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/minify_function.py
+-rw-r--r--   0        0        0      752 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/minify_json.py
+-rw-r--r--   0        0        0     1274 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/render.py
+-rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/__init__.py
+-rw-r--r--   0        0        0     5999 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/cache.py
+-rw-r--r--   0        0        0     5384 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/container.py
+-rw-r--r--   0        0        0     8787 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/file.py
+-rw-r--r--   0        0        0      894 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/utils.py
+-rw-r--r--   0        0        0     3113 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/watch.py
+-rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/__init__.py
+-rw-r--r--   0        0        0    15979 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/base.py
+-rw-r--r--   0        0        0    11575 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/data_pack.py
+-rw-r--r--   0        0        0     5493 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/resource_pack.py
+-rw-r--r--   0        0        0      343 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/utils.py
+-rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/py.typed
+-rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/toolchain/__init__.py
+-rw-r--r--   0        0        0     6807 2021-02-23 23:49:15.286186 beet-0.9.4/beet/toolchain/cli.py
+-rw-r--r--   0        0        0     5849 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/config.py
+-rw-r--r--   0        0        0     3510 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/context.py
+-rw-r--r--   0        0        0     3036 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/helpers.py
+-rw-r--r--   0        0        0     3904 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/pipeline.py
+-rw-r--r--   0        0        0    10195 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/project.py
+-rw-r--r--   0        0        0     4038 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/template.py
+-rw-r--r--   0        0        0     1769 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/utils.py
+-rw-r--r--   0        0        0     1479 2021-02-23 23:49:42.638642 beet-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     7581 2021-02-23 23:49:50.059672 beet-0.9.4/setup.py
+-rw-r--r--   0        0        0     7342 2021-02-23 23:49:50.060421 beet-0.9.4/PKG-INFO
```

### Comparing `beet-0.9.3/LICENSE` & `beet-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/README.md` & `beet-0.9.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-<img align="right" src="https://vberlier.github.io/beet/_images/logo.svg" alt="logo" width="76">
+<img align="right" src="logo.png" alt="logo" width="76">
 
 # Beet
 
-[![GitHub Actions](https://github.com/vberlier/beet/workflows/CI/badge.svg)](https://github.com/vberlier/beet/actions)
+[![GitHub Actions](https://github.com/mcbeet/beet/workflows/CI/badge.svg)](https://github.com/mcbeet/beet/actions)
 [![PyPI](https://img.shields.io/pypi/v/beet.svg)](https://pypi.org/project/beet/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/beet.svg)](https://pypi.org/project/beet/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 > The Minecraft pack development kit.
 
 ## Introduction
@@ -23,15 +23,15 @@
 - **Command-line** [https://youtu.be/fQ9up0ELPNE](https://youtu.be/fQ9up0ELPNE)
 - **Library overview** [https://youtu.be/LDvV4_l-PSc](https://youtu.be/LDvV4_l-PSc)
 - **Plugins basics** [https://youtu.be/XTzKmvHqd1g](https://youtu.be/XTzKmvHqd1g)
 - **Pipeline configuration** [https://youtu.be/QsnQncGxAAs](https://youtu.be/QsnQncGxAAs)
 
 ### Library
 
-> [Documentation](https://vberlier.github.io/beet/library/)
+> [Documentation](https://mcbeet.dev/library/)
 
 ```python
 from beet import ResourcePack, Texture
 
 # Open a zipped resource pack and add a custom stone texture
 with ResourcePack(path="stone.zip") as assets:
     assets["minecraft:block/stone"] = Texture(source_path="custom.png")
@@ -42,15 +42,15 @@
 - Create, read, edit and merge resource packs and data packs
 - Handle zipped and unzipped packs
 - Fast and lazy by default, files are transparently loaded when needed
 - Statically typed API enabling rich intellisense and autocompletion
 
 ### Toolchain
 
-> [Documentation](https://vberlier.github.io/beet/toolchain/)
+> [Documentation](https://mcbeet.dev/toolchain/)
 
 ```python
 from beet import Context, Function
 
 def greet(ctx: Context):
     """Plugin that adds a function for greeting the player."""
     ctx.data["greet:hello"] = Function(["say hello"], tags=["minecraft:load"])
@@ -133,8 +133,8 @@
 $ poetry run isort beet tests
 $ poetry run black beet tests
 $ poetry run black --check beet tests
 ```
 
 ---
 
-License - [MIT](https://github.com/vberlier/beet/blob/main/LICENSE)
+License - [MIT](https://github.com/mcbeet/beet/blob/main/LICENSE)
```

### Comparing `beet-0.9.3/beet/contrib/function_header.py` & `beet-0.9.4/beet/contrib/function_header.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/contrib/inline_function.py` & `beet-0.9.4/beet/contrib/inline_function.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/contrib/inline_function_tag.py` & `beet-0.9.4/beet/contrib/inline_function_tag.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/contrib/lantern_load.py` & `beet-0.9.4/beet/contrib/lantern_load.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/contrib/minify_json.py` & `beet-0.9.4/beet/contrib/minify_json.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/contrib/render.py` & `beet-0.9.4/beet/contrib/render.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/core/cache.py` & `beet-0.9.4/beet/core/cache.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/core/container.py` & `beet-0.9.4/beet/core/container.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/core/file.py` & `beet-0.9.4/beet/core/file.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/core/utils.py` & `beet-0.9.4/beet/core/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/core/watch.py` & `beet-0.9.4/beet/core/watch.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/library/base.py` & `beet-0.9.4/beet/library/base.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/library/data_pack.py` & `beet-0.9.4/beet/library/data_pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "ConfiguredCarver",
     "ConfiguredFeature",
     "ConfiguredStructureFeature",
     "ConfiguredSurfaceBuilder",
     "NoiseSettings",
     "ProcessorList",
     "TemplatePool",
+    "ItemModifier",
 ]
 
 
 import io
 from copy import deepcopy
 from dataclasses import dataclass
 from gzip import GzipFile
@@ -243,14 +244,21 @@
 class TemplatePool(JsonFile, NamespaceFile):
     """Class representing a worldgen template pool."""
 
     scope = ("worldgen", "template_pool")
     extension = ".json"
 
 
+class ItemModifier(JsonFile, NamespaceFile):
+    """Class representing an item modifier."""
+
+    scope = ("item_modifiers",)
+    extension = ".json"
+
+
 class DataPackNamespace(Namespace):
     """Class representing a data pack namespace."""
 
     directory = "data"
 
     # fmt: off
     advancements:                  NamespacePin[Advancement]                = NamespacePin(Advancement)
@@ -270,14 +278,15 @@
     configured_carvers:            NamespacePin[ConfiguredCarver]           = NamespacePin(ConfiguredCarver)
     configured_features:           NamespacePin[ConfiguredFeature]          = NamespacePin(ConfiguredFeature)
     configured_structure_features: NamespacePin[ConfiguredStructureFeature] = NamespacePin(ConfiguredStructureFeature)
     configured_surface_builders:   NamespacePin[ConfiguredSurfaceBuilder]   = NamespacePin(ConfiguredSurfaceBuilder)
     noise_settings:                NamespacePin[NoiseSettings]              = NamespacePin(NoiseSettings)
     processor_lists:               NamespacePin[ProcessorList]              = NamespacePin(ProcessorList)
     template_pools:                NamespacePin[TemplatePool]               = NamespacePin(TemplatePool)
+    item_modifiers:                NamespacePin[ItemModifier]               = NamespacePin(ItemModifier)
     # fmt: on
 
 
 class DataPack(Pack[DataPackNamespace]):
     """Class representing a data pack."""
 
     default_name = "untitled_data_pack"
@@ -301,8 +310,9 @@
     configured_carvers:            NamespaceProxyDescriptor[ConfiguredCarver]           = NamespaceProxyDescriptor(ConfiguredCarver)
     configured_features:           NamespaceProxyDescriptor[ConfiguredFeature]          = NamespaceProxyDescriptor(ConfiguredFeature)
     configured_structure_features: NamespaceProxyDescriptor[ConfiguredStructureFeature] = NamespaceProxyDescriptor(ConfiguredStructureFeature)
     configured_surface_builders:   NamespaceProxyDescriptor[ConfiguredSurfaceBuilder]   = NamespaceProxyDescriptor(ConfiguredSurfaceBuilder)
     noise_settings:                NamespaceProxyDescriptor[NoiseSettings]              = NamespaceProxyDescriptor(NoiseSettings)
     processor_lists:               NamespaceProxyDescriptor[ProcessorList]              = NamespaceProxyDescriptor(ProcessorList)
     template_pools:                NamespaceProxyDescriptor[TemplatePool]               = NamespaceProxyDescriptor(TemplatePool)
+    item_modifiers:                NamespaceProxyDescriptor[ItemModifier]               = NamespaceProxyDescriptor(ItemModifier)
     # fmt: on
```

### Comparing `beet-0.9.3/beet/library/resource_pack.py` & `beet-0.9.4/beet/library/resource_pack.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/cli.py` & `beet-0.9.4/beet/toolchain/cli.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/config.py` & `beet-0.9.4/beet/toolchain/config.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/context.py` & `beet-0.9.4/beet/toolchain/context.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/helpers.py` & `beet-0.9.4/beet/toolchain/helpers.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/pipeline.py` & `beet-0.9.4/beet/toolchain/pipeline.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/project.py` & `beet-0.9.4/beet/toolchain/project.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/template.py` & `beet-0.9.4/beet/toolchain/template.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/beet/toolchain/utils.py` & `beet-0.9.4/beet/toolchain/utils.py`

 * *Files identical despite different names*

### Comparing `beet-0.9.3/pyproject.toml` & `beet-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "beet"
-version = "0.9.3"
+version = "0.9.4"
 description = "The Minecraft pack development kit"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
-homepage = "https://github.com/vberlier/beet"
-repository = "https://github.com/vberlier/beet"
-documentation = "https://github.com/vberlier/beet"
+homepage = "https://github.com/mcbeet/beet"
+repository = "https://github.com/mcbeet/beet"
+documentation = "https://github.com/mcbeet/beet"
 
 readme = "README.md"
 
 keywords = [
   "beet",
   "minecraft",
   "datapack",
@@ -34,15 +34,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 pytest = "^6.2.2"
 rope = "^0.18.0"
 pytest-minecraft = "^0.1.1"
 isort = "^5.7.0"
-pytest-insta = "^0.1.4"
+pytest-insta = "^0.1.5"
 python-semantic-release = "^7.15.0"
 mudkip = "^0.3.8"
 
 [tool.poetry.scripts]
 beet = "beet.toolchain.cli:main"
 
 [tool.black]
```

### Comparing `beet-0.9.3/setup.py` & `beet-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 {':sys_platform == "win32"': ['colorama']}
 
 entry_points = \
 {'console_scripts': ['beet = beet.toolchain.cli:main']}
 
 setup_kwargs = {
     'name': 'beet',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'The Minecraft pack development kit',
-    'long_description': '<img align="right" src="https://vberlier.github.io/beet/_images/logo.svg" alt="logo" width="76">\n\n# Beet\n\n[![GitHub Actions](https://github.com/vberlier/beet/workflows/CI/badge.svg)](https://github.com/vberlier/beet/actions)\n[![PyPI](https://img.shields.io/pypi/v/beet.svg)](https://pypi.org/project/beet/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/beet.svg)](https://pypi.org/project/beet/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n> The Minecraft pack development kit.\n\n## Introduction\n\nMinecraft [resource packs](https://minecraft.gamepedia.com/Resource_Pack) and [data packs](https://minecraft.gamepedia.com/Data_Pack) work well as _distribution_ formats but can be pretty limiting as _authoring_ formats. Without the ability to parametrize or create abstractions over assets and data pack resources, projects and libraries created by the community are greatly limited when it comes to reusability and interoperability.\n\nThere\'s been a lot of attempts at establishing standardized tooling to improve the development experience and it\'s becoming more and more apparent that the problem space is fundamentally multi-paradigm. Different problems require different solutions, so providing unified cross-project reusability needs to involve an interoperability layer that\'s sufficiently unopinionated to let all these paradigms shine through.\n\nThe `beet` project is meant to serve as a platform for building a cooperative tooling ecosystem by providing a flexible composition model and a user-friendly development workflow.\n\n### Screencasts\n\n- **Quick start** [https://youtu.be/JGrJTOhG3pY](https://youtu.be/JGrJTOhG3pY)\n- **Command-line** [https://youtu.be/fQ9up0ELPNE](https://youtu.be/fQ9up0ELPNE)\n- **Library overview** [https://youtu.be/LDvV4_l-PSc](https://youtu.be/LDvV4_l-PSc)\n- **Plugins basics** [https://youtu.be/XTzKmvHqd1g](https://youtu.be/XTzKmvHqd1g)\n- **Pipeline configuration** [https://youtu.be/QsnQncGxAAs](https://youtu.be/QsnQncGxAAs)\n\n### Library\n\n> [Documentation](https://vberlier.github.io/beet/library/)\n\n```python\nfrom beet import ResourcePack, Texture\n\n# Open a zipped resource pack and add a custom stone texture\nwith ResourcePack(path="stone.zip") as assets:\n    assets["minecraft:block/stone"] = Texture(source_path="custom.png")\n```\n\nThe `beet` library provides carefully crafted primitives for working with Minecraft resource packs and data packs.\n\n- Create, read, edit and merge resource packs and data packs\n- Handle zipped and unzipped packs\n- Fast and lazy by default, files are transparently loaded when needed\n- Statically typed API enabling rich intellisense and autocompletion\n\n### Toolchain\n\n> [Documentation](https://vberlier.github.io/beet/toolchain/)\n\n```python\nfrom beet import Context, Function\n\ndef greet(ctx: Context):\n    """Plugin that adds a function for greeting the player."""\n    ctx.data["greet:hello"] = Function(["say hello"], tags=["minecraft:load"])\n```\n\nThe `beet` toolchain is designed to support a wide range of use-cases. The most basic pipeline will let you create configurable resource packs and data packs, but plugins make it easy to implement arbitrarily advanced workflows and tools like linters, asset generators and function pre-processors.\n\n- Compose plugins that can inspect and edit the generated resource pack and data pack\n- Configure powerful build systems for development and creating releases\n- First-class template integration approachable without prior Python knowledge\n- Link the generated resource pack and data pack to Minecraft\n- Automatically rebuild the project on file changes with watch mode\n\n## Installation\n\nThe package can be installed with `pip`.\n\n```bash\n$ pip install beet\n```\n\nYou can make sure that `beet` was successfully installed by trying to use the toolchain from the command-line.\n\n```bash\n$ beet --help\nUsage: beet [OPTIONS] COMMAND [ARGS]...\n\n  The beet toolchain.\n\nOptions:\n  -d, --directory DIRECTORY  Use the specified project directory.\n  -c, --config FILE          Use the specified config file.\n  -v, --version              Show the version and exit.\n  -h, --help                 Show this message and exit.\n\nCommands:\n  build  Build the current project.\n  cache  Inspect or clear the cache.\n  link   Link the generated resource pack and data pack to Minecraft.\n  watch  Watch the project directory and build on file changes.\n```\n\n## Status\n\nYou can expect current releases to be pretty stable, but the project as a whole should still be considered alpha.\n\nThe main reason is that resource pack and data pack coverage is currently lacking in certain areas. Exposing a consistent interface for every data pack and resource pack feature can involve design decisions that aren\'t immediately obvious. You\'re welcome to open an issue to discuss the implementation of currently unsupported resources. And feel free to ask questions, report bugs, and share your thoughts and impressions.\n\n## Contributing\n\nContributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org).\n\n```bash\n$ poetry install\n```\n\nYou can run the tests with `poetry run pytest`. We use [`pytest-minecraft`](https://github.com/vberlier/pytest-minecraft) to run tests against actual Minecraft releases.\n\n```bash\n$ poetry run pytest\n$ poetry run pytest --minecraft-latest\n```\n\nWe also use [`pytest-insta`](https://github.com/vberlier/pytest-minecraft) for snapshot testing. Data pack and resource pack snapshots make it easy to monitor and review changes.\n\n```bash\n$ poetry run pytest --insta review\n```\n\nThe project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you\'re using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.\n\n```bash\n$ npm run watch\n$ npm run check\n```\n\nThe code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).\n\n```bash\n$ poetry run isort beet tests\n$ poetry run black beet tests\n$ poetry run black --check beet tests\n```\n\n---\n\nLicense - [MIT](https://github.com/vberlier/beet/blob/main/LICENSE)\n',
+    'long_description': '<img align="right" src="logo.png" alt="logo" width="76">\n\n# Beet\n\n[![GitHub Actions](https://github.com/mcbeet/beet/workflows/CI/badge.svg)](https://github.com/mcbeet/beet/actions)\n[![PyPI](https://img.shields.io/pypi/v/beet.svg)](https://pypi.org/project/beet/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/beet.svg)](https://pypi.org/project/beet/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n> The Minecraft pack development kit.\n\n## Introduction\n\nMinecraft [resource packs](https://minecraft.gamepedia.com/Resource_Pack) and [data packs](https://minecraft.gamepedia.com/Data_Pack) work well as _distribution_ formats but can be pretty limiting as _authoring_ formats. Without the ability to parametrize or create abstractions over assets and data pack resources, projects and libraries created by the community are greatly limited when it comes to reusability and interoperability.\n\nThere\'s been a lot of attempts at establishing standardized tooling to improve the development experience and it\'s becoming more and more apparent that the problem space is fundamentally multi-paradigm. Different problems require different solutions, so providing unified cross-project reusability needs to involve an interoperability layer that\'s sufficiently unopinionated to let all these paradigms shine through.\n\nThe `beet` project is meant to serve as a platform for building a cooperative tooling ecosystem by providing a flexible composition model and a user-friendly development workflow.\n\n### Screencasts\n\n- **Quick start** [https://youtu.be/JGrJTOhG3pY](https://youtu.be/JGrJTOhG3pY)\n- **Command-line** [https://youtu.be/fQ9up0ELPNE](https://youtu.be/fQ9up0ELPNE)\n- **Library overview** [https://youtu.be/LDvV4_l-PSc](https://youtu.be/LDvV4_l-PSc)\n- **Plugins basics** [https://youtu.be/XTzKmvHqd1g](https://youtu.be/XTzKmvHqd1g)\n- **Pipeline configuration** [https://youtu.be/QsnQncGxAAs](https://youtu.be/QsnQncGxAAs)\n\n### Library\n\n> [Documentation](https://mcbeet.dev/library/)\n\n```python\nfrom beet import ResourcePack, Texture\n\n# Open a zipped resource pack and add a custom stone texture\nwith ResourcePack(path="stone.zip") as assets:\n    assets["minecraft:block/stone"] = Texture(source_path="custom.png")\n```\n\nThe `beet` library provides carefully crafted primitives for working with Minecraft resource packs and data packs.\n\n- Create, read, edit and merge resource packs and data packs\n- Handle zipped and unzipped packs\n- Fast and lazy by default, files are transparently loaded when needed\n- Statically typed API enabling rich intellisense and autocompletion\n\n### Toolchain\n\n> [Documentation](https://mcbeet.dev/toolchain/)\n\n```python\nfrom beet import Context, Function\n\ndef greet(ctx: Context):\n    """Plugin that adds a function for greeting the player."""\n    ctx.data["greet:hello"] = Function(["say hello"], tags=["minecraft:load"])\n```\n\nThe `beet` toolchain is designed to support a wide range of use-cases. The most basic pipeline will let you create configurable resource packs and data packs, but plugins make it easy to implement arbitrarily advanced workflows and tools like linters, asset generators and function pre-processors.\n\n- Compose plugins that can inspect and edit the generated resource pack and data pack\n- Configure powerful build systems for development and creating releases\n- First-class template integration approachable without prior Python knowledge\n- Link the generated resource pack and data pack to Minecraft\n- Automatically rebuild the project on file changes with watch mode\n\n## Installation\n\nThe package can be installed with `pip`.\n\n```bash\n$ pip install beet\n```\n\nYou can make sure that `beet` was successfully installed by trying to use the toolchain from the command-line.\n\n```bash\n$ beet --help\nUsage: beet [OPTIONS] COMMAND [ARGS]...\n\n  The beet toolchain.\n\nOptions:\n  -d, --directory DIRECTORY  Use the specified project directory.\n  -c, --config FILE          Use the specified config file.\n  -v, --version              Show the version and exit.\n  -h, --help                 Show this message and exit.\n\nCommands:\n  build  Build the current project.\n  cache  Inspect or clear the cache.\n  link   Link the generated resource pack and data pack to Minecraft.\n  watch  Watch the project directory and build on file changes.\n```\n\n## Status\n\nYou can expect current releases to be pretty stable, but the project as a whole should still be considered alpha.\n\nThe main reason is that resource pack and data pack coverage is currently lacking in certain areas. Exposing a consistent interface for every data pack and resource pack feature can involve design decisions that aren\'t immediately obvious. You\'re welcome to open an issue to discuss the implementation of currently unsupported resources. And feel free to ask questions, report bugs, and share your thoughts and impressions.\n\n## Contributing\n\nContributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org).\n\n```bash\n$ poetry install\n```\n\nYou can run the tests with `poetry run pytest`. We use [`pytest-minecraft`](https://github.com/vberlier/pytest-minecraft) to run tests against actual Minecraft releases.\n\n```bash\n$ poetry run pytest\n$ poetry run pytest --minecraft-latest\n```\n\nWe also use [`pytest-insta`](https://github.com/vberlier/pytest-minecraft) for snapshot testing. Data pack and resource pack snapshots make it easy to monitor and review changes.\n\n```bash\n$ poetry run pytest --insta review\n```\n\nThe project must type-check with [`pyright`](https://github.com/microsoft/pyright). If you\'re using VSCode the [`pylance`](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) extension should report diagnostics automatically. You can also install the type-checker locally with `npm install` and run it from the command-line.\n\n```bash\n$ npm run watch\n$ npm run check\n```\n\nThe code follows the [`black`](https://github.com/psf/black) code style. Import statements are sorted with [`isort`](https://pycqa.github.io/isort/).\n\n```bash\n$ poetry run isort beet tests\n$ poetry run black beet tests\n$ poetry run black --check beet tests\n```\n\n---\n\nLicense - [MIT](https://github.com/mcbeet/beet/blob/main/LICENSE)\n',
     'author': 'Valentin Berlier',
     'author_email': 'berlier.v@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
-    'url': 'https://github.com/vberlier/beet',
+    'url': 'https://github.com/mcbeet/beet',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `beet-0.9.3/PKG-INFO` & `beet-0.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: beet
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Minecraft pack development kit
-Home-page: https://github.com/vberlier/beet
+Home-page: https://github.com/mcbeet/beet
 License: MIT
 Keywords: beet,minecraft,datapack,resourcepack,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,23 +16,23 @@
 Requires-Dist: Pillow (>=8.0.1,<9.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: click-help-colors (>=0.9,<0.10)
 Requires-Dist: colorama; sys_platform == "win32"
 Requires-Dist: nbtlib (>=1.8.2,<2.0.0)
 Requires-Dist: pathspec (>=0.8.1,<0.9.0)
 Requires-Dist: pydantic (>=1.7.3,<2.0.0)
-Project-URL: Documentation, https://github.com/vberlier/beet
-Project-URL: Repository, https://github.com/vberlier/beet
+Project-URL: Documentation, https://github.com/mcbeet/beet
+Project-URL: Repository, https://github.com/mcbeet/beet
 Description-Content-Type: text/markdown
 
-<img align="right" src="https://vberlier.github.io/beet/_images/logo.svg" alt="logo" width="76">
+<img align="right" src="logo.png" alt="logo" width="76">
 
 # Beet
 
-[![GitHub Actions](https://github.com/vberlier/beet/workflows/CI/badge.svg)](https://github.com/vberlier/beet/actions)
+[![GitHub Actions](https://github.com/mcbeet/beet/workflows/CI/badge.svg)](https://github.com/mcbeet/beet/actions)
 [![PyPI](https://img.shields.io/pypi/v/beet.svg)](https://pypi.org/project/beet/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/beet.svg)](https://pypi.org/project/beet/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 > The Minecraft pack development kit.
 
 ## Introduction
@@ -49,15 +49,15 @@
 - **Command-line** [https://youtu.be/fQ9up0ELPNE](https://youtu.be/fQ9up0ELPNE)
 - **Library overview** [https://youtu.be/LDvV4_l-PSc](https://youtu.be/LDvV4_l-PSc)
 - **Plugins basics** [https://youtu.be/XTzKmvHqd1g](https://youtu.be/XTzKmvHqd1g)
 - **Pipeline configuration** [https://youtu.be/QsnQncGxAAs](https://youtu.be/QsnQncGxAAs)
 
 ### Library
 
-> [Documentation](https://vberlier.github.io/beet/library/)
+> [Documentation](https://mcbeet.dev/library/)
 
 ```python
 from beet import ResourcePack, Texture
 
 # Open a zipped resource pack and add a custom stone texture
 with ResourcePack(path="stone.zip") as assets:
     assets["minecraft:block/stone"] = Texture(source_path="custom.png")
@@ -68,15 +68,15 @@
 - Create, read, edit and merge resource packs and data packs
 - Handle zipped and unzipped packs
 - Fast and lazy by default, files are transparently loaded when needed
 - Statically typed API enabling rich intellisense and autocompletion
 
 ### Toolchain
 
-> [Documentation](https://vberlier.github.io/beet/toolchain/)
+> [Documentation](https://mcbeet.dev/toolchain/)
 
 ```python
 from beet import Context, Function
 
 def greet(ctx: Context):
     """Plugin that adds a function for greeting the player."""
     ctx.data["greet:hello"] = Function(["say hello"], tags=["minecraft:load"])
@@ -159,9 +159,9 @@
 $ poetry run isort beet tests
 $ poetry run black beet tests
 $ poetry run black --check beet tests
 ```
 
 ---
 
-License - [MIT](https://github.com/vberlier/beet/blob/main/LICENSE)
+License - [MIT](https://github.com/mcbeet/beet/blob/main/LICENSE)
```

