# Comparing `tmp/colorful-logger-0.2.0b2.tar.gz` & `tmp/colorful-logger-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful-logger-0.2.0b2.tar", last modified: Sun Jul 16 01:06:29 2023, max compression
+gzip compressed data, was "colorful-logger-0.2.0b3.tar", last modified: Sat Aug  5 15:43:21 2023, max compression
```

## Comparing `colorful-logger-0.2.0b2.tar` & `colorful-logger-0.2.0b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.175374 colorful-logger-0.2.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/README.zh_CN.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/colorful_logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/colorful_logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/colorful_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 01:06:29.000000 colorful-logger-0.2.0b2/colorful_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-16 01:06:17.000000 colorful-logger-0.2.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 01:06:29.179374 colorful-logger-0.2.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/README.zh_CN.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/colorful_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/colorful_logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-05 15:43:20.000000 colorful-logger-0.2.0b3/colorful_logger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/colorful_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-08-05 15:43:21.000000 colorful-logger-0.2.0b3/colorful_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-05 15:43:21.000000 colorful-logger-0.2.0b3/colorful_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 15:43:21.000000 colorful-logger-0.2.0b3/colorful_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-05 15:43:21.000000 colorful-logger-0.2.0b3/colorful_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-05 15:43:21.000000 colorful-logger-0.2.0b3/colorful_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-05 15:43:08.000000 colorful-logger-0.2.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 15:43:21.064147 colorful-logger-0.2.0b3/setup.cfg
```

### Comparing `colorful-logger-0.2.0b2/.github/workflows/publish.yaml` & `colorful-logger-0.2.0b3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/.gitignore` & `colorful-logger-0.2.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/LICENSE` & `colorful-logger-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/PKG-INFO` & `colorful-logger-0.2.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-logger
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: A colorful logger for python3.
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `colorful-logger-0.2.0b2/README.md` & `colorful-logger-0.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/README.zh_CN.md` & `colorful-logger-0.2.0b3/README.zh_CN.md`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/colorful_logger/__init__.py` & `colorful-logger-0.2.0b3/colorful_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/colorful_logger/consts.py` & `colorful-logger-0.2.0b3/colorful_logger/consts.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/colorful_logger/formatter.py` & `colorful-logger-0.2.0b3/colorful_logger/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                 "message": msg,
                 **kwargs,
                 "caller": f"{self.__file_path(record)}{self.__line_number(record)}",
             }
 
             return json.dumps(log_map)
 
-        for k, v in record.kwargs.items():
+        for k, v in kwargs.items():
             if k in ("err", "error"):
                 msg += f" {ds.format_with_one_style(k+'=', ds.fc.red)}{v}"
             else:
                 msg += f" {ds.format_with_one_style(k+'=', ds.fc.cyan)}{v}"
 
         fields = (
             self.__time(record),
```

### Comparing `colorful-logger-0.2.0b2/colorful_logger/handlers.py` & `colorful-logger-0.2.0b3/colorful_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/colorful_logger/logger.py` & `colorful-logger-0.2.0b3/colorful_logger/logger.py`

 * *Files identical despite different names*

### Comparing `colorful-logger-0.2.0b2/colorful_logger.egg-info/PKG-INFO` & `colorful-logger-0.2.0b3/colorful_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-logger
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: A colorful logger for python3.
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `colorful-logger-0.2.0b2/pyproject.toml` & `colorful-logger-0.2.0b3/pyproject.toml`

 * *Files identical despite different names*

