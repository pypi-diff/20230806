# Comparing `tmp/streamdeckapi-0.0.8.tar.gz` & `tmp/streamdeckapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeckapi-0.0.8.tar", last modified: Fri Jun 16 16:03:30 2023, max compression
+gzip compressed data, was "streamdeckapi-0.0.9.tar", last modified: Fri Jul 14 15:33:51 2023, max compression
```

## Comparing `streamdeckapi-0.0.8.tar` & `streamdeckapi-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/streamdeckapi/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-16 16:03:18.000000 streamdeckapi-0.0.8/streamdeckapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.014818 streamdeckapi-0.0.8/streamdeckapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 16:03:30.000000 streamdeckapi-0.0.8/streamdeckapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:33:51.845786 streamdeckapi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-14 15:33:51.845786 streamdeckapi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:33:51.845786 streamdeckapi-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:33:51.845786 streamdeckapi-0.0.9/streamdeckapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/streamdeckapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/streamdeckapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/streamdeckapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/streamdeckapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/streamdeckapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-14 15:33:41.000000 streamdeckapi-0.0.9/streamdeckapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:33:51.845786 streamdeckapi-0.0.9/streamdeckapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-14 15:33:51.000000 streamdeckapi-0.0.9/streamdeckapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 15:33:51.000000 streamdeckapi-0.0.9/streamdeckapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:33:51.000000 streamdeckapi-0.0.9/streamdeckapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-14 15:33:51.000000 streamdeckapi-0.0.9/streamdeckapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-14 15:33:51.000000 streamdeckapi-0.0.9/streamdeckapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 15:33:51.000000 streamdeckapi-0.0.9/streamdeckapi.egg-info/top_level.txt
```

### Comparing `streamdeckapi-0.0.8/PKG-INFO` & `streamdeckapi-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: streamdeckapi
-Version: 0.0.8
-Summary: Stream Deck API Library
-Home-page: https://github.com/Patrick762/streamdeckapi
-Author: Patrick762
-Author-email: <pip-stream-deck-api@hosting-rt.de>
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
 [![PyPI version](https://badge.fury.io/py/streamdeckapi.svg)](https://badge.fury.io/py/streamdeckapi)
 
 # streamdeckapi
 Stream Deck API Library for Home Assistant Stream Deck Integration
 
 Only compatible with separate [Stream Deck Plugin](https://github.com/Patrick762/streamdeckapi-plugin) or the bundled server.
 
@@ -32,23 +16,22 @@
 Cairo Installation for Windows:
 ```bash
 pip install pipwin
 
 pipwin install cairocffi
 ```
 
-The event `doubleTap` is not working with this server software.
-
 ### Limitations
-Discovery might not work.
+- Slow icon updates on Raspberry Pi Zero
+- No `doubleTap` event
 
 ### Installation on Linux / Raspberry Pi
 
 Install requirements:
-`sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5`
+`sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5 libgtk-3-dev python3-pip`
 
 Allow all users non-root access to Stream Deck Devices:
 ```bash
 sudo tee /etc/udev/rules.d/10-streamdeck.rules << EOF
 SUBSYSTEMS=="usb", ATTRS{idVendor}=="0fd9", GROUP="users", TAG+="uaccess"
 EOF
 ```
@@ -59,7 +42,30 @@
 Install the package:
 `pip install streamdeckapi`
 
 Reboot your system
 
 Start the server:
 `streamdeckapi-server`
+
+### Example service
+To run the server on startup, you can use the following config in the file `/etc/systemd/system/streamdeckapi.service`:
+
+```conf
+[Unit]
+Description=Stream Deck API Service
+Wants=network-online.target
+After=network.target
+
+[Service]
+WorkingDirectory=/home/pi
+ExecStart=/home/pi/.local/bin/streamdeckapi-server
+User=pi
+StandardOutput=console
+
+[Install]
+WantedBy=multi-user.target
+```
+
+To start the service, run `sudo systemctl start streamdeckapi.service`.
+
+To enable the service, run `sudo systemctl enable streamdeckapi.service`.
```

### Comparing `streamdeckapi-0.0.8/setup.py` & `streamdeckapi-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "Stream Deck API Library"
 
 # Setting up
 setup(
     name="streamdeckapi",
     version=VERSION,
     author="Patrick762",
```

### Comparing `streamdeckapi-0.0.8/streamdeckapi/api.py` & `streamdeckapi-0.0.9/streamdeckapi/api.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.8/streamdeckapi/server.py` & `streamdeckapi-0.0.9/streamdeckapi/server.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.8/streamdeckapi/tools.py` & `streamdeckapi-0.0.9/streamdeckapi/tools.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.8/streamdeckapi/types.py` & `streamdeckapi-0.0.9/streamdeckapi/types.py`

 * *Files identical despite different names*

### Comparing `streamdeckapi-0.0.8/streamdeckapi.egg-info/PKG-INFO` & `streamdeckapi-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeckapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stream Deck API Library
 Home-page: https://github.com/Patrick762/streamdeckapi
 Author: Patrick762
 Author-email: <pip-stream-deck-api@hosting-rt.de>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -32,23 +32,22 @@
 Cairo Installation for Windows:
 ```bash
 pip install pipwin
 
 pipwin install cairocffi
 ```
 
-The event `doubleTap` is not working with this server software.
-
 ### Limitations
-Discovery might not work.
+- Slow icon updates on Raspberry Pi Zero
+- No `doubleTap` event
 
 ### Installation on Linux / Raspberry Pi
 
 Install requirements:
-`sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5`
+`sudo apt install -y libudev-dev libusb-1.0-0-dev libhidapi-libusb0 libjpeg-dev zlib1g-dev libopenjp2-7 libtiff5 libgtk-3-dev python3-pip`
 
 Allow all users non-root access to Stream Deck Devices:
 ```bash
 sudo tee /etc/udev/rules.d/10-streamdeck.rules << EOF
 SUBSYSTEMS=="usb", ATTRS{idVendor}=="0fd9", GROUP="users", TAG+="uaccess"
 EOF
 ```
@@ -59,7 +58,30 @@
 Install the package:
 `pip install streamdeckapi`
 
 Reboot your system
 
 Start the server:
 `streamdeckapi-server`
+
+### Example service
+To run the server on startup, you can use the following config in the file `/etc/systemd/system/streamdeckapi.service`:
+
+```conf
+[Unit]
+Description=Stream Deck API Service
+Wants=network-online.target
+After=network.target
+
+[Service]
+WorkingDirectory=/home/pi
+ExecStart=/home/pi/.local/bin/streamdeckapi-server
+User=pi
+StandardOutput=console
+
+[Install]
+WantedBy=multi-user.target
+```
+
+To start the service, run `sudo systemctl start streamdeckapi.service`.
+
+To enable the service, run `sudo systemctl enable streamdeckapi.service`.
```

