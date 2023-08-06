# Comparing `tmp/sbot-1.1.0.tar.gz` & `tmp/sbot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbot-1.1.0.tar", last modified: Sun Aug  6 11:42:22 2023, max compression
+gzip compressed data, was "sbot-1.1.1.tar", last modified: Sun Aug  6 16:08:09 2023, max compression
```

## Comparing `sbot-1.1.0.tar` & `sbot-1.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-06 11:42:03.000000 sbot-1.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 11:42:03.000000 sbot-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-06 11:42:03.000000 sbot-1.1.0/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-06 11:42:03.000000 sbot-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-06 11:42:03.000000 sbot-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-06 11:42:03.000000 sbot-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-06 11:42:22.379370 sbot-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-06 11:42:03.000000 sbot-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-06 11:42:03.000000 sbot-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/sbot/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/arduino.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/game_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/motor_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/power_board.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/serial_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/servo_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/sbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:42:22.379370 sbot-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_arduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.371369 sbot-1.1.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/bad/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/bad/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/empty/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/missing_key/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/missing_key/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.371369 sbot-1.1.0/tests/test_data/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/nested/valid/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/nested/valid/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/not_object/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/not_object/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/valid/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/valid/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_motor_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_power_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_sbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_serial_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_servo_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.890739 sbot-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-06 16:07:47.000000 sbot-1.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.878739 sbot-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 16:07:47.000000 sbot-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.878739 sbot-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-06 16:07:47.000000 sbot-1.1.1/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-06 16:07:47.000000 sbot-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-06 16:07:47.000000 sbot-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-06 16:07:47.000000 sbot-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-06 16:08:09.890739 sbot-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-06 16:07:47.000000 sbot-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-06 16:07:47.000000 sbot-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.882739 sbot-1.1.1/sbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 16:08:09.000000 sbot-1.1.1/sbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/arduino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/game_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-08-06 16:07:47.000000 sbot-1.1.1/sbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.882739 sbot-1.1.1/sbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-06 16:08:09.000000 sbot-1.1.1/sbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-06 16:08:09.000000 sbot-1.1.1/sbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:08:09.000000 sbot-1.1.1/sbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-06 16:08:09.000000 sbot-1.1.1/sbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 16:08:09.000000 sbot-1.1.1/sbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 16:08:09.890739 sbot-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_arduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.878739 sbot-1.1.1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/test_data/bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_data/bad/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/test_data/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_data/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/test_data/missing_key/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_data/missing_key/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.878739 sbot-1.1.1/tests/test_data/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/test_data/nested/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_data/nested/valid/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/test_data/not_object/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_data/not_object/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:08:09.886739 sbot-1.1.1/tests/test_data/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_data/valid/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_sbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-06 16:07:47.000000 sbot-1.1.1/tests/test_timeout.py
```

### Comparing `sbot-1.1.0/.github/dependabot.yml` & `sbot-1.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/.github/workflows/test_build.yml` & `sbot-1.1.1/.github/workflows/test_build.yml`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/.gitignore` & `sbot-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/LICENSE` & `sbot-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/PKG-INFO` & `sbot-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbot
-Version: 1.1.0
+Version: 1.1.1
 Summary: The robot API for the Smallpeice summer school
 Author-email: SourceBots <hello@sourcebots.co.uk>
 License: MIT License
         
         Copyright (c) 2019-21 Dan Trickey
         Copyright (c) 2023 SourceBots
```

### Comparing `sbot-1.1.0/README.md` & `sbot-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/pyproject.toml` & `sbot-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/__init__.py` & `sbot-1.1.1/sbot/__init__.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/arduino.py` & `sbot-1.1.1/sbot/arduino.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/camera.py` & `sbot-1.1.1/sbot/camera.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/exceptions.py` & `sbot-1.1.1/sbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/logging.py` & `sbot-1.1.1/sbot/logging.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/marker.py` & `sbot-1.1.1/sbot/marker.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,10 +94,10 @@
         - Z axis is up
         """
         return Coordinates(tvec[2], -tvec[0], -tvec[1])
 
     def __repr__(self) -> str:
         return (
             f"<{self.__class__.__name__} id={self.id} distance={self.distance:.0f}mm "
-            f"bearing={self.azimuth:.0f}rad elevation={self.elevation:.0f}rad "
+            f"bearing={self.azimuth:.2f}rad elevation={self.elevation:.2f}rad "
             f"size={self.size}mm>"
         )
```

### Comparing `sbot-1.1.0/sbot/metadata.py` & `sbot-1.1.1/sbot/metadata.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/motor_board.py` & `sbot-1.1.1/sbot/motor_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/mqtt.py` & `sbot-1.1.1/sbot/mqtt.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/power_board.py` & `sbot-1.1.1/sbot/power_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/robot.py` & `sbot-1.1.1/sbot/robot.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/serial_wrapper.py` & `sbot-1.1.1/sbot/serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/servo_board.py` & `sbot-1.1.1/sbot/servo_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/timeout.py` & `sbot-1.1.1/sbot/timeout.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot/utils.py` & `sbot-1.1.1/sbot/utils.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/sbot.egg-info/PKG-INFO` & `sbot-1.1.1/sbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbot
-Version: 1.1.0
+Version: 1.1.1
 Summary: The robot API for the Smallpeice summer school
 Author-email: SourceBots <hello@sourcebots.co.uk>
 License: MIT License
         
         Copyright (c) 2019-21 Dan Trickey
         Copyright (c) 2023 SourceBots
```

### Comparing `sbot-1.1.0/sbot.egg-info/SOURCES.txt` & `sbot-1.1.1/sbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/conftest.py` & `sbot-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_arduino.py` & `sbot-1.1.1/tests/test_arduino.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_metadata.py` & `sbot-1.1.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_motor_board.py` & `sbot-1.1.1/tests/test_motor_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_power_board.py` & `sbot-1.1.1/tests/test_power_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_sbot.py` & `sbot-1.1.1/tests/test_sbot.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_serial_wrapper.py` & `sbot-1.1.1/tests/test_serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_servo_board.py` & `sbot-1.1.1/tests/test_servo_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.1.0/tests/test_timeout.py` & `sbot-1.1.1/tests/test_timeout.py`

 * *Files identical despite different names*

