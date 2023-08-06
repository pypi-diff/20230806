# Comparing `tmp/tech-spec-1.0.31.tar.gz` & `tmp/tech-spec-1.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.31.tar", last modified: Sat Aug  5 12:13:06 2023, max compression
+gzip compressed data, was "tech-spec-1.0.33.tar", last modified: Sat Aug  5 12:24:34 2023, max compression
```

## Comparing `tech-spec-1.0.31.tar` & `tech-spec-1.0.33.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.768698 tech-spec-1.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 12:12:52.000000 tech-spec-1.0.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:13:06.768698 tech-spec-1.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:12:52.000000 tech-spec-1.0.31/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:12:52.000000 tech-spec-1.0.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:13:06.768698 tech-spec-1.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:12:52.000000 tech-spec-1.0.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.764698 tech-spec-1.0.31/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.764698 tech-spec-1.0.31/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.764698 tech-spec-1.0.31/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.768698 tech-spec-1.0.31/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/groups/stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.768698 tech-spec-1.0.31/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.729373 tech-spec-1.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 12:24:20.000000 tech-spec-1.0.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:24:34.729373 tech-spec-1.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:24:20.000000 tech-spec-1.0.33/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:24:20.000000 tech-spec-1.0.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:24:34.729373 tech-spec-1.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:24:20.000000 tech-spec-1.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:24:34.000000 tech-spec-1.0.33/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.725373 tech-spec-1.0.33/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/groups/stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:34.729373 tech-spec-1.0.33/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-05 12:24:20.000000 tech-spec-1.0.33/techspec/schema.json
```

### Comparing `tech-spec-1.0.31/setup.py` & `tech-spec-1.0.33/setup.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.31/tech_spec.egg-info/SOURCES.txt` & `tech-spec-1.0.33/tech_spec.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tech_spec.egg-info/PKG-INFO
 tech_spec.egg-info/SOURCES.txt
 tech_spec.egg-info/dependency_links.txt
 tech_spec.egg-info/entry_points.txt
 tech_spec.egg-info/requires.txt
 tech_spec.egg-info/top_level.txt
 techspec/__init__.py
+techspec/__main__.py
 techspec/py.typed
 techspec/schema.json
 techspec/cli/__init__.py
 techspec/cli/main.py
 techspec/cli/groups/__init__.py
 techspec/cli/groups/schema.py
 techspec/cli/groups/stderr.py
```

### Comparing `tech-spec-1.0.31/techspec/cli/groups/schema.py` & `tech-spec-1.0.33/techspec/cli/groups/schema.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.31/techspec/schema.json` & `tech-spec-1.0.33/techspec/schema.json`

 * *Files identical despite different names*

