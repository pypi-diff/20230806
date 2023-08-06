# Comparing `tmp/sbot-1.0.0rc2.tar.gz` & `tmp/sbot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbot-1.0.0rc2.tar", last modified: Sat Jul 29 14:21:38 2023, max compression
+gzip compressed data, was "sbot-1.1.0.tar", last modified: Sun Aug  6 11:42:22 2023, max compression
```

## Comparing `sbot-1.0.0rc2.tar` & `sbot-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.508319 sbot-1.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.492318 sbot-1.0.0rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.496318 sbot-1.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-29 14:21:38.508319 sbot-1.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.500318 sbot-1.0.0rc2/sbot/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/arduino.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/game_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/motor_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/power_board.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/serial_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/servo_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/sbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.500318 sbot-1.0.0rc2/sbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 14:21:38.000000 sbot-1.0.0rc2/sbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:21:38.508319 sbot-1.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_arduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.492318 sbot-1.0.0rc2/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/bad/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/bad/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/empty/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/missing_key/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/missing_key/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.492318 sbot-1.0.0rc2/tests/test_data/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/nested/valid/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/nested/valid/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/not_object/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/not_object/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:21:38.504318 sbot-1.0.0rc2/tests/test_data/valid/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_data/valid/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_motor_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_power_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_sbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_serial_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_servo_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-29 14:21:16.000000 sbot-1.0.0rc2/tests/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-06 11:42:03.000000 sbot-1.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 11:42:03.000000 sbot-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-06 11:42:03.000000 sbot-1.1.0/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-06 11:42:03.000000 sbot-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-06 11:42:03.000000 sbot-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-06 11:42:03.000000 sbot-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-06 11:42:22.379370 sbot-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-06 11:42:03.000000 sbot-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-06 11:42:03.000000 sbot-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/sbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/arduino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/game_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-08-06 11:42:03.000000 sbot-1.1.0/sbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.375369 sbot-1.1.0/sbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 11:42:22.000000 sbot-1.1.0/sbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:42:22.379370 sbot-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_arduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.371369 sbot-1.1.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/bad/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/missing_key/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/missing_key/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.371369 sbot-1.1.0/tests/test_data/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/nested/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/nested/valid/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/not_object/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/not_object/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:42:22.379370 sbot-1.1.0/tests/test_data/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_data/valid/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_motor_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_power_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_sbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_serial_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_servo_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-06 11:42:03.000000 sbot-1.1.0/tests/test_timeout.py
```

### Comparing `sbot-1.0.0rc2/.github/dependabot.yml` & `sbot-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/.github/workflows/test_build.yml` & `sbot-1.1.0/.github/workflows/test_build.yml`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/.gitignore` & `sbot-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/LICENSE` & `sbot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/PKG-INFO` & `sbot-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbot
-Version: 1.0.0rc2
+Version: 1.1.0
 Summary: The robot API for the Smallpeice summer school
 Author-email: SourceBots <hello@sourcebots.co.uk>
 License: MIT License
         
         Copyright (c) 2019-21 Dan Trickey
         Copyright (c) 2023 SourceBots
         
@@ -27,21 +27,22 @@
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/sourcebots/sbot
 Project-URL: Homepage, https://sourcebots.co.uk
 Project-URL: Documentation, https://docs.sourcebots.co.uk
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Typing :: Typed
 Classifier: Topic :: Education
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: vision
+Provides-Extra: mqtt
 License-File: LICENSE
 
 # sbot
 
 [![Lint & build](https://github.com/sourcebots/sbot/actions/workflows/test_build.yml/badge.svg)](https://github.com/sourcebots/sbot/actions/workflows/test_build.yml)
 [![PyPI version](https://badge.fury.io/py/sbot.svg)](https://badge.fury.io/py/sbot)
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](http://pip.pypa.io/en/stable/?badge=stable)
```

### Comparing `sbot-1.0.0rc2/README.md` & `sbot-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/pyproject.toml` & `sbot-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     "pyserial >=3,<4",
     "april_vision >=2.0.2,<3",
     "typing-extensions; python_version<'3.10'",
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Typing :: Typed",
     "Topic :: Education",
 ]
 
 [project.urls]
 Repository = "https://github.com/sourcebots/sbot"
 Homepage = "https://sourcebots.co.uk"
@@ -74,9 +74,11 @@
     "flake8",
     "isort",
     "mypy",
     "build",
     "types-pyserial",
     "pytest",
     "pytest-cov",
+    "types-paho-mqtt",
 ]
 vision = ["opencv-python-headless >=4,<5"]
