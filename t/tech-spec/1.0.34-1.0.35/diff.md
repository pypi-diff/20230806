# Comparing `tmp/tech-spec-1.0.34.tar.gz` & `tmp/tech-spec-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.34.tar", last modified: Sun Aug  6 07:14:28 2023, max compression
+gzip compressed data, was "tech-spec-1.0.35.tar", last modified: Sun Aug  6 07:18:13 2023, max compression
```

## Comparing `tech-spec-1.0.34.tar` & `tech-spec-1.0.35.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.458132 tech-spec-1.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 07:14:14.000000 tech-spec-1.0.34/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:14:28.458132 tech-spec-1.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 07:14:14.000000 tech-spec-1.0.34/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-06 07:14:14.000000 tech-spec-1.0.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:14:28.458132 tech-spec-1.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-06 07:14:14.000000 tech-spec-1.0.34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 07:14:28.000000 tech-spec-1.0.34/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/cli/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/actions/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/actions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.454132 tech-spec-1.0.34/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/groups/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.458132 tech-spec-1.0.34/techspec/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/generator/service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:28.458132 tech-spec-1.0.34/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-06 07:14:14.000000 tech-spec-1.0.34/techspec/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 07:18:02.000000 tech-spec-1.0.35/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:18:13.804415 tech-spec-1.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 07:18:02.000000 tech-spec-1.0.35/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-06 07:18:02.000000 tech-spec-1.0.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:18:13.804415 tech-spec-1.0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-06 07:18:02.000000 tech-spec-1.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.800415 tech-spec-1.0.35/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-06 07:18:13.000000 tech-spec-1.0.35/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-06 07:18:13.000000 tech-spec-1.0.35/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:18:13.000000 tech-spec-1.0.35/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 07:18:13.000000 tech-spec-1.0.35/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 07:18:13.000000 tech-spec-1.0.35/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 07:18:13.000000 tech-spec-1.0.35/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/techspec/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/actions/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/actions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/groups/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/techspec/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/generator/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/generator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/generator/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:18:13.804415 tech-spec-1.0.35/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-06 07:18:02.000000 tech-spec-1.0.35/techspec/schema.json
```

### Comparing `tech-spec-1.0.34/setup.py` & `tech-spec-1.0.35/setup.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/tech_spec.egg-info/SOURCES.txt` & `tech-spec-1.0.35/tech_spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/techspec/cli/actions/code.py` & `tech-spec-1.0.35/techspec/cli/actions/code.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 ) -> None:
     spec = schema_validation_action(spec_dir)
     code = generator.generate(spec)
     if not output_dir.exists():
         output_dir.mkdir(parents=True)
     with open(output_dir / "forms.py", "w+") as file:
         file.write(code.forms)
+    with open(output_dir / "__init__.py", "w+") as file:
+        pass
     print("Code generated successfully")
 
 
 @inject
 def validate_action(
     spec_dir: Path,
     output_dir: Path,
```

### Comparing `tech-spec-1.0.34/techspec/cli/actions/schema.py` & `tech-spec-1.0.35/techspec/cli/actions/schema.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/techspec/cli/container.py` & `tech-spec-1.0.35/techspec/cli/container.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/techspec/generator/service.py` & `tech-spec-1.0.35/techspec/generator/service.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/techspec/schema/dtos.py` & `tech-spec-1.0.35/techspec/schema/dtos.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/techspec/schema/service.py` & `tech-spec-1.0.35/techspec/schema/service.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.34/techspec/schema.json` & `tech-spec-1.0.35/techspec/schema.json`

 * *Files identical despite different names*

