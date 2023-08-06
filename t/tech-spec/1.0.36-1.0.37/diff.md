# Comparing `tmp/tech-spec-1.0.36.tar.gz` & `tmp/tech-spec-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.36.tar", last modified: Sun Aug  6 07:41:09 2023, max compression
+gzip compressed data, was "tech-spec-1.0.37.tar", last modified: Sun Aug  6 07:46:34 2023, max compression
```

## Comparing `tech-spec-1.0.36.tar` & `tech-spec-1.0.37.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.023858 tech-spec-1.0.36/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 07:41:00.000000 tech-spec-1.0.36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:41:09.023858 tech-spec-1.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 07:41:00.000000 tech-spec-1.0.36/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-06 07:41:00.000000 tech-spec-1.0.36/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:41:09.023858 tech-spec-1.0.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-06 07:41:00.000000 tech-spec-1.0.36/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.019858 tech-spec-1.0.36/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:41:09.000000 tech-spec-1.0.36/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-06 07:41:09.000000 tech-spec-1.0.36/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:41:09.000000 tech-spec-1.0.36/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 07:41:09.000000 tech-spec-1.0.36/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 07:41:09.000000 tech-spec-1.0.36/tech_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 07:41:09.000000 tech-spec-1.0.36/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.019858 tech-spec-1.0.36/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.019858 tech-spec-1.0.36/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.019858 tech-spec-1.0.36/techspec/cli/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/actions/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/actions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.023858 tech-spec-1.0.36/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/groups/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.023858 tech-spec-1.0.36/techspec/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/generator/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/generator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/generator/service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:41:09.023858 tech-spec-1.0.36/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-06 07:41:00.000000 tech-spec-1.0.36/techspec/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.257436 tech-spec-1.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 07:46:25.000000 tech-spec-1.0.37/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:46:34.257436 tech-spec-1.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 07:46:25.000000 tech-spec-1.0.37/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-06 07:46:25.000000 tech-spec-1.0.37/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:46:34.257436 tech-spec-1.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-06 07:46:25.000000 tech-spec-1.0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.253436 tech-spec-1.0.37/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:46:34.000000 tech-spec-1.0.37/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-06 07:46:34.000000 tech-spec-1.0.37/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:46:34.000000 tech-spec-1.0.37/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 07:46:34.000000 tech-spec-1.0.37/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 07:46:34.000000 tech-spec-1.0.37/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 07:46:34.000000 tech-spec-1.0.37/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.253436 tech-spec-1.0.37/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.253436 tech-spec-1.0.37/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.253436 tech-spec-1.0.37/techspec/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/actions/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/actions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.253436 tech-spec-1.0.37/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/groups/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.257436 tech-spec-1.0.37/techspec/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/generator/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/generator/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:46:34.257436 tech-spec-1.0.37/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-06 07:46:25.000000 tech-spec-1.0.37/techspec/schema.json
```

### Comparing `tech-spec-1.0.36/setup.py` & `tech-spec-1.0.37/setup.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/tech_spec.egg-info/SOURCES.txt` & `tech-spec-1.0.37/tech_spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/techspec/cli/actions/code.py` & `tech-spec-1.0.37/techspec/cli/actions/code.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ) -> None:
     spec = schema_validation_action(spec_dir)
     try:
         code_spec = generator.get_techspec(code_dir)
     except GeneratorService.exc.OutputDirectoryDoesNotExists:
         stderr.print("Provided code directory does not exists")
         raise typer.Exit(1)
-
+    spec.themes = []
     if spec != code_spec:
         stderr.print("Code is not sync with schema")
         raise typer.Exit(1)
 
     print("Code is in sync with schema")
```

### Comparing `tech-spec-1.0.36/techspec/cli/actions/schema.py` & `tech-spec-1.0.37/techspec/cli/actions/schema.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/techspec/cli/container.py` & `tech-spec-1.0.37/techspec/cli/container.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/techspec/generator/service.py` & `tech-spec-1.0.37/techspec/generator/service.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/techspec/schema/dtos.py` & `tech-spec-1.0.37/techspec/schema/dtos.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/techspec/schema/service.py` & `tech-spec-1.0.37/techspec/schema/service.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.36/techspec/schema.json` & `tech-spec-1.0.37/techspec/schema.json`

 * *Files identical despite different names*

