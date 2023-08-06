# Comparing `tmp/reflekt-0.3.8.tar.gz` & `tmp/reflekt-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflekt-0.3.8.tar", max compression
+gzip compressed data, was "reflekt-0.3.9.tar", max compression
```

## Comparing `reflekt-0.3.8.tar` & `reflekt-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11345 2023-02-07 02:45:59.313697 reflekt-0.3.8/LICENSE
-drwxr-xr-x   0        0        0        0 2023-02-07 02:45:59.313793 reflekt-0.3.8/LICENSES/
--rw-r--r--   0        0        0    35969 2023-02-28 16:04:44.899999 reflekt-0.3.8/README.md
--rw-r--r--   0        0        0     2081 2023-03-04 17:39:15.443591 reflekt-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      307 2023-03-04 17:39:15.444245 reflekt-0.3.8/reflekt/__init__.py
--rw-r--r--   0        0        0       29 2023-02-07 02:45:59.330447 reflekt-0.3.8/reflekt/_templates/dbt_package/.gitignore
--rw-r--r--   0        0        0     1908 2023-02-09 06:57:26.831104 reflekt-0.3.8/reflekt/_templates/dbt_package/README.md
--rw-r--r--   0        0        0      323 2023-02-07 02:45:59.331425 reflekt-0.3.8/reflekt/_templates/dbt_package/dbt_project.yml
--rw-r--r--   0        0        0        0 2023-02-07 02:45:59.331584 reflekt-0.3.8/reflekt/_templates/dbt_package/models/.gitkeep
--rw-r--r--   0        0        0      135 2023-02-07 02:45:59.332111 reflekt-0.3.8/reflekt/_templates/reflekt_project/.gitignore
--rw-r--r--   0        0        0     1919 2023-02-27 06:05:53.835874 reflekt-0.3.8/reflekt/_templates/reflekt_project/README.md
--rw-r--r--   0        0        0        0 2023-02-07 02:45:59.332794 reflekt-0.3.8/reflekt/_templates/reflekt_project/artifacts/.gitkeep
--rw-r--r--   0        0        0        0 2023-02-07 02:45:59.332941 reflekt-0.3.8/reflekt/_templates/reflekt_project/schemas/.gitkeep
--rw-r--r--   0        0        0     2034 2023-02-27 06:05:53.837080 reflekt-0.3.8/reflekt/_templates/reflekt_project/schemas/.reflekt/meta/1-0.json
--rw-r--r--   0        0        0     3950 2023-02-27 06:05:53.838130 reflekt-0.3.8/reflekt/_validation/profile/1-0.json
--rw-r--r--   0        0        0     5004 2023-02-27 06:05:53.838920 reflekt-0.3.8/reflekt/_validation/project/1-0.json
--rw-r--r--   0        0        0      109 2023-02-07 02:45:59.335607 reflekt-0.3.8/reflekt/builder/__init__.py
--rw-r--r--   0        0        0    15184 2023-03-04 17:39:15.445071 reflekt-0.3.8/reflekt/builder/_schemas/segment_common/1-0.json
--rw-r--r--   0        0        0    30153 2023-03-04 17:39:15.445949 reflekt-0.3.8/reflekt/builder/dbt.py
--rw-r--r--   0        0        0     3349 2023-02-26 02:34:09.682682 reflekt-0.3.8/reflekt/builder/handler.py
--rw-r--r--   0        0        0     1972 2023-02-07 02:45:59.337068 reflekt-0.3.8/reflekt/casing.py
--rw-r--r--   0        0        0    21146 2023-03-04 09:08:38.316657 reflekt-0.3.8/reflekt/cli.py
--rw-r--r--   0        0        0     1186 2023-02-27 06:05:53.843065 reflekt-0.3.8/reflekt/constants.py
--rw-r--r--   0        0        0      668 2023-02-07 02:45:59.338778 reflekt-0.3.8/reflekt/dumper.py
--rw-r--r--   0        0        0     2380 2023-02-07 02:45:59.339430 reflekt-0.3.8/reflekt/errors.py
--rw-r--r--   0        0        0     5216 2023-02-07 02:45:59.339982 reflekt-0.3.8/reflekt/flatson.py
--rw-r--r--   0        0        0    11614 2023-02-27 06:05:53.843916 reflekt-0.3.8/reflekt/linter.py
--rw-r--r--   0        0        0     5269 2023-02-27 06:05:53.844620 reflekt-0.3.8/reflekt/profile.py
--rw-r--r--   0        0        0     9254 2023-02-27 06:05:53.845353 reflekt-0.3.8/reflekt/project.py
--rw-r--r--   0        0        0      109 2023-02-07 02:45:59.342067 reflekt-0.3.8/reflekt/registry/__init__.py
--rw-r--r--   0        0        0     9136 2023-02-27 06:05:53.846371 reflekt-0.3.8/reflekt/registry/avo.py
--rw-r--r--   0        0        0     1886 2023-02-07 02:45:59.343307 reflekt-0.3.8/reflekt/registry/handler.py
--rw-r--r--   0        0        0    20026 2023-02-27 06:05:53.847252 reflekt-0.3.8/reflekt/registry/segment.py
--rw-r--r--   0        0        0     3185 2023-02-27 06:05:53.848050 reflekt-0.3.8/reflekt/tracking.py
--rw-r--r--   0        0        0     5017 2023-03-04 01:30:52.430991 reflekt-0.3.8/reflekt/warehouse.py
--rw-r--r--   0        0        0    38408 1970-01-01 00:00:00.000000 reflekt-0.3.8/setup.py
--rw-r--r--   0        0        0    37453 1970-01-01 00:00:00.000000 reflekt-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-02-07 02:45:59.313697 reflekt-0.3.9/LICENSE
+drwxr-xr-x   0        0        0        0 2023-02-07 02:45:59.313793 reflekt-0.3.9/LICENSES/
+-rw-r--r--   0        0        0    35969 2023-02-28 16:04:44.899999 reflekt-0.3.9/README.md
+-rw-r--r--   0        0        0     2081 2023-03-04 18:51:30.317160 reflekt-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-03-04 18:51:30.317489 reflekt-0.3.9/reflekt/__init__.py
+-rw-r--r--   0        0        0       29 2023-02-07 02:45:59.330447 reflekt-0.3.9/reflekt/_templates/dbt_package/.gitignore
+-rw-r--r--   0        0        0     1908 2023-02-09 06:57:26.831104 reflekt-0.3.9/reflekt/_templates/dbt_package/README.md
+-rw-r--r--   0        0        0      323 2023-02-07 02:45:59.331425 reflekt-0.3.9/reflekt/_templates/dbt_package/dbt_project.yml
+-rw-r--r--   0        0        0        0 2023-02-07 02:45:59.331584 reflekt-0.3.9/reflekt/_templates/dbt_package/models/.gitkeep
+-rw-r--r--   0        0        0      135 2023-02-07 02:45:59.332111 reflekt-0.3.9/reflekt/_templates/reflekt_project/.gitignore
+-rw-r--r--   0        0        0     1919 2023-02-27 06:05:53.835874 reflekt-0.3.9/reflekt/_templates/reflekt_project/README.md
+-rw-r--r--   0        0        0        0 2023-02-07 02:45:59.332794 reflekt-0.3.9/reflekt/_templates/reflekt_project/artifacts/.gitkeep
+-rw-r--r--   0        0        0        0 2023-02-07 02:45:59.332941 reflekt-0.3.9/reflekt/_templates/reflekt_project/schemas/.gitkeep
+-rw-r--r--   0        0        0     2034 2023-02-27 06:05:53.837080 reflekt-0.3.9/reflekt/_templates/reflekt_project/schemas/.reflekt/meta/1-0.json
+-rw-r--r--   0        0        0     3950 2023-02-27 06:05:53.838130 reflekt-0.3.9/reflekt/_validation/profile/1-0.json
+-rw-r--r--   0        0        0     5004 2023-02-27 06:05:53.838920 reflekt-0.3.9/reflekt/_validation/project/1-0.json
+-rw-r--r--   0        0        0      109 2023-02-07 02:45:59.335607 reflekt-0.3.9/reflekt/builder/__init__.py
+-rw-r--r--   0        0        0    15184 2023-03-04 17:39:15.445071 reflekt-0.3.9/reflekt/builder/_schemas/segment_common/1-0.json
+-rw-r--r--   0        0        0    30225 2023-03-04 18:37:31.576061 reflekt-0.3.9/reflekt/builder/dbt.py
+-rw-r--r--   0        0        0     3349 2023-02-26 02:34:09.682682 reflekt-0.3.9/reflekt/builder/handler.py
+-rw-r--r--   0        0        0     1972 2023-02-07 02:45:59.337068 reflekt-0.3.9/reflekt/casing.py
+-rw-r--r--   0        0        0    21149 2023-03-04 18:33:11.842366 reflekt-0.3.9/reflekt/cli.py
+-rw-r--r--   0        0        0     1186 2023-02-27 06:05:53.843065 reflekt-0.3.9/reflekt/constants.py
+-rw-r--r--   0        0        0      668 2023-02-07 02:45:59.338778 reflekt-0.3.9/reflekt/dumper.py
+-rw-r--r--   0        0        0     2380 2023-02-07 02:45:59.339430 reflekt-0.3.9/reflekt/errors.py
+-rw-r--r--   0        0        0     5216 2023-02-07 02:45:59.339982 reflekt-0.3.9/reflekt/flatson.py
+-rw-r--r--   0        0        0    11614 2023-02-27 06:05:53.843916 reflekt-0.3.9/reflekt/linter.py
+-rw-r--r--   0        0        0     5269 2023-02-27 06:05:53.844620 reflekt-0.3.9/reflekt/profile.py
+-rw-r--r--   0        0        0     9254 2023-02-27 06:05:53.845353 reflekt-0.3.9/reflekt/project.py
+-rw-r--r--   0        0        0      109 2023-02-07 02:45:59.342067 reflekt-0.3.9/reflekt/registry/__init__.py
+-rw-r--r--   0        0        0     9136 2023-02-27 06:05:53.846371 reflekt-0.3.9/reflekt/registry/avo.py
+-rw-r--r--   0        0        0     1886 2023-02-07 02:45:59.343307 reflekt-0.3.9/reflekt/registry/handler.py
+-rw-r--r--   0        0        0    20026 2023-02-27 06:05:53.847252 reflekt-0.3.9/reflekt/registry/segment.py
+-rw-r--r--   0        0        0     3185 2023-02-27 06:05:53.848050 reflekt-0.3.9/reflekt/tracking.py
+-rw-r--r--   0        0        0     5017 2023-03-04 01:30:52.430991 reflekt-0.3.9/reflekt/warehouse.py
+-rw-r--r--   0        0        0    38408 1970-01-01 00:00:00.000000 reflekt-0.3.9/setup.py
+-rw-r--r--   0        0        0    37453 1970-01-01 00:00:00.000000 reflekt-0.3.9/PKG-INFO
```

### Comparing `reflekt-0.3.8/LICENSE` & `reflekt-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/README.md` & `reflekt-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/pyproject.toml` & `reflekt-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflekt"
-version = "0.3.8"
+version = "0.3.9"
 description = "A CLI tool to define event schemas, lint them, interact with schema registries, and build corresponding data artifacts (e.g., dbt package)."
 license = "Apache-2.0"
 authors = ["Gregory Clunies <greg.clunies@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/GClunies/Reflekt"
 keywords = ["events", "jsonchema", "analytics", "business-intelligence", "data-modeling", "dbt", "snowflake", "redshift", "segment", "avo"]
 include = ["reflekt/_templates/**/*", "reflekt/_validation/**/*"]
```

### Comparing `reflekt-0.3.8/reflekt/_templates/dbt_package/README.md` & `reflekt-0.3.9/reflekt/_templates/dbt_package/README.md`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/_templates/reflekt_project/README.md` & `reflekt-0.3.9/reflekt/_templates/reflekt_project/README.md`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/_templates/reflekt_project/schemas/.reflekt/meta/1-0.json` & `reflekt-0.3.9/reflekt/_templates/reflekt_project/schemas/.reflekt/meta/1-0.json`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/_validation/profile/1-0.json` & `reflekt-0.3.9/reflekt/_validation/profile/1-0.json`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/_validation/project/1-0.json` & `reflekt-0.3.9/reflekt/_validation/project/1-0.json`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/builder/_schemas/segment_common/1-0.json` & `reflekt-0.3.9/reflekt/builder/_schemas/segment_common/1-0.json`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/builder/dbt.py` & `reflekt-0.3.9/reflekt/builder/dbt.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,17 +227,17 @@
                 ]:
                     alias_name = col_name.replace("timestamp", "tstamp").replace(
                         "_at", "_at_tstamp"
                     )
                     taken_cols.append(alias_name)
                     col_sql = f"\n        {col_name} as {alias_name},"
                 elif "context_" in col_name:  # Context columns
