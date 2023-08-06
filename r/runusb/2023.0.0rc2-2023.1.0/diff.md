# Comparing `tmp/runusb-2023.0.0rc2.tar.gz` & `tmp/runusb-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runusb-2023.0.0rc2.tar", last modified: Sat Jul 29 14:07:07 2023, max compression
+gzip compressed data, was "runusb-2023.1.0.tar", last modified: Sun Aug  6 13:00:53 2023, max compression
```

## Comparing `runusb-2023.0.0rc2.tar` & `runusb-2023.1.0.tar`

### file list

```diff
@@ -1,16 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/runusb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/runusb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11238 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/runusb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/runusb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.719102 runusb-2023.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.707101 runusb-2023.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.711102 runusb-2023.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-06 13:00:34.000000 runusb-2023.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-06 13:00:34.000000 runusb-2023.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-06 13:00:34.000000 runusb-2023.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-06 13:00:53.719102 runusb-2023.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-06 13:00:34.000000 runusb-2023.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 13:00:34.000000 runusb-2023.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.711102 runusb-2023.1.0/runusb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:34.000000 runusb-2023.1.0/runusb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14197 2023-08-06 13:00:34.000000 runusb-2023.1.0/runusb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.715102 runusb-2023.1.0/runusb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-06 13:00:53.000000 runusb-2023.1.0/runusb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-06 13:00:53.000000 runusb-2023.1.0/runusb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:00:53.000000 runusb-2023.1.0/runusb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 13:00:53.000000 runusb-2023.1.0/runusb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-06 13:00:53.000000 runusb-2023.1.0/runusb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 13:00:53.000000 runusb-2023.1.0/runusb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.711102 runusb-2023.1.0/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.715102 runusb-2023.1.0/script/linting/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       89 2023-08-06 13:00:34.000000 runusb-2023.1.0/script/linting/lint
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-06 13:00:34.000000 runusb-2023.1.0/script/linting/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.715102 runusb-2023.1.0/script/typing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-08-06 13:00:34.000000 runusb-2023.1.0/script/typing/check
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 13:00:34.000000 runusb-2023.1.0/script/typing/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-06 13:00:53.719102 runusb-2023.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:00:34.000000 runusb-2023.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.711102 runusb-2023.1.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.715102 runusb-2023.1.0/stubs/RPi/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-06 13:00:34.000000 runusb-2023.1.0/stubs/RPi/GPIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:34.000000 runusb-2023.1.0/stubs/RPi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:00:53.719102 runusb-2023.1.0/stubs/logger_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-06 13:00:34.000000 runusb-2023.1.0/stubs/logger_extras/__init__.pyi
```

### Comparing `runusb-2023.0.0rc2/LICENSE` & `runusb-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runusb-2023.0.0rc2/runusb/__main__.py` & `runusb-2023.1.0/runusb/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import atexit
 import itertools
+import json
 import logging
 import os
 import select
 import signal
 import subprocess
 import sys
 import time
@@ -19,14 +20,19 @@
     import RPi.GPIO as GPIO
     IS_PI = True
 except ImportError:
     IS_PI = False
 
 from logger_extras import RelativeTimeFilter, TieredFormatter
 
+try:
+    from logger_extras import MQTTHandler  # type: ignore[attr-defined]
+except ImportError:
+    MQTTHandler = None
+
 REL_TIME_FILTER: RelativeTimeFilter | None = None
 
 
 logging.raiseExceptions = False  # Don't print stack traces when the USB is removed
 LOGGER = logging.getLogger('runusb')
 
 PROC_FILE = '/proc/mounts'
@@ -34,14 +40,27 @@
 METADATA_FILENAME = 'metadata.json'
 LOG_NAME = 'log.txt'
 USERCODE_LEVEL = 35  # Between INFO and WARNING
 logging.addLevelName(USERCODE_LEVEL, "USERCODE")
 
 # the directory under which all USBs will be mounted
 MOUNTPOINT_DIR = os.environ.get('RUNUSB_MOUNTPOINT_DIR', '/media')
+# This will be populated if we have the config file
+# url format: mqtt[s]://[<username>[:<password>]@]<host>[:<port>]/<topic_root>
+MQTT_URL = None
+MQTT_CONFIG_FILE = '/etc/sbot/mqtt.conf'
+
+
+class MQTTVariables(NamedTuple):
+    host: str
+    port: int | None
+    topic_prefix: str
+    use_tls: bool
+    username: str | None
+    password: str | None
 
 
 class Mountpoint(NamedTuple):
     mountpoint: str
     filesystem: str
 
 
