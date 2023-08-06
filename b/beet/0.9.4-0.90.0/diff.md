# Comparing `tmp/beet-0.9.4.tar.gz` & `tmp/beet-0.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beet-0.9.4.tar", last modified: Tue Feb 23 23:49:49 2021, max compression
+gzip compressed data, was "beet-0.90.0.tar", max compression
```

## Comparing `beet-0.9.4.tar` & `beet-0.90.0.tar`

### file list

```diff
@@ -1,36 +1,82 @@
--rw-r--r--   0        0        0     1073 2021-02-23 23:49:15.286186 beet-0.9.4/LICENSE
--rw-r--r--   0        0        0     6360 2021-02-23 23:49:15.286186 beet-0.9.4/README.md
--rw-r--r--   0        0        0      427 2021-02-23 23:49:42.630642 beet-0.9.4/beet/__init__.py
--rw-r--r--   0        0        0       44 2021-02-23 23:49:15.286186 beet-0.9.4/beet/__main__.py
--rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/__init__.py
--rw-r--r--   0        0        0      547 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/function_header.py
--rw-r--r--   0        0        0     1225 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/inline_function.py
--rw-r--r--   0        0        0     1244 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     3039 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/lantern_load.py
--rw-r--r--   0        0        0      338 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/minify_function.py
--rw-r--r--   0        0        0      752 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/minify_json.py
--rw-r--r--   0        0        0     1274 2021-02-23 23:49:15.286186 beet-0.9.4/beet/contrib/render.py
--rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/__init__.py
--rw-r--r--   0        0        0     5999 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/cache.py
--rw-r--r--   0        0        0     5384 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/container.py
--rw-r--r--   0        0        0     8787 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/file.py
--rw-r--r--   0        0        0      894 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/utils.py
--rw-r--r--   0        0        0     3113 2021-02-23 23:49:15.286186 beet-0.9.4/beet/core/watch.py
--rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/__init__.py
--rw-r--r--   0        0        0    15979 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/base.py
--rw-r--r--   0        0        0    11575 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/data_pack.py
--rw-r--r--   0        0        0     5493 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/resource_pack.py
--rw-r--r--   0        0        0      343 2021-02-23 23:49:15.286186 beet-0.9.4/beet/library/utils.py
--rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/py.typed
--rw-r--r--   0        0        0        0 2021-02-23 23:49:15.286186 beet-0.9.4/beet/toolchain/__init__.py
--rw-r--r--   0        0        0     6807 2021-02-23 23:49:15.286186 beet-0.9.4/beet/toolchain/cli.py
--rw-r--r--   0        0        0     5849 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/config.py
--rw-r--r--   0        0        0     3510 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/context.py
--rw-r--r--   0        0        0     3036 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/helpers.py
--rw-r--r--   0        0        0     3904 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/pipeline.py
--rw-r--r--   0        0        0    10195 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/project.py
--rw-r--r--   0        0        0     4038 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/template.py
--rw-r--r--   0        0        0     1769 2021-02-23 23:49:15.290186 beet-0.9.4/beet/toolchain/utils.py
--rw-r--r--   0        0        0     1479 2021-02-23 23:49:42.638642 beet-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     7581 2021-02-23 23:49:50.059672 beet-0.9.4/setup.py
--rw-r--r--   0        0        0     7342 2021-02-23 23:49:50.060421 beet-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-06 11:17:07.932692 beet-0.90.0/LICENSE
+-rw-r--r--   0        0        0     6048 2023-08-06 11:17:07.932692 beet-0.90.0/README.md
+-rw-r--r--   0        0        0      584 2023-08-06 11:17:40.085051 beet-0.90.0/beet/__init__.py
+-rw-r--r--   0        0        0       44 2023-08-06 11:17:07.932692 beet-0.90.0/beet/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/__init__.py
+-rw-r--r--   0        0        0     3265 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/auto_yaml.py
+-rw-r--r--   0        0        0     1369 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/autosave.py
+-rw-r--r--   0        0        0     2480 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/babelbox.py
+-rw-r--r--   0        0        0      574 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/clear.py
+-rw-r--r--   0        0        0     3005 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/copy_files.py
+-rw-r--r--   0        0        0     8040 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/dbg.py
+-rw-r--r--   0        0        0      187 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/default.py
+-rw-r--r--   0        0        0     1605 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/dundervar.py
+-rw-r--r--   0        0        0     1046 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/extra_files.py
+-rw-r--r--   0        0        0     3967 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/find_replace.py
+-rw-r--r--   0        0        0     1472 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/format_json.py
+-rw-r--r--   0        0        0      909 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/function_header.py
+-rw-r--r--   0        0        0     5701 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/hangman.py
+-rw-r--r--   0        0        0     1932 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/inline_function.py
+-rw-r--r--   0        0        0     1090 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     3811 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/installation_advancement.py
+-rw-r--r--   0        0        0     1771 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/json_log.py
+-rw-r--r--   0        0        0     5360 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/json_reporter.py
+-rw-r--r--   0        0        0     2871 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/lantern_load.py
+-rw-r--r--   0        0        0      816 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/line_endings.py
+-rw-r--r--   0        0        0     5916 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/link.py
+-rw-r--r--   0        0        0     6740 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/livereload.py
+-rw-r--r--   0        0        0     1742 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/load.py
+-rw-r--r--   0        0        0     4228 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/load_yaml.py
+-rw-r--r--   0        0        0      512 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/log_level.py
+-rw-r--r--   0        0        0     1587 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/messages.py
+-rw-r--r--   0        0        0      338 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/minify_function.py
+-rw-r--r--   0        0        0      235 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/minify_json.py
+-rw-r--r--   0        0        0     1590 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/model_merging.py
+-rw-r--r--   0        0        0     1591 2023-08-06 11:17:07.932692 beet-0.90.0/beet/contrib/optifine.py
+-rw-r--r--   0        0        0      960 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/output.py
+-rw-r--r--   0        0        0      959 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/relative_function_path.py
+-rw-r--r--   0        0        0     5219 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/rename_files.py
+-rw-r--r--   0        0        0     1503 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/render.py
+-rw-r--r--   0        0        0      882 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/sandstone.py
+-rw-r--r--   0        0        0      889 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/scoreboard.py
+-rw-r--r--   0        0        0      811 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/stdin.py
+-rw-r--r--   0        0        0     1357 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/strip_final_newlines.py
+-rw-r--r--   0        0        0      155 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/template_context.py
+-rw-r--r--   0        0        0      229 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/template_sandbox.py
+-rw-r--r--   0        0        0      897 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/text_encoding.py
+-rw-r--r--   0        0        0      775 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/unknown_files.py
+-rw-r--r--   0        0        0     7395 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/vanilla.py
+-rw-r--r--   0        0        0     5719 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/worldgen.py
+-rw-r--r--   0        0        0     2436 2023-08-06 11:17:07.936693 beet-0.90.0/beet/contrib/yellow_shulker_box.py
+-rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/__init__.py
+-rw-r--r--   0        0        0    11434 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/cache.py
+-rw-r--r--   0        0        0     5906 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/container.py
+-rw-r--r--   0        0        0      565 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/error.py
+-rw-r--r--   0        0        0    20025 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/file.py
+-rw-r--r--   0        0        0     8241 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/utils.py
+-rw-r--r--   0        0        0     3711 2023-08-06 11:17:07.936693 beet-0.90.0/beet/core/watch.py
+-rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/__init__.py
+-rw-r--r--   0        0        0    40084 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/base.py
+-rw-r--r--   0        0        0    11711 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/data_pack.py
+-rw-r--r--   0        0        0    11939 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/resource_pack.py
+-rw-r--r--   0        0        0      529 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/test_utils.py
+-rw-r--r--   0        0        0      660 2023-08-06 11:17:07.936693 beet-0.90.0/beet/library/utils.py
+-rw-r--r--   0        0        0       33 2023-08-06 11:17:07.936693 beet-0.90.0/beet/preset_stdin.yml
+-rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/py.typed
+-rw-r--r--   0        0        0     4266 2023-08-06 11:17:07.936693 beet-0.90.0/beet/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/__init__.py
+-rw-r--r--   0        0        0     8017 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/cli.py
+-rw-r--r--   0        0        0     4600 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/commands.py
+-rw-r--r--   0        0        0    14000 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/config.py
+-rw-r--r--   0        0        0    11226 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/context.py
+-rw-r--r--   0        0        0    11080 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/generator.py
+-rw-r--r--   0        0        0     3484 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/helpers.py
+-rw-r--r--   0        0        0     4355 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/pipeline.py
+-rw-r--r--   0        0        0    13374 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/project.py
+-rw-r--r--   0        0        0     6812 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/select.py
+-rw-r--r--   0        0        0     6457 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/template.py
+-rw-r--r--   0        0        0     3694 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/tree.py
+-rw-r--r--   0        0        0     4636 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/utils.py
+-rw-r--r--   0        0        0     9695 2023-08-06 11:17:07.936693 beet-0.90.0/beet/toolchain/worker.py
+-rw-r--r--   0        0        0     2277 2023-08-06 11:17:40.149052 beet-0.90.0/pyproject.toml
+-rw-r--r--   0        0        0     7140 1970-01-01 00:00:00.000000 beet-0.90.0/PKG-INFO
```

### Comparing `beet-0.9.4/LICENSE` & `beet-0.90.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beet-0.9.4/README.md` & `beet-0.90.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,82 @@
-<img align="right" src="logo.png" alt="logo" width="76">
+Metadata-Version: 2.1
+Name: beet
+Version: 0.90.0
+Summary: The Minecraft pack development kit
+Home-page: https://github.com/mcbeet/beet
+License: MIT
+Keywords: beet,minecraft,datapack,resourcepack,mcfunction
+Author: Valentin Berlier
+Author-email: berlier.v@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: image
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: Pillow ; extra == "image"
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
+Requires-Dist: colorama ; sys_platform == "win32"
+Requires-Dist: nbtlib (>=1.12.1,<2.0.0)
+Requires-Dist: pathspec (>=0.11.0,<0.12.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://github.com/mcbeet/beet
+Project-URL: Repository, https://github.com/mcbeet/beet
+Description-Content-Type: text/markdown
+
+<img align="right" src="https://raw.githubusercontent.com/mcbeet/beet/main/logo.png?sanitize=true" alt="logo" width="76">
 
 # Beet
 
 [![GitHub Actions](https://github.com/mcbeet/beet/workflows/CI/badge.svg)](https://github.com/mcbeet/beet/actions)
 [![PyPI](https://img.shields.io/pypi/v/beet.svg)](https://pypi.org/project/beet/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/beet.svg)](https://pypi.org/project/beet/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Discord](https://img.shields.io/discord/900530660677156924?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/98MdSGMm8j)
 
 > The Minecraft pack development kit.
 
 ## Introduction
 
-Minecraft [resource packs](https://minecraft.gamepedia.com/Resource_Pack) and [data packs](https://minecraft.gamepedia.com/Data_Pack) work well as _distribution_ formats but can be pretty limiting as _authoring_ formats. Without the ability to parametrize or create abstractions over assets and data pack resources, projects and libraries created by the community are greatly limited when it comes to reusability and interoperability.
-
-There's been a lot of attempts at establishing standardized tooling to improve the development experience and it's becoming more and more apparent that the problem space is fundamentally multi-paradigm. Different problems require different solutions, so providing unified cross-project reusability needs to involve an interoperability layer that's sufficiently unopinionated to let all these paradigms shine through.
+Minecraft [resource packs](https://minecraft.gamepedia.com/Resource_Pack) and [data packs](https://minecraft.gamepedia.com/Data_Pack) work well as _distribution_ formats but can be pretty limiting as _authoring_ formats. You can quickly end up having to manage hundreds of files, some of which might be buried within the bundled output of various generators.
 
-The `beet` project is meant to serve as a platform for building a cooperative tooling ecosystem by providing a flexible composition model and a user-friendly development workflow.
+The `beet` project is a development kit that tries to unify data pack and resource pack tooling into a single pipeline. The community is always coming up with pre-processors, frameworks, and generators of all kinds to make the developer experience more ergonomic. With `beet` you can seamlessly integrate all these tools in your project.
 
 ### Screencasts
 
 - **Quick start** [https://youtu.be/JGrJTOhG3pY](https://youtu.be/JGrJTOhG3pY)
 - **Command-line** [https://youtu.be/fQ9up0ELPNE](https://youtu.be/fQ9up0ELPNE)
 - **Library overview** [https://youtu.be/LDvV4_l-PSc](https://youtu.be/LDvV4_l-PSc)
 - **Plugins basics** [https://youtu.be/XTzKmvHqd1g](https://youtu.be/XTzKmvHqd1g)
 - **Pipeline configuration** [https://youtu.be/QsnQncGxAAs](https://youtu.be/QsnQncGxAAs)
 
 ### Library
 
-> [Documentation](https://mcbeet.dev/library/)
-
 ```python
 from beet import ResourcePack, Texture
 
 # Open a zipped resource pack and add a custom stone texture
 with ResourcePack(path="stone.zip") as assets:
     assets["minecraft:block/stone"] = Texture(source_path="custom.png")
 ```
 
 The `beet` library provides carefully crafted primitives for working with Minecraft resource packs and data packs.
 
 - Create, read, edit and merge resource packs and data packs
 - Handle zipped and unzipped packs
 - Fast and lazy by default, files are transparently loaded when needed
 - Statically typed API enabling rich intellisense and autocompletion
+- First-class [`pytest`](https://github.com/pytest-dev/pytest/) integration with detailed assertion explanations
 
 ### Toolchain
 
-> [Documentation](https://mcbeet.dev/toolchain/)
-
 ```python
 from beet import Context, Function
 
 def greet(ctx: Context):
     """Plugin that adds a function for greeting the player."""
     ctx.data["greet:hello"] = Function(["say hello"], tags=["minecraft:load"])
 ```
@@ -59,56 +84,60 @@
 The `beet` toolchain is designed to support a wide range of use-cases. The most basic pipeline will let you create configurable resource packs and data packs, but plugins make it easy to implement arbitrarily advanced workflows and tools like linters, asset generators and function pre-processors.
 
 - Compose plugins that can inspect and edit the generated resource pack and data pack
 - Configure powerful build systems for development and creating releases
 - First-class template integration approachable without prior Python knowledge
 - Link the generated resource pack and data pack to Minecraft
 - Automatically rebuild the project on file changes with watch mode
+- Batteries-included package that comes with a few handy plugins out of the box
+- Rich ecosystem, extensible CLI, and powerful generator and worker API
 
 ## Installation
 
 The package can be installed with `pip`.
 
 ```bash
 $ pip install beet
 ```
 
+To create and edit images programmatically you should install `beet` with the `image` extra or install `Pillow` separately.
+
+```bash
+$ pip install beet[image]
+$ pip install beet Pillow
+```
+
 You can make sure that `beet` was successfully installed by trying to use the toolchain from the command-line.
 
 ```bash
 $ beet --help
 Usage: beet [OPTIONS] COMMAND [ARGS]...
 
   The beet toolchain.
 
 Options:
-  -d, --directory DIRECTORY  Use the specified project directory.
-  -c, --config FILE          Use the specified config file.
-  -v, --version              Show the version and exit.
-  -h, --help                 Show this message and exit.
+  -p, --project PATH  Select project.
+  -s, --set OPTION    Set config option.
+  -l, --log LEVEL     Configure output verbosity.
+  -v, --version       Show the version and exit.
+  -h, --help          Show this message and exit.
 
 Commands:
   build  Build the current project.
   cache  Inspect or clear the cache.
   link   Link the generated resource pack and data pack to Minecraft.
   watch  Watch the project directory and build on file changes.
 ```
 
-## Status
-
-You can expect current releases to be pretty stable, but the project as a whole should still be considered alpha.
-
-The main reason is that resource pack and data pack coverage is currently lacking in certain areas. Exposing a consistent interface for every data pack and resource pack feature can involve design decisions that aren't immediately obvious. You're welcome to open an issue to discuss the implementation of currently unsupported resources. And feel free to ask questions, report bugs, and share your thoughts and impressions.
-
 ## Contributing
 
 Contributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org).
 
 ```bash
-$ poetry install
+$ poetry install --extras image
 ```
 
 You can run the tests with `poetry run pytest`. We use [`pytest-minecraft`](https://github.com/vberlier/pytest-minecraft) to run tests against actual Minecraft releases.
 
 ```bash
 $ poetry run pytest
 $ poetry run pytest --minecraft-latest
@@ -134,7 +163,8 @@
 $ poetry run black beet tests
 $ poetry run black --check beet tests
 ```
 
 ---
 
 License - [MIT](https://github.com/mcbeet/beet/blob/main/LICENSE)
+
```

### Comparing `beet-0.9.4/beet/contrib/inline_function_tag.py` & `beet-0.90.0/beet/contrib/inline_function_tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,43 +2,39 @@
 
 
 __all__ = [
     "InlineFunctionTags",
 ]
 
 
-from typing import Any
+from typing import Any, List
 
-from jinja2.ext import Extension
-from jinja2.nodes import DerivedContextReference  # type: ignore
 from jinja2.nodes import ExprStmt, Node
 
-from beet import Context, FunctionTag
-from beet.core.utils import JsonDict
+from beet import Context, FunctionTag, JinjaExtension
 
 
 def beet_default(ctx: Context):
     ctx.template.env.add_extension(InlineFunctionTags)
 
 
-class InlineFunctionTags(Extension):
+class InlineFunctionTags(JinjaExtension):
     """A Jinja extension that allows you to declare function tags inline."""
 
     tags = {"tag"}
 
     def parse(self, parser: Any) -> Node:
         lineno = next(parser.stream).lineno
+        args: List[Any] = [parser.parse_expression()]
 
-        args = [DerivedContextReference(), parser.parse_expression()]
-
-        handler = self.call_method("_function_tag_handler", args, lineno=lineno)
-        return ExprStmt(handler, lineno=lineno)
-
-    def _function_tag_handler(self, context: Any, function_tag: str):
-        ctx: Context = context["ctx"]
+        return ExprStmt(
+            self.call_method("_function_tag_handler", args, lineno=lineno),
+            lineno=lineno,
+        )
 
-        if ctx.meta["render_group"] != "functions":
+    def _function_tag_handler(self, function_tag: str):
+        if self.ctx.meta["render_group"] != "functions":
             raise TypeError("Inline tags can only be used inside functions.")
 
-        ctx.data.function_tags.merge(
-            {function_tag: FunctionTag({"values": [ctx.meta["render_path"]]})}
+        self.ctx.data.function_tags.merge(
+            {function_tag: FunctionTag({"values": [self.ctx.meta["render_path"]]})}
         )
```

### Comparing `beet-0.9.4/beet/contrib/lantern_load.py` & `beet-0.90.0/beet/contrib/lantern_load.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """Plugin that implements Lantern Load runtime dependencies."""
 
 
-from typing import Any, Dict, List
+from typing import cast
 
 from beet import Context, Function, FunctionTag
+from beet.core.utils import JsonDict
 
 
 def beet_default(ctx: Context):
     # Add the necessary boilerplate to the data pack.
     # This could also be done by merging a base data pack embedded inside the package.
     ctx.require(base_data_pack)
 
     # Grab the Lantern Load configuration.
     # The id defaults to the project name and the version to the project version.
-    config = ctx.meta.get("lantern_load", {})
+    config = ctx.meta.get("lantern_load", cast(JsonDict, {}))
 
-    id = config.get("id", ctx.project_name)
+    id = config.get("id", ctx.project_id)
     version = config.get("version", ctx.project_version)
-    dependencies = config.get("dependencies", {})
+    dependencies = config.get("dependencies", cast(JsonDict, {}))
 
     # Populate the #load:load tag with the dependencies followed by the pack's
     # own load function.
     load_tag_values = [
         *({"id": f"#{dep}:load", "required": False} for dep in dependencies),
         f"{id}:load",
     ]
 
-    ctx.data.function_tags["load:load"].data["values"].append(f"#{id}:load")
+    ctx.data.function_tags.setdefault("load:load", FunctionTag()).add(f"#{id}:load")
     ctx.data[f"{id}:load"] = FunctionTag({"values": load_tag_values})
 
     # Generate and join version checks for all the dependencies.
     # Currently this only matches a major version number against a fixed value or a range.
     version_checks = " ".join(
         f"if score {dep}.major load.status matches {version}"
         for dep, version in dependencies.items()
@@ -68,15 +69,7 @@
     ctx.data["load:_private/init"] = FunctionTag({"values": ["load:_private/init"]})
     ctx.data["load:_private/init"] = Function(
         [
             "scoreboard objectives add load.status dummy",
             "scoreboard players reset * load.status",
         ]
     )
-
-    ctx.data.function_tags.merge(
-        {
-            "load:pre_load": FunctionTag({"values": []}),
-            "load:load": FunctionTag({"values": []}),
-            "load:post_load": FunctionTag({"values": []}),
-        }
-    )
```

### Comparing `beet-0.9.4/beet/core/cache.py` & `beet-0.90.0/beet/core/container.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,200 +1,224 @@
 __all__ = [
-    "MultiCache",
-    "Cache",
+    "SupportsMerge",
+    "MergeMixin",
+    "MatchMixin",
+    "Pin",
+    "PinDefault",
+    "PinDefaultFactory",
+    "Container",
+    "ContainerProxy",
+    "Drop",
 ]
 
 
-import json
-import shutil
-from datetime import datetime, timedelta
-from pathlib import Path
-from textwrap import indent
-from typing import Any, ClassVar, Iterator, Optional
-
-from .container import Container, MatchMixin
-from .utils import FileSystemPath, JsonDict, dump_json
-
-
-class Cache:
-    """An expiring filesystem cache that can store serialized json."""
-
-    deleted: bool
-    directory: Path
-    index_path: Path
-    index: JsonDict
-
-    index_file: ClassVar[str] = "index.json"
-
-    def __init__(self, directory: FileSystemPath):
-        self.deleted = False
-        self.directory = Path(directory).resolve()
-        self.index_path = self.directory / self.index_file
-        self.index = (
-            json.loads(self.index_path.read_text())
-            if self.index_path.is_file()
-            else self.get_initial_index()
-        )
-        self.flush()
-
-    def get_initial_index(self) -> JsonDict:
-        """Return the initial cache index."""
+from dataclasses import dataclass
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterator,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Protocol,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+from pathspec import PathSpec
+
+from .utils import SENTINEL_OBJ, Sentinel
+
+K = TypeVar("K")
+V = TypeVar("V")
+CV = TypeVar("CV", covariant=True)
+ProxyKeyType = TypeVar("ProxyKeyType")
+
+PinDefault = Union[V, Sentinel]
+PinDefaultFactory = Union[Callable[[], V], Sentinel]
+
+
+class Drop(Exception):
+    """Raised to signal that an item shouldn't be added to a container."""
+
+
+class SupportsMerge(Protocol):
+    """Protocol for detecting mergeable types."""
+
+    def merge(self, other: Any) -> bool:
+        ...
+
+
+class MergeMixin:
+    def merge(self, other: Mapping[Any, SupportsMerge]) -> bool:
+        """Merge values from the given dict-like object."""
+        for key, value in other.items():
+            try:
+                if key not in self or not self[key].merge(value):  # type: ignore
+                    self[key] = value  # type: ignore
+            except Drop:
+                del self[key]  # type: ignore
+        return True
+
+
+class MatchMixin:
+    def match(self, *patterns: str) -> Set[str]:
+        """Return keys matching the given path patterns."""
+        spec = PathSpec.from_lines("gitwildmatch", patterns)
+        return set(spec.match_files(self.keys()))  # type: ignore
+
+
+@dataclass
+class Pin(Generic[K, CV]):
+    """Descriptor that exposes a specific value from a dict-like object."""
+
+    key: K
+    default: PinDefault[CV] = SENTINEL_OBJ
+    default_factory: PinDefaultFactory[CV] = SENTINEL_OBJ
+
+    def __get__(self, obj: Any, objtype: Optional[Type[Any]] = None) -> CV:
+        mapping = self.forward(obj)
+
+        try:
+            return mapping[self.key]
+        except KeyError:
+            value = (
+                self.default
+                if isinstance(self.default_factory, Sentinel)
+                else self.default_factory()
+            )
+
+            if isinstance(value, Sentinel):
+                raise
+
+            mapping[self.key] = value
+            return self.__get__(obj, objtype)
+
+    def __set__(self: "Pin[K, V]", obj: Any, value: V):
+        self.forward(obj)[self.key] = value
+
+    def __delete__(self, obj: Any):
+        del self.forward(obj)[self.key]
+
+    def forward(self, obj: Any) -> Any:
+        """Return the dict-like object that contains the pinned value."""
+        return obj
+
+    @classmethod
+    def collect_from(
+        cls: Type["Pin[K, CV]"], target: Type[Any]
+    ) -> Dict[str, "Pin[K, CV]"]:
         return {
-            "timestamp": datetime.now().isoformat(),
-            "expire": None,
-            "json": {},
+            key: value for key, value in vars(target).items() if isinstance(value, cls)
         }
 
-    @property
-    def json(self) -> JsonDict:
-        return self.index["json"]
-
-    @json.setter
-    def json(self, value: JsonDict):
-        self.index["json"] = value
-
-    @property
-    def expire(self) -> Optional[datetime]:
-        expire = self.index["expire"]
-        return expire and datetime.fromisoformat(expire)
-
-    @expire.setter
-    def expire(self, value: Optional[datetime]):
-        self.index["expire"] = value and value.isoformat()
-
-    def timeout(self, delta: Optional[timedelta] = None, **kwargs: Any) -> "Cache":
-        """Invalidate the cache after a given timeout."""
-        if not delta:
-            delta = timedelta()
-        delta += timedelta(**kwargs)
-        self.expire = datetime.fromisoformat(self.index["timestamp"]) + delta
-        return self
-
-    def restart_timeout(self):
-        """Restart the invalidation timeout."""
-        now = datetime.now()
-        timestamp = datetime.fromisoformat(self.index["timestamp"])
-
-        if self.expire:
-            self.expire += now - timestamp
-
-        self.index["timestamp"] = now.isoformat()
-
-    def __enter__(self) -> "Cache":
-        return self
-
-    def __exit__(self, *_):
-        self.flush()
-
-    def delete(self):
-        """Delete the entire cache."""
-        if not self.deleted:
-            if self.directory.is_dir():
-                shutil.rmtree(self.directory)
-            self.index = self.get_initial_index()
-            self.deleted = True
-
-    def clear(self):
-        """Clear the cache by deleting it and creating it again."""
-        self.delete()
-        self.deleted = False
-        self.flush()
-
-    def flush(self):
-        """Flush the modifications to the filesystem."""
-        if self.deleted:
-            return
-
-        if self.expire and self.expire <= datetime.now():
-            self.clear()
-        else:
-            self.directory.mkdir(parents=True, exist_ok=True)
-            self.index_path.write_text(dump_json(self.index))
+
+class Container(MutableMapping[K, V]):
+    """Generic dict-like container."""
+
+    _wrapped: Dict[K, V]
+
+    def __init__(self):
+        self._wrapped = {}
+
+    def __getitem__(self, key: K) -> V:
+        key = self.normalize_key(key)
+
+        try:
+            return self._wrapped[key]
+        except KeyError:
+            pass
+
+        value = self.missing(key)
+        self[key] = value
+        return value
+
+    def __setitem__(self, key: K, value: V):
+        key = self.normalize_key(key)
+
+        should_delete = False
+
+        try:
+            value = self.process(key, value)
+        except Drop:
+            should_delete = True
+
+        self._wrapped[key] = value
+
+        if should_delete:
+            del self[key]
+
+    def __delitem__(self, key: K):
+        key = self.normalize_key(key)
+        del self._wrapped[key]
+
+    def __iter__(self) -> Iterator[K]:
+        return iter(self._wrapped)
+
+    def __len__(self) -> int:
+        return len(self._wrapped)
+
+    def normalize_key(self, key: K) -> K:
+        """Normalize the key before accessing an item."""
+        return key
+
+    def process(self, key: K, value: V) -> V:
+        """Process the value before inserting it."""
+        return value
+
+    def missing(self, key: K) -> V:
+        """Recover missing item or raise a KeyError."""
+        raise KeyError(key)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({str(self.directory)!r})"
+        return f"{self.__class__.__name__}(keys={list(self.keys())})"
+
+
+class ContainerProxy(Generic[ProxyKeyType, K, V], MutableMapping[K, V]):
+    """Generic aggregated view over several nested bounded dict-like objects."""
 
-    def __str__(self) -> str:
-        formatted_json = indent(dump_json(self.json), "  │  ")[5:]
-        contents = indent("\n".join(self._format_directory()), "  │    ")
-
-        return (
-            f"Cache {self.index_path.parent.name}:\n"
-            f"  │  timestamp = {datetime.fromisoformat(self.index['timestamp']).ctime()}\n"
-            f"  │  expire = {self.expire and self.expire.ctime()}\n  │  \n"
-            f"  │  directory = {self.directory}\n{contents}\n  │  \n"
-            f"  │  json = {formatted_json}"
-        )
+    proxy: Mapping[K, Mapping[ProxyKeyType, MutableMapping[K, V]]]
+    proxy_key: ProxyKeyType
 
-    def _format_directory(
+    def __init__(
         self,
-        directory: Optional[FileSystemPath] = None,
-        prefix: str = "",
-    ) -> Iterator[str]:
-        entries = list(sorted(Path(directory or self.directory).iterdir()))
-        indents = ["├─"] * (len(entries) - 1) + ["└─"]
-
-        for indent, entry in zip(indents, entries):
-            yield f"{prefix}{indent} {entry.name}"
-
-            if entry.is_dir():
-                indent = "│  " if indent == "├─" else "   "
-                yield from self._format_directory(entry, prefix + indent)
-
-
-class MultiCache(MatchMixin, Container[str, Cache]):
-    """A container of lazily instantiated named caches."""
-
-    path: Path
-    default_cache: str
-
-    def __init__(self, directory: FileSystemPath, default_cache: str = "default"):
-        super().__init__()
-        self.path = Path(directory).resolve()
-        self.default_cache = default_cache
-
-    def missing(self, key: str) -> Cache:
-        cache = Cache(self.path / key)
-        self[key] = cache
-        return cache
-
-    def __delitem__(self, key: str):
-        self[key].delete()
-        super().__delitem__(key)
-
-    @property
-    def directory(self) -> Path:
-        return self[self.default_cache].directory
-
-    @property
-    def json(self) -> JsonDict:
-        return self[self.default_cache].json
-
-    def __enter__(self) -> "MultiCache":
-        return self
-
-    def __exit__(self, *_):
-        self.flush()
-
-    def preload(self):
-        """Preload all the named caches."""
-        if not self.path.is_dir():
-            return
-        for directory in self.path.iterdir():
-            if (directory / Cache.index_file).is_file():
-                assert self[directory.name]
-
-    def clear(self):
-        """Clear the entire cache."""
-        if self.path.is_dir():
-            shutil.rmtree(self.path)
-        super().clear()
-
-    def flush(self):
-        """Flush the modifications to the filesystem."""
-        for cache in self.values():
-            cache.flush()
-        if self.path.is_dir() and not (ignore := self.path / ".gitignore").is_file():
-            ignore.write_text("# Automatically created by beet\n*\n")
+        proxy: Mapping[K, Mapping[ProxyKeyType, MutableMapping[K, V]]],
+        proxy_key: ProxyKeyType,
+    ) -> None:
+        self.proxy = proxy
+        self.proxy_key = proxy_key
+
+    def __getitem__(self, key: K) -> V:
+        key1, key2 = self.split_key(key)
+        return self.proxy[key1][self.proxy_key][key2]
+
+    def __setitem__(self, key: K, value: V):
+        key1, key2 = self.split_key(key)
+        self.proxy[key1][self.proxy_key][key2] = value
+
+    def __delitem__(self, key: K):
+        key1, key2 = self.split_key(key)
+        del self.proxy[key1][self.proxy_key][key2]
+
+    def __iter__(self) -> Iterator[K]:
+        for key1, mapping in self.proxy.items():
+            for key2 in mapping[self.proxy_key]:
+                yield self.join_key(key1, key2)
+
+    def __len__(self) -> int:
+        return sum(len(mapping[self.proxy_key]) for mapping in self.proxy.values())
+
+    def split_key(self, key: K) -> Tuple[K, K]:
+        """Return the outer mapping key and the nested key."""
+        raise NotImplementedError()
+
+    def join_key(self, key1: K, key2: K) -> K:
+        """Combine the outer mapping key and the nested key."""
+        raise NotImplementedError()
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({str(self.path)!r})"
+        return f"{self.__class__.__name__}(keys={list(self.keys())})"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `beet-0.9.4/beet/core/watch.py` & `beet-0.90.0/beet/core/watch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __all__ = [
     "DirectoryWatcher",
     "FileChanges",
+    "detect_repeated_changes",
 ]
 
 
 import os
 import time
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Dict, Iterator, Literal, Optional, Sequence, Tuple, cast
+from typing import Dict, Iterable, Iterator, Literal, Optional, Sequence, Tuple, cast
 
 from pathspec import PathSpec
 
 from .utils import FileSystemPath, extra_field
 
 FileChanges = Dict[str, Literal["created", "edited", "removed"]]
 
@@ -34,15 +35,15 @@
         self.ignore_patterns = list(self.ignore_patterns)
 
         if self.ignore_file:
             ignore_file = Path(self.ignore_file)
 
             if ignore_file.parts == (ignore_file.name,):
                 for directory in Path(self.path, ignore_file).parents:
-                    if (path := (directory / ignore_file)).is_file():
+                    if (path := directory / ignore_file).is_file():
                         ignore_file = path
                         break
 
             if ignore_file.is_file():
                 self.ignore_patterns += [
                     pattern
                     for line in ignore_file.read_text().splitlines()
@@ -93,7 +94,29 @@
             if self.ignore.match_file(relative_path):
                 continue
 
             if entry_path.is_dir():
                 yield from self.walk(relative_path)
             else:
                 yield str(relative_path), entry.stat().st_mtime
+
+
+def detect_repeated_changes(
+    source: Iterable[FileChanges],
+    min_interval: float = 1.2,
+    max_streak: int = 3,
+) -> Iterator[Tuple[bool, FileChanges]]:
+    """Detect repeated changes."""
+    streak: int = 0
+    last_build: float = 0.0
+    last_changes: FileChanges = {}
+
+    for changes in source:
+        if time.time() - last_build < min_interval and changes == last_changes:
+            streak += 1
+        else:
+            streak = 0
+
+        yield streak > max_streak, changes
+
+        last_build = time.time()
+        last_changes = changes
```

### Comparing `beet-0.9.4/beet/library/data_pack.py` & `beet-0.90.0/beet/library/data_pack.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,318 +1,360 @@
 __all__ = [
     "DataPack",
     "DataPackNamespace",
     "Advancement",
+    "DamageType",
+    "ChatType",
     "Function",
+    "ItemModifier",
     "LootTable",
     "Predicate",
     "Recipe",
     "Structure",
+    "TrimPattern",
+    "TrimMaterial",
     "TagFile",
     "BlockTag",
     "EntityTypeTag",
     "FluidTag",
     "FunctionTag",
+    "GameEventTag",
     "ItemTag",
-    "DimensionType",
-    "Dimension",
-    "Biome",
-    "ConfiguredCarver",
-    "ConfiguredFeature",
-    "ConfiguredStructureFeature",
-    "ConfiguredSurfaceBuilder",
-    "NoiseSettings",
-    "ProcessorList",
-    "TemplatePool",
-    "ItemModifier",
 ]
 
 
 import io
 from copy import deepcopy
 from dataclasses import dataclass
 from gzip import GzipFile
-from typing import MutableSequence, Optional, TypeVar
+from typing import ClassVar, Iterable, List, Optional, Tuple, TypeVar, Union
 
 from nbtlib.contrib.minecraft import StructureFile, StructureFileData
 
 from beet.core.file import (
     BinaryFileBase,
     BinaryFileContent,
     FileDeserialize,
     JsonFile,
     TextFileBase,
     TextFileContent,
 )
-from beet.core.utils import extra_field
+from beet.core.utils import JsonDict, extra_field, split_version
 
-from .base import Namespace, NamespaceFile, NamespacePin, NamespaceProxyDescriptor, Pack
+from .base import (
+    LATEST_MINECRAFT_VERSION,
+    Namespace,
+    NamespacePin,
+    NamespaceProxyDescriptor,
+    Pack,
+)
 
 TagFileType = TypeVar("TagFileType", bound="TagFile")
 
 
-class Advancement(JsonFile, NamespaceFile):
+class Advancement(JsonFile):
     """Class representing an advancement."""
 
-    scope = ("advancements",)
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("advancements",)
+    extension: ClassVar[str] = ".json"
 
 
-@dataclass(eq=False)
-class Function(TextFileBase[MutableSequence[str]], NamespaceFile):
-    """Class representing a function."""
+class DamageType(JsonFile):
+    """Class representing a damage type."""
+
+    scope: ClassVar[Tuple[str, ...]] = ("damage_type",)
+    extension: ClassVar[str] = ".json"
 
-    content: TextFileContent[MutableSequence[str]] = None
-    tags: Optional[MutableSequence[str]] = extra_field(default=None)
 
-    scope = ("functions",)
-    extension = ".mcfunction"
+class ChatType(JsonFile):
+    """Class representing a chat type."""
+
+    scope: ClassVar[Tuple[str, ...]] = ("chat_type",)
+    extension: ClassVar[str] = ".json"
+
+
+@dataclass(eq=False, repr=False)
+class Function(TextFileBase[List[str]]):
+    """Class representing a function."""
 
-    lines = FileDeserialize()  # type: FileDeserialize[MutableSequence[str]]
+    content: TextFileContent[List[str]] = None
+    tags: Optional[List[str]] = extra_field(default=None)
+    prepend_tags: Optional[List[str]] = extra_field(default=None)
+
+    scope: ClassVar[Tuple[str, ...]] = ("functions",)
+    extension: ClassVar[str] = ".mcfunction"
+
+    lines: ClassVar[FileDeserialize[List[str]]] = FileDeserialize()
+
+    def append(self, other: Union["Function", Iterable[str], str]):
+        """Append lines from another function."""
+        self.lines.extend(
+            other.lines
+            if isinstance(other, Function)
+            else [other]
+            if isinstance(other, str)
+            else other
+        )
+
+    def prepend(self, other: Union["Function", Iterable[str], str]):
+        """Prepend lines from another function."""
+        self.lines[0:0] = (
+            other.lines
+            if isinstance(other, Function)
+            else [other]
+            if isinstance(other, str)
+            else other
+        )
 
     @classmethod
-    def to_str(cls, content: MutableSequence[str]) -> str:
+    def default(cls) -> List[str]:
+        return []
+
+    def to_str(self, content: List[str]) -> str:
         return "\n".join(content) + "\n"
 
-    @classmethod
-    def from_str(cls, content: str) -> MutableSequence[str]:
+    def from_str(self, content: str) -> List[str]:
         return content.splitlines()
 
-    def bind(self, pack: "DataPack", namespace: str, path: str):
-        super().bind(pack, namespace, path)
+    def bind(self, pack: "DataPack", path: str):
+        super().bind(pack, path)
 
         for tag_name in self.tags or ():
-            pack.function_tags.merge(
-                {tag_name: FunctionTag({"values": [f"{namespace}:{path}"]})}
-            )
+            pack.function_tags.merge({tag_name: FunctionTag({"values": [path]})})
+
+        for tag_name in self.prepend_tags or ():
+            function_tag = pack.function_tags.setdefault(tag_name, FunctionTag())
+            function_tag.prepend(FunctionTag({"values": [path]}))
 
 
-class LootTable(JsonFile, NamespaceFile):
+class ItemModifier(JsonFile):
+    """Class representing an item modifier."""
+
+    scope: ClassVar[Tuple[str, ...]] = ("item_modifiers",)
+    extension: ClassVar[str] = ".json"
+
+
+class LootTable(JsonFile):
     """Class representing a loot table."""
 
-    scope = ("loot_tables",)
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("loot_tables",)
+    extension: ClassVar[str] = ".json"
 
 
-class Predicate(JsonFile, NamespaceFile):
+class Predicate(JsonFile):
     """Class representing a predicate."""
 
-    scope = ("predicates",)
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("predicates",)
+    extension: ClassVar[str] = ".json"
 
 
-class Recipe(JsonFile, NamespaceFile):
+class Recipe(JsonFile):
     """Class representing a recipe."""
 
-    scope = ("recipes",)
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("recipes",)
+    extension: ClassVar[str] = ".json"
 
 
-@dataclass(eq=False)
-class Structure(BinaryFileBase[StructureFileData], NamespaceFile):
+@dataclass(eq=False, repr=False)
+class Structure(BinaryFileBase[StructureFileData]):
     """Class representing a structure file."""
 
     content: BinaryFileContent[StructureFileData] = None
 
-    scope = ("structures",)
-    extension = ".nbt"
+    scope: ClassVar[Tuple[str, ...]] = ("structures",)
+    extension: ClassVar[str] = ".nbt"
 
-    data = FileDeserialize()  # type: FileDeserialize[StructureFileData]
+    data: ClassVar[FileDeserialize[StructureFileData]] = FileDeserialize()
 
-    @classmethod
-    def from_bytes(cls, content: bytes) -> StructureFileData:
+    def from_bytes(self, content: bytes) -> StructureFileData:
         with GzipFile(fileobj=io.BytesIO(content)) as fileobj:
             return StructureFile.parse(fileobj).root
 
-    @classmethod
-    def to_bytes(cls, content: StructureFileData) -> bytes:
+    def to_bytes(self, content: StructureFileData) -> bytes:
         dst = io.BytesIO()
         with GzipFile(fileobj=dst, mode="wb") as fileobj:
             StructureFile(content).write(fileobj)
         return dst.getvalue()
 
 
-class TagFile(JsonFile, NamespaceFile):
+class TrimPattern(JsonFile):
+    """Class representing a trim pattern."""
+
+    scope: ClassVar[Tuple[str, ...]] = ("trim_pattern",)
+    extension: ClassVar[str] = ".json"
+
+
+class TrimMaterial(JsonFile):
+    """Class representing a trim material."""
+
+    scope: ClassVar[Tuple[str, ...]] = ("trim_material",)
+    extension: ClassVar[str] = ".json"
+
+
+class TagFile(JsonFile):
     """Base class for tag files."""
 
-    extension = ".json"
+    extension: ClassVar[str] = ".json"
 
     def merge(self: TagFileType, other: TagFileType) -> bool:  # type: ignore
         if other.data.get("replace"):
             self.data["replace"] = True
+            self.data["values"] = deepcopy(other.data.get("values", []))
+            return True
 
         values = self.data.setdefault("values", [])
 
         for value in other.data.get("values", []):
             if value not in values:
                 values.append(deepcopy(value))
         return True
 
+    def append(self: TagFileType, other: TagFileType):
+        """Append values from another tag."""
+        self.merge(other)
+
+    def prepend(self: TagFileType, other: TagFileType):
+        """Prepend values from another tag."""
+        if other.data.get("replace"):
+            self.data["replace"] = True
+            self.data["values"] = deepcopy(other.data.get("values", []))
+            return
+
+        values = self.data.setdefault("values", [])
+
+        for value in other.data.get("values", []):
+            if value not in values:
+                values.insert(0, deepcopy(value))
+
+    def add(self, value: str):
+        """Add an entry."""
+        values = self.data.setdefault("values", [])
+        if value not in values:
+            values.append(value)
+
+    def remove(self, value: str):
+        """Remove an entry."""
+        values = self.data.setdefault("values", [])
+        try:
+            values.remove(value)
+        except ValueError:
+            pass
+
+    @classmethod
+    def default(cls) -> JsonDict:
+        return {"values": []}
+
 
 class BlockTag(TagFile):
     """Class representing a block tag."""
 
-    scope = ("tags", "blocks")
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "blocks")
 
 
 class EntityTypeTag(TagFile):
     """Class representing an entity tag."""
 
-    scope = ("tags", "entity_types")
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "entity_types")
 
 
 class FluidTag(TagFile):
     """Class representing a fluid tag."""
 
-    scope = ("tags", "fluids")
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "fluids")
 
 
 class FunctionTag(TagFile):
     """Class representing a function tag."""
 
-    scope = ("tags", "functions")
-
-
-class ItemTag(TagFile):
-    """Class representing an item tag."""
-
-    scope = ("tags", "items")
-
-
-class DimensionType(JsonFile, NamespaceFile):
-    """Class representing a dimension type."""
-
-    scope = ("dimension_type",)
-    extension = ".json"
-
-
-class Dimension(JsonFile, NamespaceFile):
-    """Class representing a dimension."""
-
-    scope = ("dimension",)
-    extension = ".json"
-
-
-class Biome(JsonFile, NamespaceFile):
-    """Class representing a biome."""
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "functions")
 
-    scope = ("worldgen", "biome")
-    extension = ".json"
 
+class GameEventTag(TagFile):
+    """Class representing a game event tag."""
 
-class ConfiguredCarver(JsonFile, NamespaceFile):
-    """Class representing a worldgen carver."""
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "game_events")
 
-    scope = ("worldgen", "configured_carver")
-    extension = ".json"
 
+class ItemTag(TagFile):
+    """Class representing an item tag."""
 
-class ConfiguredFeature(JsonFile, NamespaceFile):
-    """Class representing a worldgen feature."""
-
-    scope = ("worldgen", "configured_feature")
-    extension = ".json"
-
-
-class ConfiguredStructureFeature(JsonFile, NamespaceFile):
-    """Class representing a worldgen structure feature."""
-
-    scope = ("worldgen", "configured_structure_feature")
-    extension = ".json"
-
-
-class ConfiguredSurfaceBuilder(JsonFile, NamespaceFile):
-    """Class representing a worldgen surface builder."""
-
-    scope = ("worldgen", "configured_surface_builder")
-    extension = ".json"
-
-
-class NoiseSettings(JsonFile, NamespaceFile):
-    """Class representing worldgen noise settings."""
-
-    scope = ("worldgen", "noise_settings")
-    extension = ".json"
-
-
-class ProcessorList(JsonFile, NamespaceFile):
-    """Class representing a worldgen processor list."""
-
-    scope = ("worldgen", "processor_list")
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "items")
 
 
-class TemplatePool(JsonFile, NamespaceFile):
-    """Class representing a worldgen template pool."""
+class ChatTypeTag(TagFile):
+    """Class representing a chat type tag."""
 
-    scope = ("worldgen", "template_pool")
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "chat_type")
 
 
-class ItemModifier(JsonFile, NamespaceFile):
-    """Class representing an item modifier."""
+class DamageTypeTag(TagFile):
+    """Class representing a damage type tag."""
 
-    scope = ("item_modifiers",)
-    extension = ".json"
+    scope: ClassVar[Tuple[str, ...]] = ("tags", "damage_type")
 
 
 class DataPackNamespace(Namespace):
     """Class representing a data pack namespace."""
 
     directory = "data"
 
     # fmt: off
-    advancements:                  NamespacePin[Advancement]                = NamespacePin(Advancement)
-    functions:                     NamespacePin[Function]                   = NamespacePin(Function)
-    loot_tables:                   NamespacePin[LootTable]                  = NamespacePin(LootTable)
-    predicates:                    NamespacePin[Predicate]                  = NamespacePin(Predicate)
-    recipes:                       NamespacePin[Recipe]                     = NamespacePin(Recipe)
-    structures:                    NamespacePin[Structure]                  = NamespacePin(Structure)
-    block_tags:                    NamespacePin[BlockTag]                   = NamespacePin(BlockTag)
-    entity_type_tags:              NamespacePin[EntityTypeTag]              = NamespacePin(EntityTypeTag)
-    fluid_tags:                    NamespacePin[FluidTag]                   = NamespacePin(FluidTag)
-    function_tags:                 NamespacePin[FunctionTag]                = NamespacePin(FunctionTag)
-    item_tags:                     NamespacePin[ItemTag]                    = NamespacePin(ItemTag)
-    dimension_types:               NamespacePin[DimensionType]              = NamespacePin(DimensionType)
-    dimensions:                    NamespacePin[Dimension]                  = NamespacePin(Dimension)
-    biomes:                        NamespacePin[Biome]                      = NamespacePin(Biome)
-    configured_carvers:            NamespacePin[ConfiguredCarver]           = NamespacePin(ConfiguredCarver)
-    configured_features:           NamespacePin[ConfiguredFeature]          = NamespacePin(ConfiguredFeature)
-    configured_structure_features: NamespacePin[ConfiguredStructureFeature] = NamespacePin(ConfiguredStructureFeature)
-    configured_surface_builders:   NamespacePin[ConfiguredSurfaceBuilder]   = NamespacePin(ConfiguredSurfaceBuilder)
-    noise_settings:                NamespacePin[NoiseSettings]              = NamespacePin(NoiseSettings)
-    processor_lists:               NamespacePin[ProcessorList]              = NamespacePin(ProcessorList)
-    template_pools:                NamespacePin[TemplatePool]               = NamespacePin(TemplatePool)
-    item_modifiers:                NamespacePin[ItemModifier]               = NamespacePin(ItemModifier)
+    advancements:     NamespacePin[Advancement]   = NamespacePin(Advancement)
+    functions:        NamespacePin[Function]      = NamespacePin(Function)
+    item_modifiers:   NamespacePin[ItemModifier]  = NamespacePin(ItemModifier)
+    loot_tables:      NamespacePin[LootTable]     = NamespacePin(LootTable)
+    predicates:       NamespacePin[Predicate]     = NamespacePin(Predicate)
+    recipes:          NamespacePin[Recipe]        = NamespacePin(Recipe)
+    trim_pattern:     NamespacePin[TrimPattern]   = NamespacePin(TrimPattern)
+    trim_material:    NamespacePin[TrimMaterial]  = NamespacePin(TrimMaterial)
+    structures:       NamespacePin[Structure]     = NamespacePin(Structure)
+    chat_type:        NamespacePin[ChatType]      = NamespacePin(ChatType)
+    damage_type:      NamespacePin[DamageType]    = NamespacePin(DamageType)
+    block_tags:       NamespacePin[BlockTag]      = NamespacePin(BlockTag)
+    entity_type_tags: NamespacePin[EntityTypeTag] = NamespacePin(EntityTypeTag)
+    fluid_tags:       NamespacePin[FluidTag]      = NamespacePin(FluidTag)
+    function_tags:    NamespacePin[FunctionTag]   = NamespacePin(FunctionTag)
+    game_event_tags:  NamespacePin[GameEventTag]  = NamespacePin(GameEventTag)
+    item_tags:        NamespacePin[ItemTag]       = NamespacePin(ItemTag)
+    chat_type_tags:   NamespacePin[ChatTypeTag]   = NamespacePin(ChatTypeTag)
+    damage_type_tags: NamespacePin[DamageTypeTag] = NamespacePin(DamageTypeTag)
     # fmt: on
 
 
 class DataPack(Pack[DataPackNamespace]):
     """Class representing a data pack."""
 
     default_name = "untitled_data_pack"
-    latest_pack_format = 6
+
+    pack_format_registry = {
+        (1, 13): 4,
+        (1, 14): 4,
+        (1, 15): 5,
+        (1, 16): 6,
+        (1, 17): 7,
+        (1, 18): 9,
+        (1, 19): 12,
+        (1, 20): 15,
+    }
+    latest_pack_format = pack_format_registry[split_version(LATEST_MINECRAFT_VERSION)]
 
     # fmt: off
-    advancements:                  NamespaceProxyDescriptor[Advancement]                = NamespaceProxyDescriptor(Advancement)
-    functions:                     NamespaceProxyDescriptor[Function]                   = NamespaceProxyDescriptor(Function)
-    loot_tables:                   NamespaceProxyDescriptor[LootTable]                  = NamespaceProxyDescriptor(LootTable)
-    predicates:                    NamespaceProxyDescriptor[Predicate]                  = NamespaceProxyDescriptor(Predicate)
-    recipes:                       NamespaceProxyDescriptor[Recipe]                     = NamespaceProxyDescriptor(Recipe)
-    structures:                    NamespaceProxyDescriptor[Structure]                  = NamespaceProxyDescriptor(Structure)
-    block_tags:                    NamespaceProxyDescriptor[BlockTag]                   = NamespaceProxyDescriptor(BlockTag)
-    entity_type_tags:              NamespaceProxyDescriptor[EntityTypeTag]              = NamespaceProxyDescriptor(EntityTypeTag)
-    fluid_tags:                    NamespaceProxyDescriptor[FluidTag]                   = NamespaceProxyDescriptor(FluidTag)
-    function_tags:                 NamespaceProxyDescriptor[FunctionTag]                = NamespaceProxyDescriptor(FunctionTag)
-    item_tags:                     NamespaceProxyDescriptor[ItemTag]                    = NamespaceProxyDescriptor(ItemTag)
-    dimension_types:               NamespaceProxyDescriptor[DimensionType]              = NamespaceProxyDescriptor(DimensionType)
-    dimensions:                    NamespaceProxyDescriptor[Dimension]                  = NamespaceProxyDescriptor(Dimension)
-    biomes:                        NamespaceProxyDescriptor[Biome]                      = NamespaceProxyDescriptor(Biome)
-    configured_carvers:            NamespaceProxyDescriptor[ConfiguredCarver]           = NamespaceProxyDescriptor(ConfiguredCarver)
-    configured_features:           NamespaceProxyDescriptor[ConfiguredFeature]          = NamespaceProxyDescriptor(ConfiguredFeature)
-    configured_structure_features: NamespaceProxyDescriptor[ConfiguredStructureFeature] = NamespaceProxyDescriptor(ConfiguredStructureFeature)
-    configured_surface_builders:   NamespaceProxyDescriptor[ConfiguredSurfaceBuilder]   = NamespaceProxyDescriptor(ConfiguredSurfaceBuilder)
-    noise_settings:                NamespaceProxyDescriptor[NoiseSettings]              = NamespaceProxyDescriptor(NoiseSettings)
-    processor_lists:               NamespaceProxyDescriptor[ProcessorList]              = NamespaceProxyDescriptor(ProcessorList)
-    template_pools:                NamespaceProxyDescriptor[TemplatePool]               = NamespaceProxyDescriptor(TemplatePool)
-    item_modifiers:                NamespaceProxyDescriptor[ItemModifier]               = NamespaceProxyDescriptor(ItemModifier)
+    advancements:     NamespaceProxyDescriptor[Advancement]   = NamespaceProxyDescriptor(Advancement)
+    functions:        NamespaceProxyDescriptor[Function]      = NamespaceProxyDescriptor(Function)
+    item_modifiers:   NamespaceProxyDescriptor[ItemModifier]  = NamespaceProxyDescriptor(ItemModifier)
+    loot_tables:      NamespaceProxyDescriptor[LootTable]     = NamespaceProxyDescriptor(LootTable)
+    predicates:       NamespaceProxyDescriptor[Predicate]     = NamespaceProxyDescriptor(Predicate)
+    recipes:          NamespaceProxyDescriptor[Recipe]        = NamespaceProxyDescriptor(Recipe)
+    trim_pattern:     NamespaceProxyDescriptor[TrimPattern]   = NamespaceProxyDescriptor(TrimPattern)
+    trim_material:    NamespaceProxyDescriptor[TrimMaterial]  = NamespaceProxyDescriptor(TrimMaterial)
+    structures:       NamespaceProxyDescriptor[Structure]     = NamespaceProxyDescriptor(Structure)
+    chat_type:        NamespaceProxyDescriptor[ChatType]      = NamespaceProxyDescriptor(ChatType)
+    damage_type:      NamespaceProxyDescriptor[DamageType]    = NamespaceProxyDescriptor(DamageType)
+    block_tags:       NamespaceProxyDescriptor[BlockTag]      = NamespaceProxyDescriptor(BlockTag)
+    entity_type_tags: NamespaceProxyDescriptor[EntityTypeTag] = NamespaceProxyDescriptor(EntityTypeTag)
+    fluid_tags:       NamespaceProxyDescriptor[FluidTag]      = NamespaceProxyDescriptor(FluidTag)
+    function_tags:    NamespaceProxyDescriptor[FunctionTag]   = NamespaceProxyDescriptor(FunctionTag)
+    game_event_tags:  NamespaceProxyDescriptor[GameEventTag]  = NamespaceProxyDescriptor(GameEventTag)
+    item_tags:        NamespaceProxyDescriptor[ItemTag]       = NamespaceProxyDescriptor(ItemTag)
+    chat_type_tags:   NamespaceProxyDescriptor[ChatTypeTag]   = NamespaceProxyDescriptor(ChatTypeTag)
+    damage_type_tags: NamespaceProxyDescriptor[DamageTypeTag] = NamespaceProxyDescriptor(DamageTypeTag)
     # fmt: on
```

### Comparing `beet-0.9.4/beet/toolchain/cli.py` & `beet-0.90.0/beet/toolchain/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,248 +1,283 @@
 __all__ = [
+    "MainGroup",
+    "BeetHelpColorsMixin",
+    "BeetCommand",
+    "BeetGroup",
+    "LogHandler",
     "main",
     "beet",
+    "format_error",
+    "error_handler",
+    "message_fence",
 ]
 
 
-import time
+import logging
 from contextlib import contextmanager
-from typing import Any, Optional, Sequence, TypeVar
+from importlib.metadata import entry_points
+from typing import Any, Callable, Iterator, List, Optional
 
 import click
-from click.decorators import pass_context
-from click_help_colors import HelpColorsGroup
+from click_help_colors import HelpColorsCommand, HelpColorsGroup
 
 from beet import __version__
+from beet.core.error import BeetException, WrappedException
+from beet.core.utils import format_exc
 
-from .pipeline import FormattedPipelineException
 from .project import Project
-from .utils import format_exc
-
-T = TypeVar("T")
-
-pass_project = click.make_pass_decorator(Project, ensure=True)
-
-
-class CustomGroup(HelpColorsGroup):
-    def __init__(self, *args: Any, **kwargs: Any):
-        super().__init__(
-            *args,
-            **kwargs,
-            invoke_without_command=True,
-            context_settings={"help_option_names": ("-h", "--help")},
-            help_headers_color="red",
-            help_options_color="green",
-        )
-
-    def get_command(self, ctx: click.Context, cmd_name: str) -> Optional[click.Command]:
-        if command := super().get_command(ctx, cmd_name):
-            return command
-
-        matches = [cmd for cmd in self.list_commands(ctx) if cmd.startswith(cmd_name)]
-
-        if len(matches) > 1:
-            match_list = ", ".join(sorted(matches))
-            ctx.fail(f"Ambiguous shorthand {cmd_name!r} ({match_list}).")
-        elif matches:
-            return super().get_command(ctx, matches[0])
-
-        return None
-
-    def format_usage(self, ctx: click.Context, formatter: Any):
-        formatter.write_usage(
-            ctx.command_path,
-            " ".join(self.collect_usage_pieces(ctx)),
-            click.style("Usage", fg="red") + ": ",
-        )
-
-
-@click.group(cls=CustomGroup)
-@pass_project
-@pass_context
-@click.option(
-    "-d",
-    "--directory",
-    type=click.Path(exists=True, file_okay=False),
-    help="Use the specified project directory.",
-)
-@click.option(
-    "-c",
-    "--config",
-    type=click.Path(exists=True, dir_okay=False),
-    help="Use the specified config file.",
-)
-@click.version_option(
-    __version__,
-    "-v",
-    "--version",
-    message=click.style("%(prog)s", fg="red")
-    + click.style(" v%(version)s", fg="green"),
-)
-def beet(
-    ctx: click.Context,
-    project: Project,
-    directory: Optional[str],
-    config: Optional[str],
-):
-    """The beet toolchain."""
-    if config:
-        project.config_path = config
-    elif directory:
-        project.config_directory = directory
-
-    if not ctx.invoked_subcommand:
-        ctx.invoke(build)  # type: ignore
 
 
 def format_error(
-    message: str, exception: Optional[BaseException] = None, padding: int = 0
+    message: str,
+    exception: Optional[BaseException] = None,
+    padding: int = 0,
 ) -> str:
+    """Format a given error message and exception."""
     output = "\n" * padding
     output += click.style("Error: " + message, fg="red", bold=True) + "\n"
     if exception:
         output += "\n" + format_exc(exception)
     output += "\n" * padding
     return output
 
 
 @contextmanager
-def error_handler(should_exit: bool = False, format_padding: int = 0):
+def error_handler(should_exit: bool = False, format_padding: int = 0) -> Iterator[None]:
+    """Context manager that catches and displays exceptions."""
     exception = None
 
     try:
         yield
-    except FormattedPipelineException as exc:
-        message, exception = exc.message, exc.__cause__ if exc.format_cause else None
+    except WrappedException as exc:
+        message = str(exc)
+        if not exc.hide_wrapped_exception:
+            exception = exc.__cause__
+    except BeetException as exc:
+        message = str(exc)
     except (click.Abort, KeyboardInterrupt):
         click.echo()
         message = "Aborted."
+    except (click.ClickException, click.exceptions.Exit):
+        raise
     except Exception as exc:
         message = "An unhandled exception occurred. This could be a bug."
         exception = exc
     else:
         return
 
+    if LogHandler.has_output and not format_padding:
+        click.echo()
+
     click.echo(format_error(message, exception, format_padding), nl=False)
 
     if should_exit:
         raise click.exceptions.Exit(1)
 
 
 @contextmanager
-def message_fence(message: str):
-    click.secho(message + "\n", fg="red")  # type: ignore
+def message_fence(message: str) -> Iterator[None]:
+    """Context manager used to report the begining and the end of a cli operation."""
+    click.secho(message + "\n", fg="red")
     yield
-    click.secho("Done!", fg="green", bold=True)  # type: ignore
+    if LogHandler.has_output:
+        click.echo()
+    click.secho("Done!", fg="green", bold=True)
+    LogHandler.has_output = False
 
 
-def command(func: T) -> T:
-    return beet.command()(pass_project(error_handler(should_exit=True)(func)))  # type: ignore
+class LogHandler(logging.Handler):
+    """Logging handler for the beet cli."""
 
+    style: Any = {
+        "CRITICAL": {"fg": "red", "bold": True},
+        "ERROR": {"fg": "red", "bold": True},
+        "WARNING": {"fg": "yellow", "bold": True},
+        "INFO": {},
+        "DEBUG": {"fg": "magenta"},
+    }
+
+    abbreviations: Any = {
+        "CRITICAL": "CRIT",
+        "WARNING": "WARN",
+    }
+
+    has_output: bool = False
+
+    def __init__(self):
+        super().__init__()
+        self.setFormatter(logging.Formatter("%(message)s"))
+
+    def emit(self, record: logging.LogRecord):
+        LogHandler.has_output = True
+        level = self.abbreviations.get(record.levelname, record.levelname)
+        style = self.style[record.levelname]
+
+        line_prefix = click.style(f"       |", **style)
+
+        leading_line, *lines = self.format(record).splitlines()
+        if record.levelname in ["ERROR", "CRITICAL"]:
+            leading_line = click.style(leading_line, **style)
+
+        leading_line = (
+            click.style(getattr(record, "prefix", record.name), bold=True, fg="black")
+            + "  "
+            + leading_line
+        )
 
-@command
-@click.option(
-    "-l",
-    "--link",
-    metavar="TARGET",
-    help="Link the project before building.",
-)
-def build(project: Project, link: Optional[str]):
-    """Build the current project."""
-    text = "Linking and building project..." if link else "Building project..."
-    with message_fence(text):
-        if link:
-            click.echo("\n".join(project.link(target=link)))
-        project.build()
+        click.echo(click.style(f"{level:<7}|", **style) + " " + leading_line)
 
+        if annotate := getattr(record, "annotate", None):
+            lines.insert(0, click.style(str(annotate), fg="cyan"))
 
-@command
-@click.option(
-    "-l",
-    "--link",
-    metavar="TARGET",
-    help="Link the project before watching.",
-)
-@click.option(
-    "-i",
-    "--interval",
-    metavar="SECONDS",
-    default=0.6,
-    help="Configure the polling interval.",
-)
-def watch(project: Project, link: Optional[str], interval: float):
-    """Watch the project directory and build on file changes."""
-    text = "Linking and watching project..." if link else "Watching project..."
-    with message_fence(text):
-        if link:
-            click.echo("\n".join(project.link(target=link)))
-
-        for changes in project.watch(interval):
-            filename, action = next(iter(changes.items()))
-
-            text = (
-                f"{action.capitalize()} {filename!r}"
-                if changes == {filename: action}
-                else f"{len(changes)} changes detected"
-            )
-
-            now = time.strftime("%H:%M:%S")
-            change_time = click.style(now, fg="green", bold=True)
-            click.echo(f"{change_time} {text}")
+        for line in lines:
+            click.echo(line_prefix + " " * bool(line) + line)
 
-            with error_handler(format_padding=1):
-                project.build()
 
+class BeetHelpColorsMixin:
+    """Mixin that fixes usage formatting."""
 
-@command
-@click.argument("patterns", nargs=-1)
-@click.option(
-    "-c",
-    "--clear",
-    is_flag=True,
-    help="Clear the cache.",
-)
-def cache(project: Project, patterns: Sequence[str], clear: bool):
-    """Inspect or clear the cache."""
-    if clear:
-        with message_fence("Clearing cache..."):
-            if cache_names := ", ".join(project.clear_cache(patterns)):
-                click.echo(f"Cache cleared successfully: {cache_names}.\n")
-            else:
-                click.echo(
-                    "No matching results.\n"
-                    if patterns
-                    else "The cache is already cleared.\n"
-                )
-    else:
-        with message_fence("Inspecting cache..."):
-            click.echo(
-                "\n".join(project.inspect_cache(patterns))
-                or (
-                    "No matching results.\n"
-                    if patterns
-                    else "The cache is completely clear.\n"
-                )
-            )
+    help_headers_color: str
+    help_options_color: str
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        kwargs.setdefault("help_headers_color", "red")
+        kwargs.setdefault("help_options_color", "green")
+        super().__init__(*args, **kwargs)
+
+    def format_usage(self, ctx: click.Context, formatter: Any):
+        formatter.write_usage(
+            ctx.command_path,
+            " ".join(self.collect_usage_pieces(ctx)),  # type: ignore
+            click.style("Usage", fg=self.help_headers_color) + ": ",
+        )
+
+
+class BeetCommand(BeetHelpColorsMixin, HelpColorsCommand):
+    """Click command subclass for the beet command-line."""
+
+
+class BeetGroup(BeetHelpColorsMixin, HelpColorsGroup):
+    """Click group subclass for the beet command-line."""
+
+    def get_command(self, ctx: click.Context, cmd_name: str) -> Optional[click.Command]:
+        if command := super().get_command(ctx, cmd_name):
+            return command
+
+        matches = [cmd for cmd in self.list_commands(ctx) if cmd.startswith(cmd_name)]
+
+        if len(matches) > 1:
+            match_list = ", ".join(sorted(matches))
+            ctx.fail(f"Ambiguous shorthand {cmd_name!r} ({match_list}).")
+        elif matches:
+            return super().get_command(ctx, matches[0])
+
+        return None
+
+    def add_command(self, cmd: click.Command, name: Optional[str] = None) -> None:
+        if cmd.callback:  # type: ignore
+            cmd.callback = error_handler(should_exit=True)(cmd.callback)  # type: ignore
+        return super().add_command(cmd, name=name)
+
+    def command(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Callable[[Callable[..., Any]], click.Command]:
+        kwargs.setdefault("cls", BeetCommand)
+        return super().command(*args, **kwargs)
+
+    def group(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Callable[[Callable[..., Any]], click.Group]:
+        kwargs.setdefault("cls", BeetGroup)
+        return super().group(*args, **kwargs)
 
 
-@command
-@click.argument("target", required=False)
+class MainGroup(BeetGroup):
+    """The root group of the beet command-line."""
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        kwargs.setdefault("invoke_without_command", True)
+        kwargs.setdefault("context_settings", {"help_option_names": ("-h", "--help")})
+        super().__init__(*args, **kwargs)
+        self.entry_points_loaded = False
+
+    def load_entry_points(self):
+        """Load commands from installed entry points if they haven't been loaded yet."""
+        if self.entry_points_loaded:
+            return
+
+        self.entry_points_loaded = True
+
+        for ep in entry_points(group="beet", name="commands"):
+            ep.load()
+
+    def get_command(self, ctx: click.Context, cmd_name: str) -> Optional[click.Command]:
+        self.load_entry_points()
+        return super().get_command(ctx, cmd_name)
+
+    def list_commands(self, ctx: click.Context) -> List[str]:
+        self.load_entry_points()
+        return super().list_commands(ctx)
+
+
+@click.group(cls=MainGroup)  # type: ignore
+@click.pass_context
 @click.option(
-    "-c",
-    "--clear",
-    is_flag=True,
-    help="Clear the link.",
+    "-p",
+    "--project",
+    metavar="PATH",
+    help="Select project.",
 )
-def link(project: Project, target: Optional[str], clear: bool):
-    """Link the generated resource pack and data pack to Minecraft."""
-    if clear:
-        with message_fence("Clearing project link..."):
-            project.clear_link()
-    else:
-        with message_fence("Linking project..."):
-            click.echo("\n".join(project.link(target)))
+@click.option(
+    "-s",
+    "--set",
+    metavar="OPTION",
+    multiple=True,
+    help="Set config option.",
+)
+@click.option(
+    "-l",
+    "--log",
+    metavar="LEVEL",
+    type=click.Choice(
+        ["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"], case_sensitive=False
+    ),
+    default="WARNING",
+    help="Configure output verbosity.",
+)
+@click.version_option(
+    __version__,
+    "-v",
+    "--version",
+    message=click.style("%(prog)s", fg="red")
+    + click.style(" v%(version)s", fg="green"),
+)
+def beet(
+    ctx: click.Context,
+    project: Optional[str],
+    set: List[str],
+    log: str,
+):
+    """The beet toolchain."""
+    logger = logging.getLogger()
+    logger.setLevel(log)
+    logger.addHandler(LogHandler())
+
+    project_obj = ctx.ensure_object(Project)
+
+    if set:
+        project_obj.config_overrides = set
+    if project:
+        project_obj.config_path = project
+
+    if not ctx.invoked_subcommand:
+        if build := beet.get_command(ctx, "build"):
+            ctx.invoke(build)
 
 
 def main():
-    """Invoke the command-line entrypoint."""
+    """Invoke the beet command-line."""
     beet(prog_name="beet")
```

### Comparing `beet-0.9.4/beet/toolchain/helpers.py` & `beet-0.90.0/beet/toolchain/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 __all__ = [
     "subproject",
     "sandbox",
     "run_beet",
+    "JinjaExtension",
 ]
 
 
-from contextlib import ExitStack
+from contextlib import contextmanager
+from functools import wraps
 from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Optional, Union
+from typing import Iterator, Optional, Union
+
+from jinja2 import Environment
+from jinja2.ext import Extension
 
-from beet.core.cache import MultiCache
 from beet.core.utils import FileSystemPath, JsonDict
 
 from .config import ProjectConfig, config_error_handler
-from .context import Context, Plugin, PluginSpec
+from .context import Context, Plugin, PluginSpec, ProjectCache
 from .project import Project, ProjectBuilder
 from .template import TemplateManager
+from .worker import WorkerPool
 
 
 def subproject(config: Union[ProjectConfig, JsonDict, FileSystemPath]) -> Plugin:
     """Return a plugin that runs a subproject."""
 
+    @wraps(subproject)
     def plugin(ctx: Context):
-        project = Project(resolved_cache=ctx.cache)
+        project = Project(
+            resolved_cache=ctx.cache,
+            resolved_worker_pool=WorkerPool(resolved_handle=ctx.worker),
+        )
 
         if isinstance(config, ProjectConfig):
             project.resolved_config = config
         elif isinstance(config, dict):
-            with config_error_handler("<subproject>"):
+            with config_error_handler("(subproject)"):
                 project.resolved_config = ProjectConfig(**config).resolve(ctx.directory)
         else:
-            path = Path(config)
-
-            if path.is_dir():
-                project.config_directory = path
-            else:
-                project.config_path = path
+            project.config_path = config
 
         ctx.require(ProjectBuilder(project))
 
     return plugin
 
 
 def sandbox(*specs: PluginSpec) -> Plugin:
     """Return a plugin that runs the specified plugins in an isolated pipeline."""
 
     def plugin(ctx: Context):
         child_ctx = Context(
+            project_id=ctx.project_id,
             project_name=ctx.project_name,
             project_description=ctx.project_description,
             project_author=ctx.project_author,
             project_version=ctx.project_version,
+            project_root=False,
+            minecraft_version=ctx.minecraft_version,
             directory=ctx.directory,
             output_directory=None,
             meta={},
             cache=ctx.cache,
+            worker=ctx.worker,
             template=TemplateManager(
                 templates=list(ctx.template.directories),
                 cache_dir=ctx.cache["template"].directory,
             ),
         )
 
         with child_ctx.activate() as pipeline:
@@ -67,35 +74,45 @@
 
         ctx.assets.merge(child_ctx.assets)
         ctx.data.merge(child_ctx.data)
 
     return plugin
 
 
+@contextmanager
 def run_beet(
-    config: Optional[Union[JsonDict, FileSystemPath]] = None,
+    config: Optional[Union[ProjectConfig, JsonDict, FileSystemPath]] = None,
     directory: Optional[FileSystemPath] = None,
-    cache: Union[bool, MultiCache] = False,
-) -> Context:  # type: ignore
+    cache: Union[bool, ProjectCache] = False,
+) -> Iterator[Context]:
     """Run the entire toolchain programmatically."""
     if not directory:
         directory = Path.cwd()
 
-    with ExitStack() as stack:
-        project = Project()
-
-        if isinstance(cache, MultiCache):
-            project.resolved_cache = cache
-        elif not cache:
-            project.resolved_cache = MultiCache(
-                stack.enter_context(TemporaryDirectory())
-            )
-
-        if isinstance(config, dict):
-            with config_error_handler("<project>"):
-                project.resolved_config = ProjectConfig(**config).resolve(directory)
-        elif config:
-            project.config_path = config
-        else:
-            project.config_directory = directory
+    tmpdir = False
+    project = Project()
 
-        return ProjectBuilder(project).build()
+    if isinstance(cache, ProjectCache):
+        project.resolved_cache = cache
+    elif not cache:
+        tmpdir = True
+
+    if isinstance(config, ProjectConfig):
+        project.resolved_config = config
+    elif isinstance(config, dict):
+        with config_error_handler("(project)"):
+            project.resolved_config = ProjectConfig(**config).resolve(directory)
+    else:
+        project.config_path = config or directory
+
+    with ProjectBuilder(project, root=True, tmpdir=tmpdir).build() as ctx:
+        yield ctx
+
+
+class JinjaExtension(Extension):
+    """Base extension that provides a reference to the beet context."""
+
+    environment: Environment
+
+    @property
+    def ctx(self) -> Context:
+        return getattr(self.environment, "_beet_template_manager").ctx
```

### Comparing `beet-0.9.4/beet/toolchain/pipeline.py` & `beet-0.90.0/beet/toolchain/pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,163 @@
 __all__ = [
     "GenericPipeline",
     "Task",
     "GenericPlugin",
     "GenericPluginSpec",
-    "PipelineFallthroughException",
-    "FormattedPipelineException",
     "PluginError",
     "PluginImportError",
 ]
 
 
 from dataclasses import dataclass, field
 from typing import (
     Any,
+    Generator,
     Generic,
     Iterable,
     Iterator,
     List,
     Optional,
     Protocol,
     Set,
     TypeVar,
     Union,
     cast,
 )
 
-from .utils import format_obj, import_from_string
+from beet.core.error import BubbleException, WrappedException
+from beet.core.utils import format_obj, import_from_string, pop_traceback
 
 T = TypeVar("T")
+ContextType = TypeVar("ContextType", contravariant=True)
 
 
-class GenericPlugin(Protocol[T]):
+class GenericPlugin(Protocol[ContextType]):
     """Protocol for detecting plugins."""
 
-    def __call__(self, ctx: T) -> Any:
+    def __call__(self, ctx: ContextType, /) -> Any:
         ...
 
 
-GenericPluginSpec = Union[GenericPlugin[T], str]
+GenericPluginSpec = Union[GenericPlugin[ContextType], str]
 
 
-class PipelineFallthroughException(Exception):
-    """Exceptions inheriting from this class will fall through the pipeline exception handling."""
-
-
-class FormattedPipelineException(PipelineFallthroughException):
-    """Exceptions inheriting from this class can expose a formatted message."""
-
-    def __init__(self, *args: Any):
-        super().__init__(*args)
-        self.message = ""
-        self.format_cause = False
-
-
-class PluginError(FormattedPipelineException):
+class PluginError(WrappedException):
     """Raised when a plugin raises an exception."""
 
+    plugin: Any
+
     def __init__(self, plugin: Any):
         super().__init__(plugin)
-        self.message = f"Plugin {format_obj(plugin)} raised an exception."
-        self.format_cause = True
+        self.plugin = plugin
 
+    def __str__(self) -> str:
+        return f"Plugin {format_obj(self.plugin)} raised an exception."
 
-class PluginImportError(FormattedPipelineException):
+
+class PluginImportError(WrappedException):
     """Raised when a plugin couldn't be imported."""
 
+    plugin: Any
+
     def __init__(self, plugin: Any):
         super().__init__(plugin)
-        self.message = f"Couldn't import plugin {format_obj(plugin)}."
-        self.format_cause = True
+        self.plugin = plugin
+
+    def __str__(self) -> str:
+        return f"Couldn't import plugin {format_obj(self.plugin)}."
 
 
 @dataclass
 class Task(Generic[T]):
     """A unit of work generated by the pipeline."""
 
     plugin: GenericPlugin[T]
     iterator: Optional[Iterator[Any]] = None
 
-    def advance(self, ctx: T) -> Optional["Task[T]"]:
+    def advance(
+        self,
+        ctx: T,
+        exception: Optional[Exception] = None,
+    ) -> Optional["Task[T]"]:
         """Make progress on the task and return it unless no more work is necessary."""
         try:
             if self.iterator is None:
                 result = self.plugin(ctx)
                 self.iterator = iter(
                     cast(Iterable[Any], result) if isinstance(result, Iterable) else []
                 )
-            for _ in self.iterator:
-                return self
-        except PipelineFallthroughException:
+            if exception is None:
+                next(self.iterator)
+            elif isinstance(self.iterator, Generator):
+                self.iterator.throw(exception)
+            else:
+                raise exception
+        except StopIteration:
+            return None
+        except BubbleException:
             raise
         except Exception as exc:
-            raise PluginError(self.plugin) from exc.with_traceback(
-                getattr(exc.__traceback__, "tb_next", exc.__traceback__)
-            )
-        return None
+            raise PluginError(self.plugin) from pop_traceback(exc)
+        return self
 
 
 @dataclass
 class GenericPipeline(Generic[T]):
     """The plugin execution engine."""
 
     ctx: T
     default_symbol: str = "beet_default"
 
+    whitelist: Optional[List[str]] = None
     plugins: Set[GenericPlugin[T]] = field(default_factory=set)
     tasks: List[Task[T]] = field(default_factory=list)
 
-    def require(self, spec: GenericPluginSpec[T]):
+    def require(self, *args: GenericPluginSpec[T]):
         """Execute the specified plugin."""
-        plugin = self.resolve(spec)
-        if plugin in self.plugins:
-            return
+        for spec in args:
+            plugin = self.resolve(spec)
+            if plugin in self.plugins:
+                continue
 
-        self.plugins.add(plugin)
+            self.plugins.add(plugin)
 
-        if remaining_work := Task(plugin).advance(self.ctx):
-            self.tasks.append(remaining_work)
+            if remaining_work := Task(plugin).advance(self.ctx):
+                self.tasks.append(remaining_work)
 
     def resolve(self, spec: GenericPluginSpec[T]) -> GenericPlugin[T]:
         """Return the imported plugin if the argument is a dotted path."""
         try:
             return (
-                import_from_string(spec, default_member=self.default_symbol)
+                import_from_string(
+                    dotted_path=spec,
+                    default_member=self.default_symbol,
+                    whitelist=self.whitelist,
+                )
                 if isinstance(spec, str)
                 else spec
             )
-        except PipelineFallthroughException:
+        except BubbleException:
             raise
         except Exception as exc:
             raise PluginImportError(spec) from exc
 
     def run(self, specs: Iterable[GenericPluginSpec[T]] = ()):
         """Run the specified plugins."""
-        for spec in specs:
-            self.require(spec)
+        try:
+            self.require(*specs)
+        except Exception as exc:
+            exception = exc
+        else:
+            exception = None
 
         while self.tasks:
-            if remaining_work := self.tasks.pop().advance(self.ctx):
-                self.tasks.append(remaining_work)
+            try:
+                if remaining_work := self.tasks.pop().advance(self.ctx, exception):
+                    self.tasks.append(remaining_work)
+            except Exception as exc:
+                exception = exc
+            else:
+                exception = None
+
+        if exception is not None:
+            raise exception
```

### Comparing `beet-0.9.4/pyproject.toml` & `beet-0.90.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beet"
-version = "0.9.4"
+version = "0.90.0"
 description = "The Minecraft pack development kit"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/beet"
 repository = "https://github.com/mcbeet/beet"
 documentation = "https://github.com/mcbeet/beet"
@@ -12,68 +12,93 @@
 readme = "README.md"
 
 keywords = [
   "beet",
   "minecraft",
   "datapack",
   "resourcepack",
-  "mcfunction"
+  "mcfunction",
 ]
 
 include = ["beet/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-nbtlib = "^1.8.2"
-pathspec = "^0.8.1"
-Pillow = "^8.0.1"
-pydantic = "^1.7.3"
-click = "^7.1.2"
-click-help-colors = "^0.9"
-Jinja2 = "^2.11.2"
+python = "^3.10"
+nbtlib = "^1.12.1"
+pathspec = "^0.11.0"
+pydantic = "^1.10.7"
+click = "^8.1.3"
+click-help-colors = "^0.9.1"
+Jinja2 = "^3.1.2"
+toml = "^0.10.2"
+PyYAML = "^6.0"
+Pillow = {version = "*", optional = true}
 colorama = {version = "*", markers = 'sys_platform == "win32"'}
 
-[tool.poetry.dev-dependencies]
-black = "^20.8b1"
-pytest = "^6.2.2"
-rope = "^0.18.0"
-pytest-minecraft = "^0.1.1"
-isort = "^5.7.0"
-pytest-insta = "^0.1.5"
-python-semantic-release = "^7.15.0"
-mudkip = "^0.3.8"
+[tool.poetry.extras]
+image = ["Pillow"]
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pytest = "^7.3.1"
+pytest-minecraft = "^0.2.0"
+isort = "^5.12.0"
+pytest-insta = "^0.2.0"
+python-semantic-release = "^7.33.3"
+mudkip = "^0.8.0"
 
 [tool.poetry.scripts]
 beet = "beet.toolchain.cli:main"
 
+[tool.poetry.plugins.beet]
+commands = "beet.toolchain.commands"
+autoload = "beet.contrib.default"
+
+[tool.poetry.plugins.pytest11]
+beet = "beet.pytest_plugin"
+
+[tool.pytest.ini_options]
+addopts = "tests beet --ignore beet/__main__.py --doctest-modules"
+doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
+
+[tool.pyright]
+typeCheckingMode = "basic"
+ignore = ["docs", "setup.py"]
+strict = [
+  "beet/contrib",
+  "beet/core",
+  "beet/library",
+  "beet/toolchain",
+  "examples",
+  "tests",
+]
+
 [tool.black]
-target-version = ["py38"]
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | node_modules
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
+target-version = ["py310"]
 
 [tool.isort]
 profile = "black"
 
 [tool.semantic_release]
 branch = "main"
 version_variable = ["beet/__init__.py:__version__"]
 version_toml = "pyproject.toml:tool.poetry.version"
 major_on_zero = false
 build_command = "poetry build"
 
+[tool.mudkip]
+base_url = "https://mcbeet.dev"
+preset = "furo"
+
+[tool.mudkip.override]
+html_title = "Beet documentation"
+html_logo = "assets/beet_logo.png"
+html_favicon = "assets/favicon.png"
+suppress_warnings = ["myst.header"]
+linkcheck_ignore = ['https://github\.com/mcbeet/beet/commit/.+']
+
+[tool.mudkip.override.html_theme_options]
+sidebar_hide_name = true
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `beet-0.9.4/PKG-INFO` & `beet-0.90.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,53 @@
-Metadata-Version: 2.1
-Name: beet
-Version: 0.9.4
-Summary: The Minecraft pack development kit
-Home-page: https://github.com/mcbeet/beet
-License: MIT
-Keywords: beet,minecraft,datapack,resourcepack,mcfunction
-Author: Valentin Berlier
-Author-email: berlier.v@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Jinja2 (>=2.11.2,<3.0.0)
-Requires-Dist: Pillow (>=8.0.1,<9.0.0)
-Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: click-help-colors (>=0.9,<0.10)
-Requires-Dist: colorama; sys_platform == "win32"
-Requires-Dist: nbtlib (>=1.8.2,<2.0.0)
-Requires-Dist: pathspec (>=0.8.1,<0.9.0)
-Requires-Dist: pydantic (>=1.7.3,<2.0.0)
-Project-URL: Documentation, https://github.com/mcbeet/beet
-Project-URL: Repository, https://github.com/mcbeet/beet
-Description-Content-Type: text/markdown
-
-<img align="right" src="logo.png" alt="logo" width="76">
+<img align="right" src="https://raw.githubusercontent.com/mcbeet/beet/main/logo.png?sanitize=true" alt="logo" width="76">
 
 # Beet
 
 [![GitHub Actions](https://github.com/mcbeet/beet/workflows/CI/badge.svg)](https://github.com/mcbeet/beet/actions)
 [![PyPI](https://img.shields.io/pypi/v/beet.svg)](https://pypi.org/project/beet/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/beet.svg)](https://pypi.org/project/beet/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Discord](https://img.shields.io/discord/900530660677156924?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/98MdSGMm8j)
 
 > The Minecraft pack development kit.
 
 ## Introduction
 
-Minecraft [resource packs](https://minecraft.gamepedia.com/Resource_Pack) and [data packs](https://minecraft.gamepedia.com/Data_Pack) work well as _distribution_ formats but can be pretty limiting as _authoring_ formats. Without the ability to parametrize or create abstractions over assets and data pack resources, projects and libraries created by the community are greatly limited when it comes to reusability and interoperability.
-
-There's been a lot of attempts at establishing standardized tooling to improve the development experience and it's becoming more and more apparent that the problem space is fundamentally multi-paradigm. Different problems require different solutions, so providing unified cross-project reusability needs to involve an interoperability layer that's sufficiently unopinionated to let all these paradigms shine through.
+Minecraft [resource packs](https://minecraft.gamepedia.com/Resource_Pack) and [data packs](https://minecraft.gamepedia.com/Data_Pack) work well as _distribution_ formats but can be pretty limiting as _authoring_ formats. You can quickly end up having to manage hundreds of files, some of which might be buried within the bundled output of various generators.
 
-The `beet` project is meant to serve as a platform for building a cooperative tooling ecosystem by providing a flexible composition model and a user-friendly development workflow.
+The `beet` project is a development kit that tries to unify data pack and resource pack tooling into a single pipeline. The community is always coming up with pre-processors, frameworks, and generators of all kinds to make the developer experience more ergonomic. With `beet` you can seamlessly integrate all these tools in your project.
 
 ### Screencasts
 
 - **Quick start** [https://youtu.be/JGrJTOhG3pY](https://youtu.be/JGrJTOhG3pY)
 - **Command-line** [https://youtu.be/fQ9up0ELPNE](https://youtu.be/fQ9up0ELPNE)
 - **Library overview** [https://youtu.be/LDvV4_l-PSc](https://youtu.be/LDvV4_l-PSc)
 - **Plugins basics** [https://youtu.be/XTzKmvHqd1g](https://youtu.be/XTzKmvHqd1g)
 - **Pipeline configuration** [https://youtu.be/QsnQncGxAAs](https://youtu.be/QsnQncGxAAs)
 
 ### Library
 
-> [Documentation](https://mcbeet.dev/library/)
-
 ```python
 from beet import ResourcePack, Texture
 
 # Open a zipped resource pack and add a custom stone texture
 with ResourcePack(path="stone.zip") as assets:
     assets["minecraft:block/stone"] = Texture(source_path="custom.png")
 ```
 
 The `beet` library provides carefully crafted primitives for working with Minecraft resource packs and data packs.
 
 - Create, read, edit and merge resource packs and data packs
 - Handle zipped and unzipped packs
 - Fast and lazy by default, files are transparently loaded when needed
 - Statically typed API enabling rich intellisense and autocompletion
+- First-class [`pytest`](https://github.com/pytest-dev/pytest/) integration with detailed assertion explanations
 
 ### Toolchain
 
-> [Documentation](https://mcbeet.dev/toolchain/)
-
 ```python
 from beet import Context, Function
 
 def greet(ctx: Context):
     """Plugin that adds a function for greeting the player."""
     ctx.data["greet:hello"] = Function(["say hello"], tags=["minecraft:load"])
 ```
@@ -85,56 +55,60 @@
 The `beet` toolchain is designed to support a wide range of use-cases. The most basic pipeline will let you create configurable resource packs and data packs, but plugins make it easy to implement arbitrarily advanced workflows and tools like linters, asset generators and function pre-processors.
 
 - Compose plugins that can inspect and edit the generated resource pack and data pack
 - Configure powerful build systems for development and creating releases
 - First-class template integration approachable without prior Python knowledge
 - Link the generated resource pack and data pack to Minecraft
 - Automatically rebuild the project on file changes with watch mode
+- Batteries-included package that comes with a few handy plugins out of the box
+- Rich ecosystem, extensible CLI, and powerful generator and worker API
 
 ## Installation
 
 The package can be installed with `pip`.
 
 ```bash
 $ pip install beet
 ```
 
+To create and edit images programmatically you should install `beet` with the `image` extra or install `Pillow` separately.
+
+```bash
+$ pip install beet[image]
+$ pip install beet Pillow
+```
+
 You can make sure that `beet` was successfully installed by trying to use the toolchain from the command-line.
 
 ```bash
 $ beet --help
 Usage: beet [OPTIONS] COMMAND [ARGS]...
 
   The beet toolchain.
 
 Options:
-  -d, --directory DIRECTORY  Use the specified project directory.
-  -c, --config FILE          Use the specified config file.
-  -v, --version              Show the version and exit.
-  -h, --help                 Show this message and exit.
+  -p, --project PATH  Select project.
+  -s, --set OPTION    Set config option.
+  -l, --log LEVEL     Configure output verbosity.
+  -v, --version       Show the version and exit.
+  -h, --help          Show this message and exit.
 
 Commands:
   build  Build the current project.
   cache  Inspect or clear the cache.
   link   Link the generated resource pack and data pack to Minecraft.
   watch  Watch the project directory and build on file changes.
 ```
 
-## Status
-
-You can expect current releases to be pretty stable, but the project as a whole should still be considered alpha.
-
-The main reason is that resource pack and data pack coverage is currently lacking in certain areas. Exposing a consistent interface for every data pack and resource pack feature can involve design decisions that aren't immediately obvious. You're welcome to open an issue to discuss the implementation of currently unsupported resources. And feel free to ask questions, report bugs, and share your thoughts and impressions.
-
 ## Contributing
 
 Contributions are welcome. Make sure to first open an issue discussing the problem or the new feature before creating a pull request. The project uses [`poetry`](https://python-poetry.org).
 
 ```bash
-$ poetry install
+$ poetry install --extras image
 ```
 
 You can run the tests with `poetry run pytest`. We use [`pytest-minecraft`](https://github.com/vberlier/pytest-minecraft) to run tests against actual Minecraft releases.
 
 ```bash
 $ poetry run pytest
 $ poetry run pytest --minecraft-latest
@@ -160,8 +134,7 @@
 $ poetry run black beet tests
 $ poetry run black --check beet tests
 ```
 
 ---
 
 License - [MIT](https://github.com/mcbeet/beet/blob/main/LICENSE)
-
```