-                    alias_name = f"{col_name.replace('context_', '')},"
+                    alias_name = f"{col_name.replace('context_', '')}"
                     taken_cols.append(alias_name)
-                    col_sql = f"\n        {col_name} as {alias_name}"
+                    col_sql = f"\n        {col_name} as {alias_name},"
                 else:  # Other columns (i.e., from schema properties)
                     if col_name in taken_cols or col_name in [
                         "call_type",
                         "source_schema",
                         "source_table",
                         "schema_id",
                     ]:
@@ -592,14 +592,15 @@
 
                     # Build users table/model/doc (use columns from identifies table)
                     logger.info(
                         "Building dbt artifacts for schema: "
                         "[magenta]Segment 'users' table[magenta/]"
                     )
 
+                    # Search users table for columns in identify schema
                     columns, warehouse_error = self.warehouse.find_columns(
                         table_name="users",
                         columns_to_search=columns_to_search,
                     )
 
                     if warehouse_error is not None:
                         self.warehouse_errors.append(warehouse_error)
```

### Comparing `reflekt-0.3.8/reflekt/builder/handler.py` & `reflekt-0.3.9/reflekt/builder/handler.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/casing.py` & `reflekt-0.3.9/reflekt/casing.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/cli.py` & `reflekt-0.3.9/reflekt/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,12 +610,12 @@
     #     source="snowflake.raw.ecomm_demo",
     #     sdk="segment",
     #     profile_name=None,  # Must have value when using Vscode debugger
     # )
 
     build(
         artifact="dbt",
-        select="segment/buoyweather-web",
-        source="snowflake.raw.buoyweather",
+        select="segment/surfline-web/identify",
+        source="snowflake.raw.surfline",
         sdk="segment",
         profile_name="wavetrak_segment",  # Must have value when using Vscode debugger
     )