@@ -172,14 +191,17 @@
 
 class RobotUSBHandler(USBHandler):
     def __init__(self, mountpoint_path: str) -> None:
         self._setup_logging(mountpoint_path)
         LED_CONTROLLER.yellow()
         env = dict(os.environ)
         env["SBOT_METADATA_PATH"] = MOUNTPOINT_DIR
+        if MQTT_URL is not None:
+            # pass the mqtt url to the robot for camera images
+            env["SBOT_MQTT_URL"] = MQTT_URL
         self.process = subprocess.Popen(
             [sys.executable, '-u', ROBOT_FILE],
             stdin=subprocess.DEVNULL,
             stderr=subprocess.STDOUT,
             stdout=subprocess.PIPE,
             bufsize=1,  # line buffered
             cwd=mountpoint_path,
@@ -339,20 +361,88 @@
         if mountpoint.mountpoint == '/':
             return False
 
         # Defer to the declared filter by path
         return detect_usb_type(mountpoint.mountpoint) is not USBType.INVALID
 
 
+def set_mqtt_url(config: MQTTVariables) -> None:
+    global MQTT_URL
+    if config.username is not None and config.password is not None:
+        auth = f"{config.username}:{config.password}@"
+    elif config.username is not None:
+        auth = f"{config.username}@"
+    else:
+        auth = ""
+
+    port_str = (f":{config.port}" if config.port is not None else "")
+    scheme = 'mqtts' if config.use_tls else 'mqtt'
+
+    MQTT_URL = (
+        f"{scheme}://{auth}{config.host}{port_str}/{config.topic_prefix}"
+    )
+
+
+def read_mqtt_config_file() -> MQTTVariables | None:
+    """
+    Read the MQTT config file and return the config.
+
+    Returns None if the file does not exist or is invalid.
+    """
+    if not os.path.exists(MQTT_CONFIG_FILE):
+        return None
+
+    try:
+        with open(MQTT_CONFIG_FILE) as f:
+            config_dict = json.load(f)
+            config = MQTTVariables(
+                host=config_dict['host'],
+                port=config_dict.get('port', None),
+                topic_prefix=config_dict['topic_prefix'],
+                use_tls=config_dict.get('use_tls', False),
+                username=config_dict.get('username', None),
+                password=config_dict.get('password', None),
+            )
+            set_mqtt_url(config)
+            return config
+    except Exception as e:
+        LOGGER.error(f"Failed to read MQTT config file: {e}")
+        return None
+
+
 def setup_usercode_logging() -> None:
     global REL_TIME_FILTER
     usercode_logger = logging.getLogger('usercode')
     REL_TIME_FILTER = RelativeTimeFilter()
     usercode_logger.addFilter(REL_TIME_FILTER)
 
+    if MQTTHandler is not None:
+        # If we have relative logging, we should also have the MQTT handler
+        mqtt_config = read_mqtt_config_file()
+
+        if mqtt_config is not None:
+            handler = MQTTHandler(
+                host=mqtt_config.host,
+                topic=f"{mqtt_config.topic_prefix}/logs",
+                port=mqtt_config.port,
+                use_tls=mqtt_config.use_tls,
+                username=mqtt_config.username,
+                password=mqtt_config.password,
+                connected_topic=f"{mqtt_config.topic_prefix}/connected",
+            )
+
+            handler.setLevel(logging.INFO)
+            handler.setFormatter(TieredFormatter(
+                fmt='[%(reltime)08.3f - %(levelname)s] %(message)s',
+                level_fmts={
+                    USERCODE_LEVEL: '[%(reltime)08.3f] %(message)s',
+                },
+            ))
+            usercode_logger.addHandler(handler)
+
 
 def main():
     logging.basicConfig(level=logging.DEBUG)
     setup_usercode_logging()
 
     fstab_reader = FSTabReader()
```

### Comparing `runusb-2023.0.0rc2/setup.cfg` & `runusb-2023.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [metadata]
 name = runusb
-version = 2023.0.0rc2
 description = Automagic running of USB sticks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = "Alistair Lynn"
 url = https://github.com/sourcebots/runusb
 
 [options]
 python_requires = >=3.8
 packages = find:
 install_requires = 
-	logger-extras==0.2.0
+	logger-extras==0.3.2
 	rpi.GPIO==0.7.1
 
+[options.extras_require]
+mqtt = logger-extras[mqtt]==0.3.3
+
 [options.entry_points]
 console_scripts = 
 	runusb = runusb.__main__:main
 
 [flake8]
 exclude = 
 	.eggs,
```