+mqtt = ["paho-mqtt >=1.6,<2"]
```

### Comparing `sbot-1.0.0rc2/sbot/arduino.py` & `sbot-1.1.0/sbot/arduino.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/camera.py` & `sbot-1.1.0/sbot/camera.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/exceptions.py` & `sbot-1.1.0/sbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/logging.py` & `sbot-1.1.0/sbot/logging.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/marker.py` & `sbot-1.1.0/sbot/marker.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/metadata.py` & `sbot-1.1.0/sbot/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,20 +64,21 @@
     """
     search_path = os.environ.get(METADATA_ENV_VAR)
     if search_path:
         search_root = Path(search_path)
         if not search_root.is_dir():
             raise FileNotFoundError(f"Metaddata path {search_path} does not exist")
         for item in Path(search_path).iterdir():
-            if item.is_dir():
-                if (item / METADATA_NAME).exists():
+            try:
+                if item.is_dir() and (item / METADATA_NAME).exists():
                     return _load_metadata(item / METADATA_NAME)
-            else:
-                if item.name == METADATA_NAME:
+                elif item.name == METADATA_NAME:
                     return _load_metadata(item)
+            except PermissionError:
+                logger.debug(f"Unable to read {item}")
         else:
             logger.info(f"No JSON metadata files found in {search_path}")
     else:
         logger.info(f"{METADATA_ENV_VAR} not set, not loading metadata")
     return DEFAULT_METADATA
```

### Comparing `sbot-1.0.0rc2/sbot/motor_board.py` & `sbot-1.1.0/sbot/motor_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/power_board.py` & `sbot-1.1.0/sbot/power_board.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,23 +464,23 @@
     """
     __slots__ = ('_serial',)
 
     def __init__(self, serial: SerialWrapper):
         self._serial = serial
 
     @log_to_debug
-    def buzz(self, duration: float, frequency: float) -> None:
+    def buzz(self, frequency: float, duration: float) -> None:
         """
         Produce a tone on the piezo.
 
         This method is non-blocking, and sending another tone while one is
         playing will cancel the first.
 
-        :param duration: The duration of the tone, in seconds.
         :param frequency: The frequency of the tone, in Hz.
+        :param duration: The duration of the tone, in seconds.
         """
         frequency_int = int(float_bounds_check(
             frequency, 8, 10_000, "Frequency is a float in Hz between 0 and 10000"))
         duration_ms = int(float_bounds_check(
             duration * 1000, 0, 2**31 - 1,
             f"Duration is a float in seconds between 0 and {(2**31-1)/1000:,.0f}"))
```

### Comparing `sbot-1.0.0rc2/sbot/robot.py` & `sbot-1.1.0/sbot/robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 from .logging import log_to_debug, setup_logging
 from .metadata import Metadata
 from .motor_board import MotorBoard
 from .power_board import Note, PowerBoard
 from .servo_board import ServoBoard
 from .utils import obtain_lock, singular
 