```

### Comparing `reflekt-0.3.8/reflekt/constants.py` & `reflekt-0.3.9/reflekt/constants.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/dumper.py` & `reflekt-0.3.9/reflekt/dumper.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/errors.py` & `reflekt-0.3.9/reflekt/errors.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/flatson.py` & `reflekt-0.3.9/reflekt/flatson.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/linter.py` & `reflekt-0.3.9/reflekt/linter.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/profile.py` & `reflekt-0.3.9/reflekt/profile.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/project.py` & `reflekt-0.3.9/reflekt/project.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/registry/avo.py` & `reflekt-0.3.9/reflekt/registry/avo.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/registry/handler.py` & `reflekt-0.3.9/reflekt/registry/handler.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/registry/segment.py` & `reflekt-0.3.9/reflekt/registry/segment.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/tracking.py` & `reflekt-0.3.9/reflekt/tracking.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/reflekt/warehouse.py` & `reflekt-0.3.9/reflekt/warehouse.py`

 * *Files identical despite different names*

### Comparing `reflekt-0.3.8/setup.py` & `reflekt-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
  'typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['reflekt = reflekt.cli:app']}
 
 setup_kwargs = {
     'name': 'reflekt',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'A CLI tool to define event schemas, lint them, interact with schema registries, and build corresponding data artifacts (e.g., dbt package).',
     'long_description': '<!--\nSPDX-FileCopyrightText: 2022 Gregory Clunies <greg@reflekt-ci.com>\n\nSPDX-License-Identifier: Apache-2.0\n-->\n\n# Reflekt\n![PyPI](https://img.shields.io/pypi/v/reflekt?style=for-the-badge)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reflekt?style=for-the-badge)\n![GitHub](https://img.shields.io/github/license/gclunies/reflekt?style=for-the-badge)\n\n> ***Product analytics is a team sport***\n\nReflekt helps Data, Engineering, and Product teams work together to define, manage, and model events for product analytics. Reflekt integrates with [schema registries](#interacting-with-schema-registries), cloud [data warehouses]((#supported-data-warehouses)), and [dbt](#dbt-artifacts).\n\n- Define event schemas (aka data contracts) as `code` using [jsonschema](https://json-schema.org/). Schemas are version controlled, and stored in a GitHub repo.\n- Configure naming and metadata conventions for events and properties. Lint schemas to test for compliance.\n- Open pull requests (PRs) to propose schema changes, get input, and request reviews.\n- Easily build a CI suite to [lint](#linting-schemas) schemas, [push](#push-schemas-to-a-registry) them to a schema registry, and [build corresponding dbt artifacts](#building-private-dbt-packages).\n\nhttps://user-images.githubusercontent.com/28986302/217134526-df83ec90-86f3-491e-9588-b7cd56956db1.mp4\n\n## Table of Contents\n- [Getting Started](#usage)<br>\n  - [Installation](#installation)<br>\n  - [Reflekt `--help`](#reflekt-help)<br>\n  - [Creating a project](#creating-a-project)<br>\n  - [Project configuration](#project-configuration)<br>\n- [Using Reflekt](#using-schemas)<br>\n  - [Defining schemas](#defining-schemas)<br>\n  - [Identifying and selecting schemas](#identifying-and-selecting-schemas)<br>\n  - [Schema versions](#schema-versions)<br>\n  - [Linting schemas](#linting-schemas)<br>\n  - [Interacting with schema registries](#interacting-with-schema-registries)<br>\n  - [Building dbt artifacts](#dbt-artifacts)<br>\n  - [Supported data warehouses](#supported-data-warehouses)<br>\n\n## Getting Started\n\n### Installation\nReflekt is available on [PyPI](https://pypi.org/project/my-reflekt-project/). Install with `pip` (or package manager of choice), preferably in a virtual environment:\n```bash\n❯ source /path/to/venv/bin/activate  # Activate virtual environment\n❯ pip install reflekt                # Install Reflekt\n❯ reflekt --version                  # Confirm installation\nReflekt CLI Version: 0.3.1\n```\n\n### Reflekt `--help`\nThe `--help` flag provides an overview of available `reflekt` commands.\n```bash\n❯ reflekt --help  # Show general --help details\n\n Usage: reflekt [OPTIONS] COMMAND [ARGS]...\n\n Reflekt CLI.\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --version                                                                                                                                                        │\n│ --install-completion        [bash|zsh|fish|powershell|pwsh]  Install completion for the specified shell. [default: None]                                         │\n│ --show-completion           [bash|zsh|fish|powershell|pwsh]  Show completion for the specified shell, to copy it or customize the installation. [default: None]  │\n│ --help                                                       Show this message and exit.                                                                         │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ build             Build data artifacts based on schemas.                                                                                                         │\n│ debug             Check Reflekt project configuration.                                                                                                           │\n│ init              Initialize a Reflekt project.                                                                                                                  │\n│ lint              Lint schema(s) to test for naming and metadata conventions.                                                                                    │\n│ pull              Pull schema(s) from a schema registry.                                                                                                         │\n│ push              Push schema(s) to a schema registry.                                                                                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\nEach command also has a `--help` flag providing command details (arguments, options, syntax, etc.).\n```bash\n❯ reflekt lint --help  # Show --help details for `reflekt lint`\n\n Usage: reflekt lint [OPTIONS]\n\n Lint schema(s) to test for naming and metadata conventions.\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *  --select  -s      TEXT  Schema(s) to lint. [default: None] [required]                                                                                         │\n│    --help                  Show this message and exit.                                                                                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### Creating a project\nCreate a new directory, initialize a new Git repo, and run `reflekt init` to create a new Reflekt project.\n```bash\n❯ mkdir ~/Repos/my-reflekt-project  # Create a new directory for the project\n❯ cd ~/Repos/my-reflekt-project     # Navigate to the project directory\n❯ git init                          # Initialize a new Git repo\n❯ reflekt init --dir .              # Initialize a new Reflekt project in the current directory\n\n# Follow the prompts to configure the project\n```\n\nThis will create a new Reflekt project with the following structure:\n```bash\nmy-reflekt-project\n├── .logs/                # Reflekt command logs\n├── .reflekt_cache/       # Local cache used by Reflekt\n├── artifacts/            # Where Reflekt builds data artifacts (i.e., dbt packages)\n├── schemas/              # Where event schemas are defined and stored\n├── .gitignore\n├── README.md\n└── reflekt_project.yml   # Project configuration\n```\n\n### Project configuration\nReflekt uses 3 files to configure a project: `reflekt_project.yml`, `reflekt_profiles.yml`, and `schemas/.reflekt/meta/1-0.json`. Under the hood, Reflekt validates these configuration files before running, raising errors if an invalid configuration is detected. Examples of each file with configuration details are found below.\n\n#### **reflekt_project.yml**\nContains general project settings as well as configuration for schema conventions, schema registry details (if needed), and data artifact generation. Click to expand the example below with details on each setting.\n\n<details>\n<summary><code>example_reflekt_project.yml</code>(CLICK TO EXPAND)</summary>\n<br>\n\n```yaml\n# Example reflekt_project.yml\n# GENERAL CONFIG ----------------------------------------------------------------------\nversion: 1.0\n\nname: reflekt_demo              # Project name\nvendor: com.company_name        # Default vendor for schemas in reflekt project\ndefault_profile: dev_reflekt    # Default profile to use from reflekt_profiles.yml\nprofiles_path: ~/.reflekt/reflekt_profiles.yml  # Path to reflekt_profiles.yml\n\n# SCHEMAS CONFIG ----------------------------------------------------------------------\nschemas:                        # Define schema conventions\n  conventions:\n    event:\n      casing: title             # title | snake | camel | any\n      capitalize_camel: true    # Only applies if \'casing: camel\'\n      numbers: false            # Allow numbers in event names\n      reserved: []              # Reserved event names\n    property:\n      casing: snake             # title | snake | camel | any\n      capitalize_camel: true    # Only applies if \'casing: camel\'\n      numbers: false            # Allow numbers in property names\n      reserved: []              # Reserved property names\n    data_types: [               # Allowed data types\n        string, integer, number, boolean, object, array, any, \'null\'\n    ]\n\n# REGISTRY CONFIG ---------------------------------------------------------------------\nregistry:                       # Additional config for schema registry if needed\n  avo:                          # Avo specific config\n    branches:                   # Provide ID for Avo branches for `reflekt pull` to work\n      staging: AbC12dEfG        # Safe to version control (See Avo docs to find branch ID: https://bit.ly/avo-docs-branch-id)\n      main: main                # \'main\' always refers to the main branch\n\n# ARTIFACTS CONFIG -----------------------------------------------------------------------\nartifacts:                      # Configure how data artifacts are built\n  dbt:                          # dbt package config\n    sources:\n      prefix: __src_            # Source files will start with this prefix\n    models:\n      prefix: stg_              # Model files will start with this prefix\n    docs:\n      prefix: _stg_             # Docs files will start with this prefix\n      in_folder: false          # Docs files in separate folder?\n      tests:                    # dbt tests to add based on column name (can be empty dict {})\n        id: [unique, not_null]\n\n```\n</details>\n<br>\n\n#### **reflekt_profiles.yml**\nContains connection details for schema registries (used to validate event data) and data sources (i.e., data warehouse with raw event data). Click to expand the example below with details on each setting.\n<details>\n<summary><code>example_reflekt_profiles.yml</code>(CLICK TO EXPAND)</summary>\n<br>\n\n```yaml\n# Example reflekt_profiles.yml\nversion: 1.0\n\ndev_reflekt:                                              # Profile name (multiple profiles can be defined)\n  # Define connections to schema registries (multiple allowed)\n  registry:\n    - type: segment\n      api_token: segment_api_token                        # https://docs.segmentapis.com/tag/Getting-Started#section/Get-an-API-token\n    - type: avo\n      workspace_id: avo_workspace_id                      # https://www.avo.app/docs/public-api/export-tracking-plan#endpoint\n      service_account_name: avo_service_account_name      # https://www.avo.app/docs/public-api/authentication#creating-service-accounts\n      service_account_secret: avo_service_account_secret\n\n  # Connections to data sources (data warehouses) where event data is stored.\n  # Sources are uniquely identified by their ID and are used in the `--source` arg when running `reflekt build`.\n  source:\n    - id: snowflake             # For simplicity, we use the same ID as the source type.\n      type: snowflake           # Snowflake DWH. Credentials follow.\n      account: abc12345\n      database: raw\n      warehouse: transforming\n      role: transformer\n      user: reflekt_user\n      password: reflekt_user_password\n\n    - id: redshift              # For simplicity, we use the same ID as the source type.\n      type: redshift            # Redshift DWH. Credentials follow.\n      host: example-redshift-cluster-1.abc123.us-west-1.redshift.amazonaws.com\n      database: analytics\n      port: 5439\n      user: reflekt_user\n      password: reflekt_user_password\n\n```\n</details>\n<br>\n\n#### **schemas/.reflekt/meta/1-0.json**\nA meta-schema used to validate all event schemas in the project. Under the hood, Reflekt uses this meta-schema along with the naming conventions defined in the `reflekt_project.yml` file to validate all event schemas.\n\nTo define ***required metadata*** for all event schemas in your project, you can update the `metadata` object in `schemas/.reflekt/meta/1-0.json`. See the example below showing how to require both **code owner** and **product owner** metadata.\n\n<details>\n<summary><code>schemas/.reflekt/meta/1-0.json</code>(CLICK TO EXPAND)</summary>\n<br>\n\n```json\n{\n    "$schema": "http://json-schema.org/draft-07/schema#",\n    "$id": ".reflekt/meta/1-0.json",\n    "description": "Meta-schema for all Reflekt events",\n    "self": {\n        "vendor": "reflekt",\n        "name": "meta",\n        "format": "jsonschema",\n        "version": "1-0"\n    },\n    "type": "object",\n    "allOf": [\n        {\n            "$ref": "http://json-schema.org/draft-07/schema#"\n        },\n        {\n            "properties": {\n                "self": {\n                    "type": "object",\n                    "properties": {\n                        "vendor": {\n                            "type": "string",\n                            "description": "The company, application, team, or system that authored the schema (e.g., com.company, com.company.android, com.company.marketing)"\n                        },\n                        "name": {\n                            "type": "string",\n                            "description": "The schema name. Describes what the schema is meant to capture (e.g., pageViewed, clickedLink)"\n                        },\n                        "format": {\n                            "type": "string",\n                            "description": "The format of the schema",\n                            "const": "jsonschema"\n                        },\n                        "version": {\n                            "type": "string",\n                            "description": "The schema version, in MODEL-ADDITION format (e.g., 1-0, 1-1, 2-3, etc.)",\n                            "pattern": "^[1-9][0-9]*-(0|[1-9][0-9]*)$"\n                        },\n                        "metadata": {  // EXAMPLE: Defining required metadata (code_owner, product_owner)\n                            "type": "object",\n                            "description": "Required metadata for all event schemas",\n                            "properties": {\n                                "code_owner": {"type": "string"},\n                                "product_owner": {"type": "string"}\n                            },\n                            "required": ["code_owner", "product_owner"],\n                            "additionalProperties": false\n                        },\n                    },\n                    "required": ["vendor", "name", "format", "version"],\n                    "additionalProperties": false\n                },\n                "properties": {},\n                "tests": {},\n            },\n            "required": ["self", "metadata", "properties"]\n        }\n    ]\n}\n\n```\n\n</details>\n\n<br>\n<br>\n\n## Using Reflekt\n### Defining schemas\nEvent schemas are defined using [jsonschema](https://json-schema.org/). Each schema is defined as a separate JSON file, stored in the `schemas/` directory of a Reflekt project. An example `ProductClicked` event schema is shown below.\n\n<details>\n<summary><code>my-reflekt-project/schemas/segment/ecommerce/ProductClicked/1-0.json</code>(CLICK TO EXPAND)</summary>\n<br>\n\n```json\n{\n  "$id": "segment/ecommerce/ProductClicked/1-0.json",    // Unique ID for the schema\n  "$schema": "http://json-schema.org/draft-07/schema#",  // JSON Schema version\n  "self": {\n      "vendor": "com.company_name",  // Company, application, team, or system that authored the schema\n      "name": "ProductClicked",      // Name of the event\n      "format": "jsonschema",        // Format of the schema\n      "version": "1-0",              // Version of the schema\n      "metadata": {                  // Metadata for the event\n          "code_owner": "engineering/ecommerce-squad",\n          "product_owner": "product_manager_name@company_name.com",\n      }\n  },\n  "type": "object",\n  "properties": {                   // Properties of the event\n      "product_id": {\n          "type": "string",\n          "description": "Database id of the product being viewed"\n      },\n      "sku": {\n          "type": "string",\n          "description": "Sku of the product being viewed"\n      },\n      "category": {\n          "type": "string",\n          "description": "Category of the product being viewed"\n      },\n      "name": {\n          "type": "string",\n          "description": "Name of the product being viewed"\n      },\n      "brand": {\n          "type": "string",\n          "description": "Brand of the product being viewed"\n      },\n      "variant": {\n          "type": "string",\n          "description": "Variant of the product being viewed"\n      },\n      "price": {\n          "type": "number",\n          "description": "Price of the product ($) being viewed"\n      },\n      "quantity": {\n          "type": "integer",\n          "description": "Quantity of the product being viewed"\n      },\n      "coupon": {\n          "type": "string",\n          "description": "Coupon code associated with a product (for example, MAY_DEALS_3)"\n      },\n      "position": {\n          "type": "integer",\n          "description": "Position in the product list (ex. 3)"\n      },\n      "url": {\n          "type": "string",\n          "description": "URL of the product being viewed"\n      },\n      "image_url": {\n          "type": "string",\n          "description": "URL of the product image being viewed"\n      },\n  },\n\n  "required": [                    // Required properties\n      "product_id",\n      "sku",\n      "category",\n      "name",\n      "brand",\n      "price",\n      "quantity"\n  ],\n  "additionalProperties": false,   // No additional properties allowed\n}\n```\n\n</details>\n<br>\n\n### Identifying and selecting schemas\nSchemas are uniquely identified by their `$id`, which is determine by their path relative to the `schemas/` directory. For example:\n\n| Path to schema                                                      | Schema `$id`                             |\n|---------------------------------------------------------------------|------------------------------------------|\n| `my-reflekt-project/schemas/segment/ecommerce/CartViewed/1-0.json`  | `segment/ecommerce/CartViewed/1-0.json`  |\n| `my-reflekt-project/schemas/segment/ecommerce/LinkClicked/2-1.json` | `segment/ecommerce/LinkClicked/2-1.json` |\n\nThese `$id`s are used to `--select` schemas when running Reflekt commands. For example:\n\n```bash\n❯ reflekt lint --select segment/ecommerce/CartViewed/1-0.json      # Lint version 1-0 of the CartViewed schema\n❯ reflekt lint --select "segment/ecommerce/Link Clicked/2-1.json"  # $ids with spaces must be surrounded by quotes\n❯ reflekt lint --select segment/ecommerce                          # Lint all schemas in the segment/ecommerce directory\n```\n\n### Schema versions\nAs data collection requirements change, event schemas must be updated to *reflekt* the new schema. Reflekt supports schema evolution by defining a `version` for each schema, starting at `1-0` and following a `MAJOR-MINOR` version spec. The definition of `MAJOR` and `MINOR` is as follows:\n\n- **MAJOR** - Breaking schema changes incompatible with previous data. Examples:\n  - Add/remove/rename a required property\n  - Change a property from *optional to required*\n  - Change a property\'s type\n- **MINOR** - Non-breaking schema changes compatible with previous data. Examples:\n  - Add/remove/rename an optional property\n  - Change a property from *required to optional*\n\nWhen defining a new schema version, **create a new file** with the incremented version and updated schema definition.\n\n### Interacting with schema registries\nSchema registries are used to store and serve schemas. Once a schema is in a registry, it can be used to validate event data against the schema to ensure event data quality. Reflekt supports interacting with schema registries to push (publish) and pull (retrieve) schemas. Currently, the following registries are supported:\n\n| **Registry**          | **`--push` support** | **`--pull` support** | **Schema `--select` syntax**            | **Schema `version` support**                                                                                                                                                                                            |\n|-----------------------|:--------:|:--------:|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| **Segment Protocols** |     ✅    |     ✅    | `--select segment/tracking_plan_name` | Only supports `MAJOR-0` versions.                                                                                                                                              |\n| **Avo**               |     ❌    |     ✅    | `--select avo/branch_name`            | Schema changes managed in Avo [branches](https://www.avo.app/docs/workspace/branches) - `"version": "1-0"` (always).<br> Avo customers pull schemas with `reflekt pull` and build dbt artifacts with `reflekt build`. |\n\n#### Pull schemas from a registry\nPulling schemas from a registry is as easy as ...\n```bash\n❯ reflekt pull --select segment/ecommerce\n[19:28:32] INFO     Running with reflekt=0.3.1\n\n[19:28:32] INFO     Searching Segment for schemas\n\n[19:28:33] INFO     Found 9 schemas to pull:\n\n[19:28:33] INFO     1 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Identify/1-0.json\n[19:28:34] INFO     2 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Group/1-0.json\n[19:28:34] INFO     3 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/1-0.json\n[19:28:34] INFO     4 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Started/1-0.json\n[19:28:34] INFO     5 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Step Completed/1-0.json\n[19:28:34] INFO     6 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Step Viewed/1-0.json\n[19:28:34] INFO     7 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Order Completed/1-0.json\n[19:28:34] INFO     8 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Page Viewed/1-0.json\n[19:28:34] INFO     9 of 9 Writing to /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Product Added/1-0.json\n\n[19:28:34] INFO     Completed successfully\n```\nThe `reflekt pull` command builds the corresponding JSON files in the `schemas/` directory. For the example above, the resulting directory structure would be:\n```bash\nschemas\n├── .reflekt\n└── segment\n    └── ecommerce\n        ├── Cart Viewed\n        │   └── 1-0.json\n        ├── Checkout Started\n        │   └── 1-0.json\n        ├── Checkout Step Completed\n        │   └── 1-0.json\n        ├── Checkout Step Viewed\n        │   └── 1-0.json\n        ├── Group\n        │   └── 1-0.json\n        ├── Identify\n        │   └── 1-0.json\n        ├── Order Completed\n        │   └── 1-0.json\n        ├── Page Viewed\n        │   └── 1-0.json\n        └── Product Added\n            └── 1-0.json\n```\n\n#### Push schemas to a registry\nPublishing schemas to a registry follows the same pattern ...\n\n```bash\n❯ reflekt push --select segment/ecommerce\n[19:29:06] INFO     Running with reflekt=0.3.1\n\n[19:29:07] INFO     Searching for JSON schemas in: /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce\n\n[19:29:07] INFO     Found 9 schemas to push\n\n[19:29:07] INFO     1 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Identify/1-0.json\n[19:29:07] INFO     2 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/1-0.json\n[19:29:07] INFO     3 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Step Viewed/1-0.json\n[19:29:07] INFO     4 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Group/1-0.json\n[19:29:07] INFO     5 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Order Completed/1-0.json\n[19:29:07] INFO     6 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Step Completed/1-0.json\n[19:29:07] INFO     7 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Started/1-0.json\n[19:29:07] INFO     8 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Page Viewed/1-0.json\n[19:29:07] INFO     9 of 9 Pushing /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Product Added/1-0.json\n\n[19:29:08] INFO     Completed successfully\n```\n\n<br>\n\n### Linting schemas\nSchemas can be linted to test if they follow the naming and metadata conventions configured for a Reflekt project.\n\n```bash\n❯ reflekt lint --select segment/ecommerce\n[18:57:45] INFO     Running with reflekt=0.3.1\n\n[18:57:46] INFO     Searching for JSON schemas in: /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce\n\n[18:57:46] INFO     Found 9 schema(s) to lint\n\n[18:57:46] INFO     1 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Identify/1-0.json\n[18:57:47] INFO     2 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/1-0.json\n[18:57:48] ERROR    Property \'cartId\' in /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/1-0.json does not match naming convention \'casing: snake\' in\n                    /Users/myuser/Repos/my-reflekt-project/reflekt_project.yml.\n[18:57:48] INFO     3 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Step Viewed/1-0.json\n[18:57:50] INFO     4 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Group/1-0.json\n[18:57:50] INFO     5 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Order Completed/1-0.json\n[18:57:54] INFO     6 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Step Completed/1-0.json\n[18:57:55] INFO     7 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Checkout Started/1-0.json\n[18:57:58] INFO     8 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Page Viewed/1-0.json\n[18:58:01] INFO     9 of 9 Linting /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Product Added/1-0.json\n\n[18:58:04] ERROR    Linting failed with 1 error(s):\n\n[18:58:04] ERROR    Property \'cartId\' in /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/1-0.json does not match naming convention \'casing: snake\' in\n                    /Users/myuser/Repos/my-reflekt-project/reflekt_project.yml.\n```\n\nRunning `reflekt lint` in a CI/CD pipeline is a great way to ensure schema consistency and quality before pushing schemas to a schema registry.\n\n<br>\n\n## dbt artifacts\n[dbt](https://www.getdbt.com/) is a popular data tool to transformation and model data. When modeling data in dbt, it is [best practice](https://docs.getdbt.com/guides/best-practices/how-we-structure/1-guide-overview) to:\n- Define sources pointing to the raw data.\n- Define staging models, 1-to-1 for each source, that [rename, recast, or usefully reconsider](https://discourse.getdbt.com/t/how-we-used-to-structure-our-dbt-projects/355#data-transformation-101-1) columns into a consistent format. Materialized as views.\n- Document staging models with descriptions for the model and its fields, including relevant tests (e.g., unique and not_null IDs) as required.\n\nWhile we recommend following this practice, it can be ***a lot of work to maintain*** for product analytics, where:\n- There are many events (often 100+) and properties.\n- Events and properties are added or updated regularly as the product and data requirements evolve.\n- The Product and Engineer teams are bigger than the Data team, making it hard to keep up with the changes.\n\n**Reflekt can help by building dbt artifacts for you with a single CLI command.** Think of this as dbt\'s [codegen](https://github.com/dbt-labs/dbt-codegen) package on steroids :muscle: :pill:.\n\n### Building private dbt packages\nTo build a private dbt package with sources, staging models, and docs that perfectly *reflekts* the schemas in a Reflekt project and the raw data in the warehouse, you can run a command like the example below.\n\nWhere:\n- `--select segment/ecommerce` selects all the schemas in the `schemas/segment/ecommerce/` directory.\n- `--source snowflake.raw.ecomm_demo` specifies to connect to a data source with ID `snowflake`, database `raw`, and schema `ecomm_demo` as defined in `reflekt_profiles.yml`.\n- `--sdk segment` specifies the event data was collected via the Segment SDK. Reflekt knows how Segment loads data into data warehouses and writes SQL models accordingly.\n\nIf an event schema has multiple versions, Reflekt builds a staging model for both versions, allowing the Data team to easily consolidate schema changes as needed.\n\n```bash\n❯ reflekt build dbt --select segment/ecommerce --source snowflake.raw.ecomm_demo --sdk segment\n[09:45:23] INFO     Running with reflekt=0.3.1\n\n[09:45:24] INFO     Searching for JSON schemas in: /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce\n\n[09:45:24] INFO     Found 10 schemas to build\n\n[09:45:24] INFO     Building dbt package:\n                        name: reflekt_demo\n                        dir: /Users/myuser/Repos/my-reflekt-project/artifacts/dbt/reflekt_demo\n                        --select: segment/ecommerce\n                        --sdk_arg: segment\n                        --source: snowflake.raw.ecomm_demo\n\n[09:45:24] INFO     Building dbt source \'ecomm_demo\'\n[09:45:24] INFO     Building dbt artifacts for schema: /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Identify/1-0.json\n[09:45:26] INFO     Building dbt table \'identifies\' in source \'ecomm_demo\'\n[09:45:26] INFO     Building staging model \'stg_ecomm_demo__identifies.sql\'\n[09:45:26] INFO     Building dbt documentation \'_stg_ecomm_demo__identifies.yml\'\n\n[09:45:26] INFO     Building dbt artifacts for schema: Segment \'users\' table\n[09:45:26] INFO     Building dbt table \'users\' in source \'ecomm_demo\'\n[09:45:26] INFO     Building staging model \'stg_ecomm_demo__users.sql\'\n[09:45:26] INFO     Building dbt documentation \'_stg_ecomm_demo__users.yml\'\n\n[09:45:26] INFO     Building dbt artifacts for schema: /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/2-0.json\n[09:45:26] INFO     Building dbt table \'cart_viewed\' in source \'ecomm_demo\'\n[09:45:26] INFO     Building staging model \'stg_ecomm_demo__cart_viewed__v2_0.sql\'\n[09:45:26] INFO     Building dbt documentation \'_stg_ecomm_demo__cart_viewed__v2_0.yml\'\n\n[09:45:26] INFO     Building dbt artifacts for schema: /Users/myuser/Repos/my-reflekt-project/schemas/segment/ecommerce/Cart Viewed/1-0.json\n[09:45:27] INFO     Building staging model \'stg_ecomm_demo__cart_viewed.sql\'\n[09:45:27] INFO     Building dbt documentation \'_stg_ecomm_demo__cart_viewed.yml\'\n\n...\n...  # Full output omitted for brevity\n...\n\n[09:45:29] INFO     Building dbt artifacts for schema: Segment \'tracks\' table\n[09:45:29] INFO     Building dbt table \'tracks\' in source \'ecomm_demo\'\n[09:45:29] INFO     Building staging model \'stg_ecomm_demo__tracks.sql\'\n[09:45:29] INFO     Building dbt documentation \'_stg_ecomm_demo__tracks.yml\'\n\n\n[09:45:29] INFO     Copying dbt package from temporary path /Users/myuser/Repos/my-reflekt-project/.reflekt_cache/artifacts/dbt/reflekt_demo to\n                    /Users/myuser/Repos/my-reflekt-project/artifacts/dbt/reflekt_demo\n\n[09:45:29] INFO     Successfully built dbt package\n```\n\n### Using private dbt packages\nTo use a Reflekt dbt package in a downstream dbt project, add it to the dbt project\'s `packages.yml`.\n\n#### dbt-core\n```yaml\n# packages.yml\npackages:\n  - git: "https://github.com/<your_user_or_org>/<your_repo>"  # Reflekt project Github repo URL\n    subdirectory: "dbt-packages/<reflekt_dbt_package_name>"\n    revision: v0.1.0__reflekt_demo  # Branch, tag, or commit (40-character hash). For latest, use \'main\' branch.\n```\n\n#### dbt-cloud\n```yaml\n# packages.yml\npackages:\n  - git: ""https://{{env_var(\'DBT_ENV_SECRET_GITHUB_PAT\')}}@github.com/<your_user_or_org>/<your_repo>.git""  # Reflekt project Github repo URL with GitHub PAT\n    subdirectory: "dbt-packages/<reflekt_dbt_package_name>"\n    revision: v0.1.0__reflekt_demo  # Branch, tag, or commit (40-character hash). For latest, use \'main\' branch.\n```\nTo use with dbt-cloud, you will need to create a [Github personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) (e.g., `DBT_ENV_SECRET_GITHUB_PAT`) and [configure it as an environment variable](https://docs.getdbt.com/docs/dbt-cloud/using-dbt-cloud/cloud-environment-variables) in your dbt-cloud account.\n\nFor local dbt development, set the environment variable on your local machine.\n```bash\n# Add the following line to your .zshrc, .bash_profile, etc.\nexport DBT_ENV_SECRET_GITHUB_PAT=YOUR_TOKEN\n```\n\n### Supported data warehouses\nReflekt currently supports the following data warehouses:\n- Snowflake\n- Redshift\n- :construction: BigQuery support coming soon! :construction:\n',
     'author': 'Gregory Clunies',
     'author_email': 'greg.clunies@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/GClunies/Reflekt',
```

### Comparing `reflekt-0.3.8/PKG-INFO` & `reflekt-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflekt
-Version: 0.3.8
+Version: 0.3.9
 Summary: A CLI tool to define event schemas, lint them, interact with schema registries, and build corresponding data artifacts (e.g., dbt package).
 Home-page: https://github.com/GClunies/Reflekt
 License: Apache-2.0
 Keywords: events,jsonchema,analytics,business-intelligence,data-modeling,dbt,snowflake,redshift,segment,avo
 Author: Gregory Clunies
 Author-email: greg.clunies@gmail.com
 Requires-Python: >=3.8,<4.0
```

