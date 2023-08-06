# Comparing `tmp/tech-spec-1.0.33.tar.gz` & `tmp/tech-spec-1.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.33.tar", last modified: Sat Aug  5 12:24:34 2023, max compression
+gzip compressed data, was "tech-spec-1.0.34.tar", last modified: Sun Aug  6 07:14:28 2023, max compression
```

## Comparing `tech-spec-1.0.33.tar` & `tech-spec-1.0.34.tar`

### file list

```diff
@@ -1,30 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.729373 tech-spec-1.0.33/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 12:24:20.000000 tech-spec-1.0.33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:24:34.729373 tech-spec-1.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:24:20.000000 tech-spec-1.0.33/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:24:20.000000 tech-spec-1.0.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:24:34.729373 tech-spec-1.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:24:20.000000 tech-spec-1.0.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/groups/stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.729373 tech-spec-1.0.33/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.458132 tech-spec-1.0.34/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 07:14:14.000000 tech-spec-1.0.34/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:14:28.458132 tech-spec-1.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 07:14:14.000000 tech-spec-1.0.34/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-06 07:14:14.000000 tech-spec-1.0.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:14:28.458132 tech-spec-1.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-06 07:14:14.000000 tech-spec-1.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/actions/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/actions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/groups/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.458132 tech-spec-1.0.34/techspec/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.458132 tech-spec-1.0.34/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema.json
```

### Comparing `tech-spec-1.0.33/setup.py` & `tech-spec-1.0.34/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 setup(
     name="tech-spec",
     version=os.environ["GITHUB_REF_NAME"],
     description="Tech spec for code generation",
     author="Vladimir Vojtenko",
     author_email="vladimirdev635@gmail.com",
     license="MIT",
-    install_requires=["typer[all]", "pyyaml", "jsonschema"],
+    install_requires=[
+        "typer[all]",
+        "pyyaml",
+        "jsonschema",
+        "dependency-injector",
+    ],
     packages=find_packages(exclude=["__tests__*"]),
     include_package_data=True,
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     entry_points={"console_scripts": ["techspecpy=techspec.cli:cli_main"]},
 )
```

### Comparing `tech-spec-1.0.33/techspec/schema.json` & `tech-spec-1.0.34/techspec/schema.json`

 * *Files identical despite different names*