+try:
+    from .mqtt import MQTT_VALID, MQTTClient, get_mqtt_variables
+except ImportError:
+    MQTT_VALID = False
+
 logger = logging.getLogger(__name__)
 
 
 class Robot:
     """
     The main robot class that provides access to all the boards.
 
@@ -34,15 +39,15 @@
         defaults to True
     :param trace_logging: Enable trace level logging to the console, defaults to False
     :param manual_boards: A dictionary of board types to a list of serial port paths
         to allow for connecting to boards that are not automatically detected, defaults to None
     """
     __slots__ = (
         '_lock', '_metadata', '_power_board', '_motor_boards', '_servo_boards',
-        '_arduinos', '_cameras',
+        '_arduinos', '_cameras', '_mqttc',
     )
 
     def __init__(
         self,
         *,
         debug: bool = False,
         wait_for_start: bool = True,
@@ -106,15 +111,24 @@
     def _init_camera(self) -> None:
         """
         Locate cameras that we have calibration data for.
 
         These cameras are used for AprilTag detection and provide location data of
         markers in its field of view.
         """
-        self._cameras = MappingProxyType(_setup_cameras(game_specific.MARKER_SIZES))
+        if MQTT_VALID:
+            # get the config from env vars
+            mqtt_config = get_mqtt_variables()
+            self._mqttc = MQTTClient.establish(**mqtt_config)
+            self._cameras = MappingProxyType(_setup_cameras(
+                game_specific.MARKER_SIZES,
+                self._mqttc.wrapped_publish,
+            ))
+        else:
+            self._cameras = MappingProxyType(_setup_cameras(game_specific.MARKER_SIZES))
 
     def _log_connected_boards(self) -> None:
         """
         Log the board types and serial numbers of all the boards connected to the robot.
 
         Firmware versions are also logged at debug level.
         """
@@ -284,15 +298,15 @@
         Once the start button is pressed, the metadata will be loaded and the timeout
         will start if in competition mode.
         """
         # ignore previous button presses
         _ = self.power_board._start_button()
         logger.info('Waiting for start button.')
 
-        self.power_board.piezo.buzz(0.1, Note.A6)
+        self.power_board.piezo.buzz(Note.A6, 0.1)
         self.power_board._run_led.flash()
 
         while not self.power_board._start_button():
             sleep(0.1)
         logger.info("Start button pressed.")
         self.power_board._run_led.on()
```

### Comparing `sbot-1.0.0rc2/sbot/serial_wrapper.py` & `sbot-1.1.0/sbot/serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/servo_board.py` & `sbot-1.1.0/sbot/servo_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/timeout.py` & `sbot-1.1.0/sbot/timeout.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot/utils.py` & `sbot-1.1.0/sbot/utils.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/sbot.egg-info/PKG-INFO` & `sbot-1.1.0/sbot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbot
-Version: 1.0.0rc2
+Version: 1.1.0
 Summary: The robot API for the Smallpeice summer school
 Author-email: SourceBots <hello@sourcebots.co.uk>
 License: MIT License
         
         Copyright (c) 2019-21 Dan Trickey
         Copyright (c) 2023 SourceBots
         
@@ -27,21 +27,22 @@
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/sourcebots/sbot
 Project-URL: Homepage, https://sourcebots.co.uk
 Project-URL: Documentation, https://docs.sourcebots.co.uk
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Typing :: Typed
 Classifier: Topic :: Education
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: vision
+Provides-Extra: mqtt
 License-File: LICENSE
 
 # sbot
 
 [![Lint & build](https://github.com/sourcebots/sbot/actions/workflows/test_build.yml/badge.svg)](https://github.com/sourcebots/sbot/actions/workflows/test_build.yml)
 [![PyPI version](https://badge.fury.io/py/sbot.svg)](https://badge.fury.io/py/sbot)
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](http://pip.pypa.io/en/stable/?badge=stable)
```

### Comparing `sbot-1.0.0rc2/sbot.egg-info/SOURCES.txt` & `sbot-1.1.0/sbot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 sbot/camera.py
 sbot/exceptions.py
 sbot/game_specific.py
 sbot/logging.py
 sbot/marker.py
 sbot/metadata.py
 sbot/motor_board.py
+sbot/mqtt.py
 sbot/power_board.py
 sbot/py.typed
 sbot/robot.py
 sbot/serial_wrapper.py
 sbot/servo_board.py
 sbot/timeout.py
 sbot/utils.py
```

### Comparing `sbot-1.0.0rc2/tests/conftest.py` & `sbot-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_arduino.py` & `sbot-1.1.0/tests/test_arduino.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_metadata.py` & `sbot-1.1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_motor_board.py` & `sbot-1.1.0/tests/test_motor_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_power_board.py` & `sbot-1.1.0/tests/test_power_board.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,17 +106,17 @@
     # Test that we can get the power board regulator voltage
     assert power_board.status.regulator_voltage == 5.234
 
     # Test that we can get the power board start button status
     assert power_board._start_button() is True
 
     # Test that we can play a note using the Note class
-    power_board.piezo.buzz(0.1, Note.C6)
+    power_board.piezo.buzz(Note.C6, 0.1)
     # And using a float
-    power_board.piezo.buzz(0.2345, 261.63)
+    power_board.piezo.buzz(261.63, 0.2345)
 
     # Test that we can reset the power board
     power_board.reset()
 
 
 def test_power_board_leds(powerboard_serial: MockPowerBoard) -> None:
     """
@@ -307,37 +307,37 @@
     with pytest.raises(TypeError):
         power_board.outputs[None].is_enabled = True
     with pytest.raises(TypeError):
         power_board.outputs[1.5].is_enabled = True
 
     # Test that we can't buzz an invalid note frequency
     with pytest.raises(ValueError):
-        power_board.piezo.buzz(0.1, -1)
+        power_board.piezo.buzz(-1, 0.1)
     with pytest.raises(ValueError):
-        power_board.piezo.buzz(0.1, 0)
+        power_board.piezo.buzz(0, 0.1)
     with pytest.raises(ValueError):
-        power_board.piezo.buzz(0.1, 10001)
+        power_board.piezo.buzz(10001, 0.1)
 
     # Test that we can't buzz an invalid note frequency type
     with pytest.raises(TypeError):
-        power_board.piezo.buzz(0.1, None)
+        power_board.piezo.buzz(None, 0.1)
     with pytest.raises(TypeError):
-        power_board.piezo.buzz(0.1, {})
+        power_board.piezo.buzz({}, 0.1)
 
     # Test that we can't buzz an invalid note duration
     with pytest.raises(ValueError):
-        power_board.piezo.buzz(-1, 1000)
+        power_board.piezo.buzz(1000, -1)
     with pytest.raises(ValueError):
-        power_board.piezo.buzz(10**100, 1000)
+        power_board.piezo.buzz(1000, 10**100)
 
     # Test that we can't buzz an invalid note duration type
     with pytest.raises(TypeError):
-        power_board.piezo.buzz(None, 1000)
+        power_board.piezo.buzz(1000, None)
     with pytest.raises(TypeError):
-        power_board.piezo.buzz({}, 1000)
+        power_board.piezo.buzz(1000, {})
 
 
 def test_power_board_discovery(monkeypatch) -> None:
     """
     Test that discovery finds power boards from USB serial ports.
 
     Test that different USB pid/vid combinations are ignored.
```

### Comparing `sbot-1.0.0rc2/tests/test_sbot.py` & `sbot-1.1.0/tests/test_sbot.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_serial_wrapper.py` & `sbot-1.1.0/tests/test_serial_wrapper.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_servo_board.py` & `sbot-1.1.0/tests/test_servo_board.py`

 * *Files identical despite different names*

### Comparing `sbot-1.0.0rc2/tests/test_timeout.py` & `sbot-1.1.0/tests/test_timeout.py`

 * *Files identical despite different names*

