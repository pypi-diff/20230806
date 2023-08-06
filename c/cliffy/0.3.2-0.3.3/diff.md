# Comparing `tmp/cliffy-0.3.2.tar.gz` & `tmp/cliffy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.3.2.tar", max compression
+gzip compressed data, was "cliffy-0.3.3.tar", max compression
```

## Comparing `cliffy-0.3.2.tar` & `cliffy-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1060 2023-06-24 20:57:23.061909 cliffy-0.3.2/LICENSE
--rw-r--r--   0        0        0     6810 2023-06-24 20:57:23.061909 cliffy-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/__init__.py
--rw-r--r--   0        0        0       97 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/__main__.py
--rw-r--r--   0        0        0     1859 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/builder.py
--rw-r--r--   0        0        0     8076 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     6380 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1976 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     3776 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/helper.py
--rw-r--r--   0        0        0     3000 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/homer.py
--rw-r--r--   0        0        0     1392 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/loader.py
--rw-r--r--   0        0        0      396 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7355 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/merger.py
--rw-r--r--   0        0        0     4663 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/parser.py
--rw-r--r--   0        0        0        0 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/py.typed
--rw-r--r--   0        0        0      972 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/rich.py
--rw-r--r--   0        0        0       47 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/run.py
--rw-r--r--   0        0        0     3829 2023-06-24 20:57:23.061909 cliffy-0.3.2/cliffy/transformer.py
--rw-r--r--   0        0        0      895 2023-06-24 20:57:23.065909 cliffy-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     7763 1970-01-01 00:00:00.000000 cliffy-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-18 02:44:21.701176 cliffy-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6770 2023-07-18 02:44:21.701176 cliffy-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/__main__.py
+-rw-r--r--   0        0        0     2595 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/builder.py
+-rw-r--r--   0        0        0     7627 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     6602 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      990 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1976 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     3725 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/helper.py
+-rw-r--r--   0        0        0     3000 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/homer.py
+-rw-r--r--   0        0        0     1392 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/loader.py
+-rw-r--r--   0        0        0      391 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7353 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/merger.py
+-rw-r--r--   0        0        0     4662 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/parser.py
+-rw-r--r--   0        0        0        0 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/py.typed
+-rw-r--r--   0        0        0     1595 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/run.py
+-rw-r--r--   0        0        0     3837 2023-07-18 02:44:21.701176 cliffy-0.3.3/cliffy/transformer.py
+-rw-r--r--   0        0        0     1245 2023-07-18 02:44:21.705176 cliffy-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 cliffy-0.3.3/PKG-INFO
```

### Comparing `cliffy-0.3.2/LICENSE` & `cliffy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.2/README.md` & `cliffy-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,42 +8,14 @@
 ## Features
 * Rapidly build CLIs with YAML-defined manifests
 * Manage CLIs- load, list, update, and remove
 * Built-in shell and Python scripting support
 * Supports Jinja2-templating
 * Build and bundle CLIs into self-contained, portable zipapps
 
