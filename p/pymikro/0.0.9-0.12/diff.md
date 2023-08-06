# Comparing `tmp/pymikro-0.0.9.tar.gz` & `tmp/pymikro-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pymikro-0.12.tar", last modified: Sun Aug  6 20:09:14 2023, max compression
```

## Comparing `pymikro-0.0.9.tar` & `pymikro-0.12.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pymikro-0.0.9/50-ni-maschine.rules
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 pymikro-0.0.9/demo/demo_lights.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pymikro-0.0.9/demo/demo_main.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pymikro-0.0.9/demo/demo_output_state.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pymikro-0.0.9/demo/demo_pads_buttons.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pymikro-0.0.9/demo/demo_screen.py
--rw-r--r--   0        0        0   756072 2020-02-02 00:00:00.000000 pymikro-0.0.9/src/pymikro/DejaVuSans.ttf
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 pymikro-0.0.9/src/pymikro/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pymikro-0.0.9/src/pymikro/maschine_mikro_mk3.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pymikro-0.0.9/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 pymikro-0.0.9/LICENSE
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 pymikro-0.0.9/README.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pymikro-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 pymikro-0.0.9/PKG-INFO
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/
+-rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-07-17 08:23:51.000000 pymikro-0.12/LICENSE
+-rw-r--r--   0 ze        (1000) ze        (1000)      286 2023-08-06 20:09:14.041136 pymikro-0.12/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)     6787 2023-07-18 17:01:01.000000 pymikro-0.12/README.md
+-rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-06 20:09:14.041136 pymikro-0.12/setup.cfg
+-rw-r--r--   0 ze        (1000) ze        (1000)      502 2023-08-06 20:08:59.000000 pymikro-0.12/setup.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/src/
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/src/pymikro/
+-rw-r--r--   0 ze        (1000) ze        (1000)     5299 2023-07-29 13:25:33.000000 pymikro-0.12/src/pymikro/__init__.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/src/pymikro.egg-info/
+-rw-r--r--   0 ze        (1000) ze        (1000)      286 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)      224 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/SOURCES.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/dependency_links.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)       11 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/requires.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        8 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/top_level.txt
```

### Comparing `pymikro-0.0.9/src/pymikro/__init__.py` & `pymikro-0.12/src/pymikro/__init__.py`

 * *Files identical despite different names*

### Comparing `pymikro-0.0.9/LICENSE` & `pymikro-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pymikro-0.0.9/README.md` & `pymikro-0.12/README.md`

 * *Files identical despite different names*