-## Install
-* `pip install "cliffy[rich]"` to include [rich-click](https://github.com/ewels/rich-click) for colorful CLI help output formatted with [rich](https://github.com/Textualize/rich).
-
-or 
-
-* `pip install cliffy`
-
-## How it works
-1. Define CLI manifests in YAML files
-2. Run `cli` commands to load, build, and manage CLIs
-3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
-4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
-5. Run loaded CLIs straight from the terminal
-6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
-
-## Usage
-`cli <command>`
-* `init <cli name> --raw`: Generate a template CLI manifest for a new CLI
-* `load <manifest>`: Add a new CLI based on the manifest
-* `render <manifest>`: View generated CLI script for a manifest
-* `list` or `ls`: Output a list of loaded CLIs 
-* `update <cli name>`: Reload a loaded CLI
-* `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
-* `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
-* `build <manifest>`: Build a CLI manifest into a self-contained zipapp
-* `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
-* `info <cli name>`: Display CLI metadata
-
 ### Load
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
 version: 0.1.0
@@ -100,16 +72,43 @@
 Builds a portable zipapp containing the CLI and its package requirements.
 
 3. Run CLI
 ```
 ./dist/requires -h
 ```
 
+## Usage
+`cli <command>`
+* `init <cli name> --raw`: Generate a template CLI manifest for a new CLI
+* `load <manifest>`: Add a new CLI based on the manifest
+* `render <manifest>`: View generated CLI script for a manifest
+* `list` or `ls`: Output a list of loaded CLIs 
+* `update <cli name>`: Reload a loaded CLI
+* `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
+* `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
+* `build <cli name or manifest>`: Build a CLI manifest or a loaded CLI into a self-contained zipapp
+* `info <cli name>`: Display CLI metadata
+
+## How it works
+1. Define CLI manifests in YAML files
+2. Run `cli` commands to load, build, and manage CLIs
+3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
+4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
+5. Run loaded CLIs straight from the terminal
+6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
+
+## Install
+* `pip install "cliffy[rich]"` to include [rich-click](https://github.com/ewels/rich-click) for colorful CLI help output formatted with [rich](https://github.com/Textualize/rich).
+
+or 
+
+* `pip install cliffy`
+
 ## Manifest template
-Generated by `cli init`:
+Generated by `cli init`. For a barebones template, run `cli init --raw`
 ```yaml
 # cliffy v1 template
 manifestVersion: v1
 
 # The name of the CLI
 # This will be used as the script name when invoking the CLI from the command line.
 name: cliffy 
@@ -184,14 +183,13 @@
     # this is a nested command that will get invoked with: hello greet all
     greet.all: 
         - help: Help text for list.all       # you can also define help text like this
         - $ echo "hello all"                 # this is a bash command that will get converted to python subprocess call
         - print("greetings from python")     # this python code will get directly invoked
 
 ```
-For a barebones template: `cli init --raw`
 
 ## Development
 ```
 poetry shell
 cli -h
 ```
```

### Comparing `cliffy-0.3.2/cliffy/builder.py` & `cliffy-0.3.3/cliffy/builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from io import TextIOWrapper
 import os
 import sys
 from importlib import import_module
 from pathlib import Path
 from shutil import copy
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from types import ModuleType
@@ -9,21 +10,41 @@
 
 from click.testing import CliRunner, Result
 from shiv import cli as shiv_cli
 from shiv import pip
 
 from cliffy.helper import TEMP_FILES, delete_temp_files
 
+from cliffy.transformer import Transformer
+
+from cliffy.commander import CLI
+
+
+def build_cli_from_manifest(
+    manifestIO: TextIOWrapper, output_dir: Optional[str] = None, interpreter: str = "/usr/bin/env python3"
+) -> tuple[CLI, Result]:
+    T = Transformer(manifestIO, validate_requires=False)
+    with NamedTemporaryFile(mode="w", prefix=f"{T.cli.name}_", suffix=".py", delete=False) as script:
+        script.write(T.cli.code)
+        script.flush()
+        result = build_cli(
+            T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir, interpreter=interpreter
+        )
+        TEMP_FILES.append(script)
+
+    delete_temp_files()
+    return T.cli, result
+
 
 def build_cli(
     cli_name: str,
     script_path: str,
     deps: Optional[list[str]] = None,
     output_dir: Optional[str] = None,
-    interpreter: str = "/usr/bin/env python3 -sE",
+    interpreter: str = "/usr/bin/env python3",
 ) -> Result:
     if deps is None:
         deps = []
 
     if output_dir and not Path(output_dir).exists():
         os.mkdir(output_dir)
 
@@ -32,15 +53,15 @@
         pip_deps = ["typer"] + deps
 
         pip.install(["--target", tdist] + pip_deps)
 
         runner = CliRunner()
         output_file = os.path.join(output_dir, f"{cli_name}") if output_dir else cli_name
         return runner.invoke(
-            shiv_cli.main,
+            shiv_cli.main,  # type: ignore
             ["--site-packages", tdist, "--compressed", "-e", f"{cli_name}.cli", "-o", output_file, "-p", interpreter],
         )
 
 
 def import_module_from_path(filepath: str) -> ModuleType:
     module_path, module_filename = os.path.split(filepath)
     sys.path.append(module_path)
```

### Comparing `cliffy-0.3.2/cliffy/cli.py` & `cliffy-0.3.3/cliffy/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 ## CLI to generate CLIs
 import contextlib
-from tempfile import NamedTemporaryFile
-from typing import TextIO
+from io import TextIOWrapper
+import os
+from typing import IO, Any, Optional, TextIO, Union, cast
 
-try:
-    import rich_click as click  # type: ignore
-    from rich.console import Console  # type: ignore
-    from rich_click.rich_group import RichGroup as AliasGroup  # type: ignore
-except ImportError:
-    import click
-    from .rich import Console
-    from click import Group as AliasGroup
+from click.core import Context, Parameter
+from click.types import _is_file_like
 
-from .builder import build_cli, run_cli
+from .rich import click, Console
+from .rich import ClickGroup  # type: ignore
+
+from .builder import build_cli, build_cli_from_manifest, run_cli
 from .helper import (
     CLIFFY_CLI_DIR,
-    TEMP_FILES,
     age_datetime,
-    delete_temp_files,
     exit_err,
     indent_block,
     out,
     out_err,
     print_rich_table,
     write_to_file,
 )
@@ -29,41 +25,56 @@
 from .loader import Loader
 from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
-class AliasedGroup(AliasGroup):  # type: ignore
-    def get_command(self, ctx, cmd_name):
+class AliasedGroup(ClickGroup):
+    def get_command(self, ctx: click.Context, cmd_name: Optional[str]) -> Optional[click.Command]:
         with contextlib.suppress(KeyError):
-            cmd_name = ALIASES[cmd_name].name
+            cmd_name = ALIASES[cmd_name].name  # type: ignore
         return super().get_command(ctx, cmd_name or "")
 
 
-@click.group(context_settings=CONTEXT_SETTINGS, cls=AliasedGroup)
+class ManifestOrCLI(click.File):
+    def convert(  # type: ignore[override]
+        self, value: Union[str, "os.PathLike[str]", IO[Any]], param: Optional[Parameter], ctx: Optional[Context]
+    ) -> Union[str, IO[Any]]:
+        if _is_file_like(value):
+            return value
+
+        value = cast("Union[str, os.PathLike[str]]", value)
+
+        if isinstance(value, os.PathLike) or value.endswith("yaml"):
+            return super().convert(value, param, ctx)
+
+        return value
+
+
+@click.group(context_settings=CONTEXT_SETTINGS, cls=AliasedGroup)  # type: ignore[arg-type]
 @click.version_option()
 def cli() -> None:
     pass
 
 
-@cli.command()
+@cli.command()  # type: ignore[arg-type]
 @click.argument("manifests", type=click.File("rb"), nargs=-1)
 def load(manifests: list[TextIO]) -> None:
     """Load CLI for given manifest(s)"""
     for manifest in manifests:
         T = Transformer(manifest)
         Loader.load_from_cli(T.cli)
         save_metadata(manifest.name, T.cli)
         out(f"✨ Generated {T.cli.name} CLI v{T.cli.version} ✨", fg="green")
         out("$", fg="magenta", nl=False)
         out(f" {T.cli.name} -h")
 
 
-@cli.command()
+@cli.command()  # type: ignore[arg-type]
 @click.argument("cli_names", type=str, nargs=-1)
 def update(cli_names: list[str]) -> None:
     """Reloads CLI by name"""
     for cli_name in cli_names:
         if cli_metadata := get_metadata(cli_name):
             T = Transformer(open(cli_metadata.runner_path, "r"))
             Loader.load_from_cli(T.cli)
@@ -71,34 +82,34 @@
             out(f"✨ Reloaded {T.cli.name} CLI v{T.cli.version} ✨", fg="green")
             out("$", fg="magenta", nl=False)
             out(f" {T.cli.name} -h")
         else:
             out_err(f"~ {cli_name} not found")
 
 
-@cli.command()
+@cli.command()  # type: ignore[arg-type]
 @click.argument("manifest", type=click.File("rb"))
 def render(manifest: TextIO) -> None:
     """Render the CLI manifest generation as code"""
     T = Transformer(manifest)
     console = Console()
     console.print(T.cli.code, overflow="fold", emoji=False, markup=False)
     out(f"# Rendered {T.cli.name} CLI v{T.cli.version} ~", fg="green")
 
 
-@cli.command("run")
+@cli.command("run")  # type: ignore[arg-type]
 @click.argument("manifest", type=click.File("rb"))
 @click.argument("cli_args", type=str, nargs=-1)
 def cliffy_run(manifest: TextIO, cli_args: tuple[str]) -> None:
     """Run CLI for a manifest"""
     T = Transformer(manifest)
     run_cli(T.cli.name, T.cli.code, cli_args)
 
 
-@cli.command()
+@cli.command()  # type: ignore[arg-type]
 @click.argument("cli_name", type=str, default="cliffy")
 @click.option("--version", "-v", type=str, show_default=True, default="v1", help="Manifest version")
 @click.option("--render", is_flag=True, show_default=True, default=False, help="Render template to terminal directly")
 @click.option(
     "--raw",
     type=bool,
     is_flag=True,
@@ -118,121 +129,84 @@
         try:
             write_to_file(f"{cli_name}.yaml", text=template)
         except Exception as e:
             exit_err(f"~ error writing to file: {e}")
         out(f"+ {cli_name}.yaml", fg="green")
 
 
-@cli.command("list")
+@cli.command("list")  # type: ignore[arg-type]
 def cliffy_list() -> None:
     "List all CLIs loaded"
     cols = ["Name", "Version", "Age", "Manifest"]
     rows = [
         [metadata.cli_name, metadata.version, age_datetime(metadata.loaded), metadata.runner_path]
         for metadata in get_clis()
     ]
     print_rich_table(cols, rows, styles=["cyan", "magenta", "green", "blue"])
 
 
-@cli.command()
+@cli.command()  # type: ignore[arg-type]
 @click.argument("cli_names", type=str, nargs=-1)
 def remove(cli_names: list[str]) -> None:
     "Remove a loaded CLI by name"
     for cli_name in cli_names:
         if get_metadata_path(cli_name):
             remove_metadata(cli_name)
             Loader.unload_cli(cli_name)
             out(f"~ {cli_name} removed 💥", fg="green")
         else:
             out_err(f"~ {cli_name} not loaded")
 
 
-@cli.command()
-@click.argument("cli_names", type=str, nargs=-1)
-@click.option("--debug", is_flag=True, show_default=True, default=False, help="Display build output")
+@cli.command()  # type: ignore[arg-type]
+@click.argument("cli_or_manifests", type=ManifestOrCLI(), nargs=-1)
 @click.option("--output-dir", "-o", type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
 @click.option(
     "--python",
     "-p",
     type=str,
     help="Python interpreter to set as the zipapp shebang. This gets added after the #! ",
-    default="/usr/bin/env python3 -sE",
+    default="/usr/bin/env python3",
     show_default=True,
 )
-def bundle(cli_names: list[str], debug: bool, output_dir: str, python: str) -> None:
-    "Bundle a loaded CLI into a zipapp"
-    for cli_name in cli_names:
-        if not (metadata := get_metadata(cli_name)):
-            out_err(f"~ {cli_name} not loaded")
-            continue
-
-        result = build_cli(
-            cli_name,
-            script_path=f"{CLIFFY_CLI_DIR}/{cli_name}.py",
-            deps=metadata.requires,
-            output_dir=output_dir,
-            interpreter=python,
-        )
-
-        if result.exit_code != 0:
-            out(result.stdout)
-            out_err(f"~ {cli_name} bundle failed")
-            continue
-
-        if debug:
-            out(result.stdout)
-        out(f"+ {cli_name} bundled 📦", fg="green")
-
+def build(cli_or_manifests: list[Union[TextIOWrapper, str]], output_dir: str, python: str) -> None:
+    "Build a CLI manifest or a loaded CLI into a zipapp"
+    print(output_dir)
+    for cli_or_manifest in cli_or_manifests:
+        if isinstance(cli_or_manifest, TextIOWrapper):
+            cli, result = build_cli_from_manifest(cli_or_manifest, output_dir=output_dir, interpreter=python)
+            cli_name = cli.name
+        else:
+            cli_name = cast("str", cli_or_manifest)
+            if not (metadata := get_metadata(cli_name)):
+                out_err(f"~ {cli_name} not loaded")
+                continue
 
-@cli.command()
-@click.argument("manifests", type=click.File("rb"), nargs=-1)
-@click.option("--debug", is_flag=True, show_default=True, default=False, help="Display build output")
-@click.option("--output-dir", "-o", type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
-@click.option(
-    "--python",
-    "-p",
-    type=str,
-    help="Python interpreter to set as the zipapp shebang. This gets added after the #! ",
-    default="/usr/bin/env python3 -sE",
-    show_default=True,
-)
-def build(manifests: list[TextIO], debug: bool, output_dir: str, python: str) -> None:
-    "Build a CLI manifest into a zipapp"
-    for manifest in manifests:
-        T = Transformer(manifest, validate_requires=False)
-        with NamedTemporaryFile(mode="w", prefix=f"{T.cli.name}_", suffix=".py", delete=False) as script:
-            script.write(T.cli.code)
-            script.flush()
             result = build_cli(
-                T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir, interpreter=python
+                cli_name,
+                script_path=f"{CLIFFY_CLI_DIR}/{cli_name}.py",
+                deps=metadata.requires,
+                output_dir=output_dir,
+                interpreter=python,
             )
-            TEMP_FILES.append(script)
-
-        delete_temp_files()
 
         if result.exit_code != 0:
             out(result.stdout)
-            out_err(f"~ {T.cli.name} build failed")
+            out_err(f"~ {cli_name} build failed")
             continue
 
-        if debug:
-            out(result.stdout)
-        out(f"+ {T.cli.name} built 📦", fg="green")
+        out(f"+ {cli_name} built 📦", fg="green")
 
 
-@cli.command()
+@cli.command()  # type: ignore[arg-type]
 @click.argument("cli_name", type=str)
 def info(cli_name: str):
     "Display CLI info"
     metadata = get_metadata(cli_name) or exit_err(f"~ {cli_name} not loaded")
     out(f"{click.style('name:', fg='blue')} {metadata.cli_name}")
     out(f"{click.style('version:', fg='blue')} {metadata.version}")
     out(f"{click.style('requires:', fg='blue')} {metadata.requires}")
     out(f"{click.style('age:', fg='blue')} {age_datetime(metadata.loaded)} ({metadata.loaded.ctime()})")
     out(f"{click.style('manifest:', fg='blue')}\n{indent_block(metadata.manifest, spaces=2)}")
 
 
-ALIASES = {
-    "add": load,
-    "rm": remove,
-    "ls": cliffy_list,
-}
+ALIASES = {"add": load, "rm": remove, "ls": cliffy_list, "reload": update}
```

### Comparing `cliffy-0.3.2/cliffy/commander.py` & `cliffy-0.3.3/cliffy/commander.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+from __future__ import annotations
+
 from collections import defaultdict
 from typing import DefaultDict
 
 from pybash.transformer import transform as transform_bash
 from pydantic import BaseModel
 
-from .manifests import COMMAND_BLOCK, Manifest
+from .manifests import CommandBlock, Manifest
 from .parser import Parser
 
 
 class Command(BaseModel):
     name: str
-    script: COMMAND_BLOCK
+    script: CommandBlock
+
+    @classmethod
+    def from_greedy_make_lazy(cls, greedy_command: Command, group: str) -> Command:
+        lazy_command_name = greedy_command.name.replace("(*)", group)
+        lazy_command_script: CommandBlock = ""
+        if isinstance(greedy_command.script, str):
+            lazy_command_script = greedy_command.script.replace("{(*)}", group)
+        elif isinstance(greedy_command.script, list):
+            lazy_command_script = []
+            for script_block in greedy_command.script:
+                if isinstance(script_block, dict):
+                    lazy_command_script.append(script_block["help"].replace("{(*)}", group))
+                else:
+                    lazy_command_script.append(script_block.replace("{(*)}", group))
+
+        return cls(name=lazy_command_name, script=lazy_command_script)
 
 
 class CLI(BaseModel):
     name: str
     version: str
     code: str
     requires: list[str] = []
@@ -52,18 +70,19 @@
                 self.greedy.append(command)
                 continue
 
             if "." in command.name:
                 group_name = command.name.split(".")[:-1][-1]
                 groups[group_name].append(command)
             else:
-                for script_block in command.script:
-                    if isinstance(script_block, dict) and script_block.get("help"):
-                        group_help = script_block["help"]
-                        group_help_dict[command.name] = group_help
+                group_help_dict = {
+                    command.name: script_block["help"]
+                    for script_block in command.script
+                    if isinstance(script_block, dict) and script_block.get("help")
+                }
 
         for group_name, commands in groups.items():
             self.groups[group_name] = Group(
                 name=group_name, commands=commands, help=group_help_dict.get(group_name, "")
             )
 
     def generate_cli(self) -> None:
@@ -120,31 +139,20 @@
     def add_command(self, command: Command) -> None:
         if "." in command.name:
             group = command.name.split(".")[:-1][-1]
             self.add_sub_command(command, self.groups[group])
 
     def add_lazy_command(self, greedy_command: Command, group: str):
         # make it lazy and interpolate
-        lazy_command_name = greedy_command.name.replace("(*)", group)
-        lazy_command_script = ""
-        if isinstance(greedy_command.script, str):
-            lazy_command_script = greedy_command.script.replace("{(*)}", group)
-        elif isinstance(greedy_command.script, list):
-            lazy_command_script = []
-            for script_block in greedy_command.script:
-                if isinstance(script_block, dict):
-                    lazy_command_script.append(script_block["help"].replace("{(*)}", group))
-                else:
-                    lazy_command_script.append(script_block.replace("{(*)}", group))
+        lazy_command = Command.from_greedy_make_lazy(greedy_command=greedy_command, group=group)
 
         if greedy_command_args := self.manifest.args.get(greedy_command.name):
-            self.manifest.args[lazy_command_name] = greedy_command_args
+            self.manifest.args[lazy_command.name] = greedy_command_args
 
         # lazy load
-        lazy_command = Command(name=lazy_command_name, script=lazy_command_script)
         self.commands.append(lazy_command)
         self.add_command(lazy_command)
 
     def add_greedy_commands(self) -> None:
         """Greedy commands get lazy-loaded. Only supported for group-commands currently"""
         for greedy_command in self.greedy:
             if greedy_command.name.startswith("(*)"):
```

### Comparing `cliffy-0.3.2/cliffy/commanders/click.py` & `cliffy-0.3.3/cliffy/commanders/click.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 
-from ..commander import Command, Commander
+from ..commander import Command, Commander, Group
 
 
 class ClickCommander(Commander):
     """Generates commands based on the command config"""
 
     def add_base_imports(self):
         self.cli = f"""## Generated {self.manifest.name} on {datetime.datetime.now()}
@@ -25,14 +25,14 @@
         self.cli += f"""
 @cli.command()
 def {command.name}():
     \"\"\"Help for {command.name}\"\"\"
     {self.parser.parse_command(command.script)}
 """
 
-    def add_sub_command(self, command: Command, group: str):
+    def add_sub_command(self, command: Command, group: Group):
         self.cli += f"""
 @{group}.command()
 def {command.name}():
     \"\"\"Help for {command.name}\"\"\"
     {self.parser.parse_command(command.script)}
 """
```

### Comparing `cliffy-0.3.2/cliffy/commanders/typer.py` & `cliffy-0.3.3/cliffy/commanders/typer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.2/cliffy/helper.py` & `cliffy-0.3.3/cliffy/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 import os
 import platform
 import subprocess
 import sys
 from datetime import datetime
 from importlib.resources import files
 from pathlib import Path
+from tempfile import _TemporaryFileWrapper
 from typing import Any, NoReturn, Optional
 
 from click import secho
 from packaging import version
 from pydantic import BaseModel
 
-try:
-    from rich.console import Console  # type: ignore
-    from rich.table import Table  # type: ignore
-except ImportError:
-    from .rich import Console, Table
+from .rich import Console, Table
 
 HOME_PATH = str(Path.home())
 PYTHON_BIN = (
     f"{os.path.join(sys.exec_prefix, 'Scripts')}"
     if platform.system() == "Windows"
     else f"{os.path.join(sys.exec_prefix, 'bin')}"
 )
@@ -32,15 +29,15 @@
     "==": operator.eq,
     "!=": operator.ne,
     ">=": operator.ge,
     "<=": operator.le,
     "<": operator.lt,
     ">": operator.gt,
 }
-TEMP_FILES = []
+TEMP_FILES: list[_TemporaryFileWrapper] = []
 
 
 class RequirementSpec(BaseModel):
     name: str
     operator: Optional[str]
     version: Optional[str]
 
@@ -95,15 +92,15 @@
     console.print(table)
 
 
 def get_installed_package_versions() -> dict[str, str]:
     reqs = subprocess.check_output([sys.executable, "-m", "pip", "freeze"])
     installed_packages = {}
     for r in reqs.split():
-        r_spec = r.decode().split("==")
+        r_spec = r.decode().lower().split("==")
         if len(r_spec) > 1:
             installed_packages[r_spec[0]] = r_spec[1]
     return installed_packages
 
 
 def parse_requirement(requirement: str) -> RequirementSpec:
     for op in OPERATOR_MAP:
```

### Comparing `cliffy-0.3.2/cliffy/homer.py` & `cliffy-0.3.3/cliffy/homer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.2/cliffy/loader.py` & `cliffy-0.3.3/cliffy/loader.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.2/cliffy/manifests/v1.py` & `cliffy-0.3.3/cliffy/manifests/v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Any, Literal, Union
 from pydantic import BaseModel, Field
 
 from ..helper import wrap_as_comment, wrap_as_var
 
-COMMAND_BLOCK = Union[str, list[Union[str, dict[Literal["help"], str]]]]
+CommandBlock = Union[str, list[Union[str, dict[Literal["help"], str]]]]
 
 
 class CLIManifest(BaseModel):
     name: str = Field(
         description="The name of the CLI. "
         "This will be used as the script name when invoking the CLI from the command line."
     )
@@ -34,15 +34,15 @@
     vars: dict[str, Union[str, dict[str, None]]] = Field(
         {},
         description="A mapping defining manifest variables that can be referenced in any other blocks. "
         "Environments variables can be used in this section with ${some_env_var} for dynamic parsing. "
         "Supports jinja2 formatted expressions as values. "
         "Interpolate defined vars in other blocks jinja2-styled {{ var_name }}.",
     )
-    commands: dict[str, COMMAND_BLOCK] = Field(
+    commands: dict[str, CommandBlock] = Field(
         {},
         description="A mapping containing the command definitions for the CLI. "
         "Each command should have a unique key- which can be either a group command or nested subcommands. "
         "Nested subcommands are joined by '.' in between each level. "
         "A special (*) wildcard can be used to spread the subcommand to all group-level commands. "
         "The value is the python code to run when the command is called "
         "OR a list of bash commands to run (prefixed with $).",
```

### Comparing `cliffy-0.3.2/cliffy/parser.py` & `cliffy-0.3.3/cliffy/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pybash.transformer import transform as transform_bash
 
 from .manifests import Manifest
 
 
 class Parser:
-
     __slots__ = ("manifest",)
 
     def __init__(self, manifest: Manifest) -> None:
         self.manifest = manifest
 
     def is_param_required(self, param_type: str) -> bool:
         return (
```

### Comparing `cliffy-0.3.2/cliffy/transformer.py` & `cliffy-0.3.3/cliffy/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def validate_cli_requires(self) -> None:
         if not self.manifest.requires:
             return
 
         installed_package_versions = get_installed_package_versions()
         for dep in self.manifest.requires:
             dep_spec = parse_requirement(dep)
-            if dep_spec.name not in installed_package_versions:
+            if dep_spec.name.lower() not in installed_package_versions:
                 exit_err(f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed")
 
             if dep_spec.version and not compare_versions(
                 installed_package_versions[dep_spec.name], dep_spec.version, dep_spec.operator
             ):
                 exit_err(
                     f"~ missing requirement: `{self.manifest_io.name}` requires `{dep}` to be installed"
```

### Comparing `cliffy-0.3.2/PKG-INFO` & `cliffy-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.3.2
+Version: 0.3.3
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: rich
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pybash (>=0.3.4,<0.4.0)
-Requires-Dist: pydantic (>=2.0a4)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "rich"
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) ; extra == "rich"
 Requires-Dist: shiv (>=1.0.3,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
 Description-Content-Type: text/markdown
@@ -34,42 +34,14 @@
 ## Features
 * Rapidly build CLIs with YAML-defined manifests
 * Manage CLIs- load, list, update, and remove
 * Built-in shell and Python scripting support
 * Supports Jinja2-templating
 * Build and bundle CLIs into self-contained, portable zipapps
 
-## Install
-* `pip install "cliffy[rich]"` to include [rich-click](https://github.com/ewels/rich-click) for colorful CLI help output formatted with [rich](https://github.com/Textualize/rich).
-
-or 
-
-* `pip install cliffy`
-
-## How it works
-1. Define CLI manifests in YAML files
-2. Run `cli` commands to load, build, and manage CLIs
-3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
-4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
-5. Run loaded CLIs straight from the terminal
-6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
-
-## Usage
-`cli <command>`
-* `init <cli name> --raw`: Generate a template CLI manifest for a new CLI
-* `load <manifest>`: Add a new CLI based on the manifest
-* `render <manifest>`: View generated CLI script for a manifest
-* `list` or `ls`: Output a list of loaded CLIs 
-* `update <cli name>`: Reload a loaded CLI
-* `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
-* `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
-* `build <manifest>`: Build a CLI manifest into a self-contained zipapp
-* `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
-* `info <cli name>`: Display CLI metadata
-
 ### Load
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
 version: 0.1.0
@@ -126,16 +98,43 @@
 Builds a portable zipapp containing the CLI and its package requirements.
 
 3. Run CLI
 ```
 ./dist/requires -h
 ```
 
+## Usage
+`cli <command>`
+* `init <cli name> --raw`: Generate a template CLI manifest for a new CLI
+* `load <manifest>`: Add a new CLI based on the manifest
+* `render <manifest>`: View generated CLI script for a manifest
+* `list` or `ls`: Output a list of loaded CLIs 
+* `update <cli name>`: Reload a loaded CLI
+* `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
+* `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
+* `build <cli name or manifest>`: Build a CLI manifest or a loaded CLI into a self-contained zipapp
+* `info <cli name>`: Display CLI metadata
+
+## How it works
+1. Define CLI manifests in YAML files
+2. Run `cli` commands to load, build, and manage CLIs
+3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
+4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
+5. Run loaded CLIs straight from the terminal
+6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
+
+## Install
+* `pip install "cliffy[rich]"` to include [rich-click](https://github.com/ewels/rich-click) for colorful CLI help output formatted with [rich](https://github.com/Textualize/rich).
+
+or 
+
+* `pip install cliffy`
+
 ## Manifest template
-Generated by `cli init`:
+Generated by `cli init`. For a barebones template, run `cli init --raw`
 ```yaml
 # cliffy v1 template
 manifestVersion: v1
 
 # The name of the CLI
 # This will be used as the script name when invoking the CLI from the command line.
 name: cliffy 
@@ -210,15 +209,14 @@
     # this is a nested command that will get invoked with: hello greet all
     greet.all: 
         - help: Help text for list.all       # you can also define help text like this
         - $ echo "hello all"                 # this is a bash command that will get converted to python subprocess call
         - print("greetings from python")     # this python code will get directly invoked
 
 ```
-For a barebones template: `cli init --raw`
 
 ## Development
 ```
 poetry shell
 cli -h
 ```
```

