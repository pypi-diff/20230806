# Comparing `tmp/hahomematic-2023.8.1.tar.gz` & `tmp/hahomematic-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.8.1.tar", last modified: Fri Aug  4 15:39:34 2023, max compression
+gzip compressed data, was "hahomematic-2023.8.2.tar", last modified: Sun Aug  6 16:11:05 2023, max compression
```

## Comparing `hahomematic-2023.8.1.tar` & `hahomematic-2023.8.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.599002 hahomematic-2023.8.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.599002 hahomematic-2023.8.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    55112 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    48499 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.599002 hahomematic-2023.8.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-04 15:39:33.000000 hahomematic-2023.8.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:39:32.000000 hahomematic-2023.8.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.948033 hahomematic-2023.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-06 16:11:05.948033 hahomematic-2023.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.944033 hahomematic-2023.8.2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.944033 hahomematic-2023.8.2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25201 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55787 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49143 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.944033 hahomematic-2023.8.2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.944033 hahomematic-2023.8.2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.948033 hahomematic-2023.8.2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.948033 hahomematic-2023.8.2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.948033 hahomematic-2023.8.2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:11:05.944033 hahomematic-2023.8.2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-06 16:11:05.000000 hahomematic-2023.8.2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-08-06 16:11:05.000000 hahomematic-2023.8.2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:11:05.000000 hahomematic-2023.8.2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:11:03.000000 hahomematic-2023.8.2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 16:11:05.000000 hahomematic-2023.8.2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 16:11:05.000000 hahomematic-2023.8.2/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-08-06 16:10:31.000000 hahomematic-2023.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-06 16:11:05.948033 hahomematic-2023.8.2/setup.cfg
```

### Comparing `hahomematic-2023.8.1/LICENSE` & `hahomematic-2023.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/PKG-INFO` & `hahomematic-2023.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.8.1/README.md` & `hahomematic-2023.8.2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/__init__.py` & `hahomematic-2023.8.2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/caches/dynamic.py` & `hahomematic-2023.8.2/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/caches/persistent.py` & `hahomematic-2023.8.2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/caches/visibility.py` & `hahomematic-2023.8.2/hahomematic/caches/visibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     PARAM_TEMPERATURE_MINIMUM,
     PARAMSET_KEY_MASTER,
     PARAMSET_KEY_VALUES,
     HmPlatform,
 )
 from hahomematic.platforms.custom.definition import get_required_parameters
 from hahomematic.platforms.generic import entity as hmge
+from hahomematic.support import reduce_args
 
 _LOGGER = logging.getLogger(__name__)
 
 # Define which additional parameters from MASTER paramset should be created as entity.
 # By default these are also on the _HIDDEN_PARAMETERS, which prevents these entities
 # from being display by default. Usually these enties are used within custom entities,
 # and not for general display.
@@ -648,15 +649,15 @@
                 ) as fptr:
                     for file_line in fptr.readlines():
                         if "#" not in file_line:
                             self._raw_un_ignore_list.add(file_line.strip())
             except Exception as ex:
                 _LOGGER.warning(
                     "LOAD failed: Could not read unignore file %s",
-                    ex.args,
+                    reduce_args(args=ex.args),
                 )
 
         if self._central.config.load_un_ignore:
             await self._central.async_add_executor_job(_load)
 
         for line in self._raw_un_ignore_list:
             if "#" not in line:
```

### Comparing `hahomematic-2023.8.1/hahomematic/central_unit.py` & `hahomematic-2023.8.2/hahomematic/central_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 from hahomematic.platforms.update import HmUpdate
 from hahomematic.support import (
     HM_INTERFACE_EVENT_SCHEMA,
     SystemInformation,
     check_or_create_directory,
     check_password,
     get_device_address,
+    reduce_args,
 )
 from hahomematic.xml_rpc_proxy import XmlRpcProxy
 
 _LOGGER = logging.getLogger(__name__)
 _R = TypeVar("_R")
 _T = TypeVar("_T")
 
@@ -401,15 +402,15 @@
                     interface_id=interface_config.interface_id,
                     interface_event_type=HmInterfaceEventType.PROXY,
                     data={ATTR_AVAILABLE: False},
                 )
                 _LOGGER.warning(
                     "CREATE_CLIENTS failed: No connection to interface %s [%s]",
                     interface_config.interface_id,
-                    ex.args,
+                    reduce_args(args=ex.args),
                 )
 
         if self.has_clients:
             _LOGGER.debug(
                 "CREATE_CLIENTS: All clients successfully created for %s",
                 self._attr_name,
             )
@@ -518,14 +519,16 @@
             for interface_config in self.config.interface_configs:
                 client = await hmcl.create_client(
                     central=self, interface_config=interface_config, local_ip=local_ip
                 )
                 if not system_information.serial:
                     system_information = client.system_information
             return system_information
+        except NoClients:
+            raise
         except Exception as ex:
             _LOGGER.warning(ex)
             raise
 
     def get_client(self, interface_id: str) -> hmcl.Client:
         """Return a client by interface_id. #CC."""
         if not self.has_client(interface_id=interface_id):
@@ -627,16 +630,15 @@
             _LOGGER.warning("LOAD_CACHES failed: Unable to load caches for %s", self._attr_name)
             await self.clear_all_caches()
 
     async def _create_devices(self) -> None:
         """Trigger creation of the objects that expose the functionality."""
         if not self._clients:
             raise HaHomematicException(
-                f"create_devices: "
-                f"No clients initialized. Not starting central {self._attr_name}."
+                f"CREATE_DEVICES failed: No clients initialized. Not starting central {self._attr_name}."
             )
         _LOGGER.debug("CREATE_DEVICES: Starting to create devices for %s", self._attr_name)
 
         new_devices = set[HmDevice]()
         for interface_id in self._clients:
             if not self.paramset_descriptions.has_interface_id(interface_id=interface_id):
                 _LOGGER.debug(
@@ -658,29 +660,29 @@
                         device_address=device_address,
                     )
 
                 except Exception as err:  # pragma: no cover
                     _LOGGER.error(
                         "CREATE_DEVICES failed: %s [%s] Unable to create device: %s, %s",
                         type(err).__name__,
-                        err.args,
+                        reduce_args(args=err.args),
                         interface_id,
                         device_address,
                     )
                 try:
                     if device:
                         create_entities_and_append_to_device(device=device)
                         await device.load_value_cache()
                         new_devices.add(device)
                         self._devices[device_address] = device
                 except Exception as err:  # pragma: no cover
                     _LOGGER.error(
                         "CREATE_DEVICES failed: %s [%s] Unable to create entities: %s, %s",
                         type(err).__name__,
-                        err.args,
+                        reduce_args(args=err.args),
                         interface_id,
                         device_address,
                     )
         _LOGGER.debug("CREATE_DEVICES: Finished creating devices for %s", self._attr_name)
 
         if new_devices:
             self.fire_system_event_callback(name=HH_EVENT_DEVICES_CREATED, new_devices=new_devices)
@@ -754,15 +756,19 @@
             client = self._clients[interface_id]
             for dev_desc in device_descriptions:
                 try:
                     self.device_descriptions.add_device_description(interface_id, dev_desc)
                     if dev_desc[HM_ADDRESS] not in known_addresses:
                         await client.fetch_paramset_descriptions(dev_desc)
                 except Exception as err:  # pragma: no cover
-                    _LOGGER.error("ADD_NEW_DEVICES failed: %s [%s]", type(err).__name__, err.args)
+                    _LOGGER.error(
+                        "ADD_NEW_DEVICES failed: %s [%s]",
+                        type(err).__name__,
+                        reduce_args(args=err.args),
+                    )
 
             await self.device_descriptions.save()
             await self.paramset_descriptions.save()
             await self.device_details.load()
             await self.device_data.load()
             await self._create_devices()
 
@@ -788,26 +794,26 @@
         if (channel_address, parameter) in self._entity_event_subscriptions:
             try:
                 for callback in self._entity_event_subscriptions[(channel_address, parameter)]:
                     callback(value)
             except RuntimeError as rte:  # pragma: no cover
                 _LOGGER.debug(
                     "event: RuntimeError [%s]. Failed to call callback for: %s, %s, %s",
-                    rte.args,
+                    reduce_args(args=rte.args),
                     interface_id,
                     channel_address,
                     parameter,
                 )
             except Exception as ex:  # pragma: no cover
                 _LOGGER.warning(
                     "EVENT failed: Unable to call callback for: %s, %s, %s, %s",
                     interface_id,
                     channel_address,
                     parameter,
-                    ex.args,
+                    reduce_args(args=ex.args),
                 )
 
     @callback_system_event(name=HH_EVENT_LIST_DEVICES)
     def list_devices(self, interface_id: str) -> list[dict[str, Any]]:
         """Return already existing devices to CCU / Homegear."""
         _LOGGER.debug("list_devices: interface_id = %s", interface_id)
 
@@ -947,19 +953,17 @@
         """Add an executor job from within the event_loop."""
         try:
             task = self._loop.run_in_executor(None, target, *args)
             self._tasks.add(task)
             task.add_done_callback(self._tasks.remove)
             return task
         except (CancelledError, asyncio.TimeoutError) as err:  # pragma: no cover
-            _LOGGER.debug(
-                "async_add_executor_job: task cancelled for %s",
-                self._attr_name,
-            )
-            raise HaHomematicException from err
+            message = f"async_add_executor_job: task cancelled for {self._attr_name} [{reduce_args(args=err.args)}]"
+            _LOGGER.debug(message)
+            raise HaHomematicException(message) from err
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU / Homegear."""
         if client := self.primary_client:
             return await client.execute_program(pid=pid)
         return False
 
@@ -1063,15 +1067,17 @@
 
         # Events like INTERFACE, KEYPRESS, ...
         """
         for callback_handler in self._callback_ha_event:
             try:
                 callback_handler(event_type, event_data)
             except Exception as ex:
-                _LOGGER.error("FIRE_HA_EVENT_CALLBACK: Unable to call handler: %s", ex.args)
+                _LOGGER.error(
+                    "FIRE_HA_EVENT_CALLBACK: Unable to call handler: %s", reduce_args(args=ex.args)
+                )
 
     def register_entity_event_callback(self, callback_handler: Callable) -> None:
         """Register entity_event callback in central."""
         self._callback_entity_event.add(callback_handler)
 
     def unregister_entity_event_callback(self, callback_handler: Callable) -> None:
         """Un register entity_event callback in central."""
@@ -1087,15 +1093,18 @@
         Not used by HA.
         Re-Fired events from CCU for parameter updates.
         """
         for callback_handler in self._callback_entity_event:
             try:
                 callback_handler(interface_id, channel_address, parameter, value)
             except Exception as ex:
-                _LOGGER.error("FIRE_ENTITY_EVENT_CALLBACK: Unable to call handler: %s", ex.args)
+                _LOGGER.error(
+                    "FIRE_ENTITY_EVENT_CALLBACK: Unable to call handler: %s",
+                    reduce_args(args=ex.args),
+                )
 
     def register_entity_data_event_callback(self, callback_handler: Callable) -> None:
         """Register entity_event callback in central."""
         self._callback_entity_data_event.add(callback_handler)
 
     def unregister_entity_data_event_callback(self, callback_handler: Callable) -> None:
         """Un register entity_event callback in central."""
@@ -1110,15 +1119,16 @@
         Fires parameter data updates as events with entity.
         """
         for callback_handler in self._callback_entity_data_event:
             try:
                 callback_handler(interface_id, entity)
             except Exception as ex:
                 _LOGGER.error(
-                    "FIRE_ENTITY_DATA_EVENT_CALLBACK: Unable to call handler: %s", ex.args
+                    "FIRE_ENTITY_DATA_EVENT_CALLBACK: Unable to call handler: %s",
+                    reduce_args(args=ex.args),
                 )
 
     def register_system_event_callback(self, callback_handler: Callable) -> None:
         """Register system_event callback in central."""
         self._callback_system_event.add(callback_handler)
 
     def unregister_system_event_callback(self, callback_handler: Callable) -> None:
@@ -1132,15 +1142,18 @@
 
         e.g. DEVICES_CREATED, HUB_REFRESHED
         """
         for callback_handler in self._callback_system_event:
             try:
                 callback_handler(name, **kwargs)
             except Exception as ex:
-                _LOGGER.error("FIRE_SYSTEM_EVENT_CALLBACK: Unable to call handler: %s", ex.args)
+                _LOGGER.error(
+                    "FIRE_SYSTEM_EVENT_CALLBACK: Unable to call handler: %s",
+                    reduce_args(args=ex.args),
+                )
 
 
 class ConnectionChecker(threading.Thread):
     """Periodically check Connection to CCU / Homegear."""
 
     def __init__(self, central: CentralUnit) -> None:
         """Init the connection checker."""
@@ -1195,18 +1208,24 @@
                         await asyncio.gather(*reconnects)
                         if self._central.available:
                             # refresh cache
                             await self._central.device_data.load()
                             # refresh entity data
                             await self._central.device_data.refresh_entity_data()
             except NoConnection as nex:
-                _LOGGER.error("CHECK_CONNECTION failed: no connection: %s", nex.args)
+                _LOGGER.error(
+                    "CHECK_CONNECTION failed: no connection: %s", reduce_args(args=nex.args)
+                )
                 continue
             except Exception as err:
-                _LOGGER.error("CHECK_CONNECTION failed: %s [%s]", type(err).__name__, err.args)
+                _LOGGER.error(
+                    "CHECK_CONNECTION failed: %s [%s]",
+                    type(err).__name__,
+                    reduce_args(args=err.args),
+                )
             if self._active:
                 await asyncio.sleep(config.CONNECTION_CHECKER_INTERVAL)
 
 
 class CentralConfig:
     """Config for a Client."""
```

### Comparing `hahomematic-2023.8.1/hahomematic/client.py` & `hahomematic-2023.8.2/hahomematic/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 from hahomematic.support import (
     ProgramData,
     SystemInformation,
     SystemVariableData,
     build_headers,
     build_xml_rpc_uri,
     get_channel_no,
+    reduce_args,
 )
 from hahomematic.xml_rpc_proxy import XmlRpcProxy
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Client(ABC):
@@ -122,15 +123,15 @@
                 forced_availability=HmForcedDeviceAvailability.NOT_SET
             )
             _LOGGER.debug("PROXY_INIT: Proxy for %s initialized", self.interface_id)
         except BaseHomematicException as hhe:
             _LOGGER.warning(
                 "PROXY_INIT failed: %s [%s] Unable to initialize proxy for %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 self.interface_id,
             )
             self.last_updated = INIT_DATETIME
             return PROXY_INIT_FAILED
         self.last_updated = datetime.now()
         return PROXY_INIT_SUCCESS
 
@@ -145,15 +146,15 @@
         try:
             _LOGGER.debug("PROXY_DE_INIT: init('%s')", self._config.init_url)
             await self._proxy.init(self._config.init_url)
         except BaseHomematicException as hhe:
             _LOGGER.warning(
                 "PROXY_DE_INIT failed: %s [%s] Unable to de-initialize proxy for %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 self.interface_id,
             )
             return PROXY_DE_INIT_FAILED
 
         self.last_updated = INIT_DATETIME
         return PROXY_DE_INIT_SUCCESS
 
@@ -317,24 +318,28 @@
         return None
 
     async def get_all_device_descriptions(self) -> Any:
         """Get device descriptions from CCU / Homegear."""
         try:
             return await self._proxy.listDevices()
         except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_DEVICE_DESCRIPTIONS failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "GET_ALL_DEVICE_DESCRIPTIONS failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
         return None
 
     async def get_device_descriptions(self, device_address: str) -> Any:
         """Get device descriptions from CCU / Homegear."""
         try:
             if device_descriptions := await self._proxy_read.getDeviceDescription(device_address):
                 return [device_descriptions]
         except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_DEVICE_DESCRIPTIONS failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "GET_DEVICE_DESCRIPTIONS failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
         return None
 
     # pylint: disable=invalid-name
     async def set_install_mode(
         self,
         on: bool = True,
         t: int = 60,
@@ -349,24 +354,28 @@
                 if device_address:
                     args.append(device_address)
                 else:
                     args.append(mode)
 
             await self._proxy.setInstallMode(*args)
         except BaseHomematicException as hhe:
-            _LOGGER.warning("SET_INSTALL_MODE failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "SET_INSTALL_MODE failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
             return False
         return True
 
     async def get_install_mode(self) -> Any:
         """Get remaining time in seconds install mode is active from CCU / Homegear."""
         try:
             return await self._proxy.getInstallMode()
         except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_INSTALL_MODE failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "GET_INSTALL_MODE failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
         return 0
 
     async def get_value(
         self,
         channel_address: str,
         paramset_key: str,
         parameter: str,
@@ -387,20 +396,20 @@
                 await self._proxy_read.getParamset(channel_address, PARAMSET_KEY_MASTER) or {}
             )
             return paramset.get(parameter)
         except BaseHomematicException as hhe:
             _LOGGER.debug(
                 "GET_VALUE failed with %s [%s]: %s, %s, %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 channel_address,
                 parameter,
                 paramset_key,
             )
-            raise hhe
+            raise
 
     async def _set_value(
         self,
         channel_address: str,
         parameter: str,
         value: Any,
         rx_mode: str | None = None,
@@ -412,15 +421,15 @@
                 await self._proxy.setValue(channel_address, parameter, value, rx_mode)
             else:
                 await self._proxy.setValue(channel_address, parameter, value)
         except BaseHomematicException as hhe:
             _LOGGER.warning(
                 "SET_VALUE failed with %s [%s]: %s, %s, %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 channel_address,
                 parameter,
                 value,
             )
             return False
         return True
 
@@ -461,19 +470,19 @@
                 paramset_key,
             )
             return await self._proxy_read.getParamset(address, paramset_key)
         except BaseHomematicException as hhe:
             _LOGGER.debug(
                 "GET_PARAMSET failed with %s [%s]: %s, %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 address,
                 paramset_key,
             )
-            raise hhe
+            raise
 
     async def put_paramset(
         self,
         address: str,
         paramset_key: str,
         value: Any,
         rx_mode: str | None = None,
@@ -490,15 +499,15 @@
                 await self._proxy.putParamset(address, paramset_key, value, rx_mode)
             else:
                 await self._proxy.putParamset(address, paramset_key, value)
         except BaseHomematicException as hhe:
             _LOGGER.warning(
                 "PUT_PARAMSET failed: %s [%s] %s, %s, %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 address,
                 paramset_key,
                 value,
             )
             return False
         return True
 
@@ -519,15 +528,15 @@
                 paramset_description=parameter_data,
             )
         except BaseHomematicException as hhe:
             _LOGGER.warning(
                 "FETCH_PARAMSET_DESCRIPTION failed: "
                 "%s [%s] Unable to get paramset %s for channel_address %s",
                 hhe.name,
-                hhe.args,
+                reduce_args(args=hhe.args),
                 paramset_key,
                 channel_address,
             )
         if save_to_file:
             await self.central.paramset_descriptions.save()
 
     async def fetch_paramset_descriptions(self, device_description: dict[str, Any]) -> None:
@@ -577,15 +586,15 @@
                 paramsets[address][paramset_key] = await self._get_paramset_description(
                     address=address, paramset_key=paramset_key
                 )
             except BaseHomematicException as hhe:
                 _LOGGER.warning(
                     "GET_PARAMSET_DESCRIPTIONS failed with %s [%s] for %s address %s",
                     hhe.name,
-                    hhe.args,
+                    reduce_args(args=hhe.args),
                     paramset_key,
                     address,
                 )
         return paramsets
 
     async def _get_paramset_description(self, address: str, paramset_key: str) -> Any:
         """Get paramset description from CCU."""
@@ -628,15 +637,15 @@
                     "success" if result else "failed",
                 )
                 return result
             except BaseHomematicException as bex:
                 _LOGGER.warning(
                     "UPDATE_DEVICE_FIRMWARE failed: %s [%s]",
                     bex.name,
-                    bex.args,
+                    reduce_args(args=bex.args),
                 )
         return False
 
     async def update_paramset_descriptions(self, device_address: str) -> None:
         """Update paramsets descriptions for provided device_address."""
         if not self.central.device_descriptions.get_device_descriptions(
             interface_id=self.interface_id
@@ -716,15 +725,19 @@
         """Check if _proxy is still initialized."""
         try:
             await self._proxy.ping(self.interface_id)
             self.last_updated = datetime.now()
             self.central.increase_ping_count(interface_id=self.interface_id)
             return True
         except BaseHomematicException as hhe:
-            _LOGGER.debug("CHECK_CONNECTION_AVAILABILITY failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.debug(
+                "CHECK_CONNECTION_AVAILABILITY failed: %s [%s]",
+                hhe.name,
+                reduce_args(args=hhe.args),
+            )
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on CCU."""
         return await self._json_rpc_client.execute_program(pid=pid)
 
@@ -816,69 +829,81 @@
                     address,
                     await self._proxy_read.getMetadata(address, HM_NAME),
                 )
             except BaseHomematicException as hhe:
                 _LOGGER.warning(
                     "%s [%s] Failed to fetch name for device %s",
                     hhe.name,
-                    hhe.args,
+                    reduce_args(args=hhe.args),
                     address,
                 )
 
     async def check_connection_availability(self) -> bool:
         """Check if proxy is still initialized."""
         try:
             await self._proxy.clientServerInitialized(self.interface_id)
             self.last_updated = datetime.now()
             if self.supports_ping_pong:
                 self.central.increase_ping_count(interface_id=self.interface_id)
             return True
         except BaseHomematicException as hhe:
-            _LOGGER.debug("CHECK_CONNECTION_AVAILABILITY failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.debug(
+                "CHECK_CONNECTION_AVAILABILITY failed: %s [%s]",
+                hhe.name,
+                reduce_args(args=hhe.args),
+            )
         self.last_updated = INIT_DATETIME
         return False
 
     async def execute_program(self, pid: str) -> bool:
         """Execute a program on Homegear."""
         return True
 
     async def set_system_variable(self, name: str, value: Any) -> bool:
         """Set a system variable on CCU / Homegear."""
         try:
             await self._proxy.setSystemVariable(name, value)
         except BaseHomematicException as hhe:
-            _LOGGER.warning("SET_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "SET_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
             return False
         return True
 
     async def delete_system_variable(self, name: str) -> bool:
         """Delete a system variable from CCU / Homegear."""
         try:
             await self._proxy.deleteSystemVariable(name)
         except BaseHomematicException as hhe:
-            _LOGGER.warning("DELETE_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "DELETE_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
             return False
         return True
 
     async def get_system_variable(self, name: str) -> Any:
         """Get single system variable from CCU / Homegear."""
         try:
             return await self._proxy.getSystemVariable(name)
         except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "GET_SYSTEM_VARIABLE failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
 
     async def get_all_system_variables(self, include_internal: bool) -> list[SystemVariableData]:
         """Get all system variables from CCU / Homegear."""
         variables: list[SystemVariableData] = []
         try:
             if hg_variables := await self._proxy.getAllSystemVariables():
                 for name, value in hg_variables.items():
                     variables.append(SystemVariableData(name=name, value=value))
         except BaseHomematicException as hhe:
-            _LOGGER.warning("GET_ALL_SYSTEM_VARIABLES failed: %s [%s]", hhe.name, hhe.args)
+            _LOGGER.warning(
+                "GET_ALL_SYSTEM_VARIABLES failed: %s [%s]", hhe.name, reduce_args(args=hhe.args)
+            )
         return variables
 
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get all programs, if available."""
         return []
 
     async def get_all_rooms(self) -> dict[str, set[str]]:
@@ -1188,20 +1213,18 @@
                 if "Homegear" in self.version or "pydevccu" in self.version
                 else ClientCCU(client_config=self)
             ):
                 await client.init_client()
                 if await client.check_connection_availability():
                     return client
             raise NoConnection(f"No connection to {self.interface_id}")
-        except AuthFailure as auf:
-            raise AuthFailure(f"Unable to authenticate {auf.args}.") from auf
-        except NoConnection as noc:
-            raise noc
+        except (AuthFailure, NoConnection):
+            raise
         except Exception as exc:
-            raise NoConnection(f"Unable to connect {exc.args}.") from exc
+            raise NoConnection(f"Unable to connect {reduce_args(args=exc.args)}.") from exc
 
     def get_xml_rpc_proxy(self, auth_enabled: bool | None = None) -> XmlRpcProxy:
         """Return a XmlRPC proxy for backend communication."""
         central_config = self.central.config
         xml_rpc_headers = (
             build_headers(
                 username=central_config.username,
```

### Comparing `hahomematic-2023.8.1/hahomematic/const.py` & `hahomematic-2023.8.2/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/decorators.py` & `hahomematic-2023.8.2/hahomematic/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from inspect import getfullargspec
 import logging
 from typing import Any, ParamSpec, TypeVar
 
 from hahomematic import client as hmcl
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.platforms import entity as hme
+from hahomematic.support import reduce_args
 
 _LOGGER = logging.getLogger(__name__)
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
@@ -68,15 +69,17 @@
         if client := hmcl.get_client(interface_id=interface_id):
             client.last_updated = datetime.now()
             client.central.fire_system_event_callback(name=name, **kwargs)
     except Exception as err:  # pragma: no cover
         _LOGGER.warning(
             "EXEC_CALLBACK_SYSTEM_EVENT failed: Unable to reduce kwargs for callback_system_event"
         )
-        raise HaHomematicException("args-exception callback_system_event") from err
+        raise HaHomematicException(
+            f"args-exception callback_system_event [{reduce_args(args=err.args)}]"
+        ) from err
 
 
 def callback_event(func: Callable[P, R]) -> Callable[P, R]:
     """Check if callback_event is set and call it AFTER original function."""
 
     @wraps(func)
     def wrapper_callback_event(*args: P.args, **kwargs: P.kwargs) -> R:
@@ -93,15 +96,17 @@
             if client := hmcl.get_client(interface_id=interface_id):
                 client.last_updated = datetime.now()
                 client.central.fire_entity_event_callback(*args, **kwargs)
         except Exception as err:  # pragma: no cover
             _LOGGER.warning(
                 "EXEC_CALLBACK_ENTITY_EVENT failed: Unable to reduce kwargs for callback_event"
             )
-            raise HaHomematicException("args-exception callback_event") from err
+            raise HaHomematicException(
+                f"args-exception callback_event [{reduce_args(args=err.args)}]"
+            ) from err
 
     return wrapper_callback_event
 
 
 _CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
```

### Comparing `hahomematic-2023.8.1/hahomematic/exceptions.py` & `hahomematic-2023.8.2/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/exporter.py` & `hahomematic-2023.8.2/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/hmcli.py` & `hahomematic-2023.8.2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/json_rpc_client.py` & `hahomematic-2023.8.2/hahomematic/json_rpc_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import re
 from typing import Any, Final
 
 from aiohttp import (
     ClientConnectorCertificateError,
     ClientConnectorError,
     ClientError,
+    ClientResponse,
     ClientSession,
 )
 import orjson
 
 from hahomematic import central_unit as hmcu, config
 from hahomematic.const import (
     ATTR_NAME,
@@ -44,24 +45,26 @@
     SYSVAR_NAME,
     SYSVAR_TYPE,
     SYSVAR_TYPE_NUMBER,
     SYSVAR_UNIT,
     SYSVAR_VALUE,
     SYSVAR_VALUE_LIST,
 )
-from hahomematic.exceptions import ClientException
+from hahomematic.exceptions import AuthFailure, BaseHomematicException, ClientException
 from hahomematic.support import (
     ProgramData,
     SystemVariableData,
     get_tls_context,
     parse_sys_var,
+    reduce_args,
 )
 
 P_ERROR = "error"
 P_RESULT = "result"
+P_MESSAGE = "message"
 SESSION_ID: Final = "_session_id_"
 
 ALLOWED_METHOD_ON_FAILURE = ("Session.login",)
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -180,15 +183,15 @@
             session_id=session_id,
             method=method,
             extra_params=extra_params,
             use_default_params=use_default_params,
         )
 
         if extra_params:
-            _LOGGER.debug("POST method: %s, [%s]", method, extra_params)
+            _LOGGER.debug("POST method: %s [%s]", method, extra_params)
         else:
             _LOGGER.debug("POST method: %s", method)
 
         if not keep_session:
             await self._do_logout(session_id=session_id)
 
         return response
@@ -276,66 +279,89 @@
                 )
             else:
                 response = await self._client_session.post(
                     self._url, data=payload, headers=headers, timeout=config.TIMEOUT
                 )
             if response.status == 200:
                 self._connection_state.remove_issue(issuer=self)
-                try:
-                    return await response.json(encoding="utf-8")
-                except ValueError as ver:
-                    _LOGGER.debug(
-                        "DO_POST: ValueError [%s] Unable to parse JSON. Trying workaround",
-                        ver.args,
-                    )
-                    # Workaround for bug in CCU
-                    return orjson.loads((await response.json(encoding="utf-8")).replace("\\", ""))
-            else:
-                json_response = await response.json(encoding="utf-8")
-                message = f"Status: {response.status}"
+                json_response = await self._get_json_reponse(response=response)
+
                 if error := json_response[P_ERROR]:
-                    message = f"{message}: {error}"
-                raise ClientException(message)
+                    error_message = error[P_MESSAGE]
+                    message = f"POST method '{method}' failed: {error_message}"
+                    _LOGGER.debug(message)
+                    if error_message.startswith("access denied"):
+                        raise AuthFailure(message)
+                    raise ClientException(message)
+
+                return json_response
+
+            json_response = await self._get_json_reponse(response=response)
+            message = f"Status: {response.status}"
+            if error := json_response[P_ERROR]:
+                error_message = error[P_MESSAGE]
+                message = f"{message}: {error_message}"
+            raise ClientException(message)
+        except (AuthFailure, ClientException):
+            self._connection_state.add_issue(issuer=self)
+            await self.logout()
+            raise
         except ClientConnectorCertificateError as cccerr:
+            self.clear_session()
             message = f"ClientConnectorCertificateError[{cccerr}]"
             if self._tls is False and cccerr.ssl is True:
                 message = (
                     f"{message}. Possible reason: 'Automatic forwarding to HTTPS' is enabled in backend, "
                     f"but this integration is not configured to use TLS"
                 )
             raise ClientException(message) from cccerr
-        except ClientConnectorError as err:
-            raise ClientException from err
-        except ClientError as cce:
-            raise ClientException from cce
+        except (ClientConnectorError, ClientError) as cce:
+            self.clear_session()
+            raise ClientException(reduce_args(args=cce.args)) from cce
         except (OSError, TypeError, Exception) as ex:
-            raise ClientException from ex
+            self.clear_session()
+            raise ClientException(reduce_args(args=ex.args)) from ex
+
+    async def _get_json_reponse(self, response: ClientResponse) -> dict[str, Any] | Any:
+        """Return the json object from response."""
+        try:
+            return await response.json(encoding="utf-8")
+        except ValueError as ver:
+            _LOGGER.debug(
+                "DO_POST: ValueError [%s] Unable to parse JSON. Trying workaround",
+                reduce_args(args=ver.args),
+            )
+            # Workaround for bug in CCU
+            return orjson.loads((await response.json(encoding="utf-8")).replace("\\", ""))
 
     async def logout(self) -> None:
         """Logout of CCU."""
         try:
             await self._do_logout(self._session_id)
         except ClientException as clex:
-            self._handle_client_exception(method="LOGOUT", clex=clex)
+            self._handle_exception_log(method="LOGOUT", exception=clex)
             return
 
     async def _do_logout(self, session_id: str | None) -> None:
         """Logout of CCU."""
         if not session_id:
             _LOGGER.debug("DO_LOGOUT: Not logged in. Not logging out.")
             return
 
         method = "Session.logout"
         params = {SESSION_ID: session_id}
-        await self._do_post(
-            session_id=session_id,
-            method=method,
-            extra_params=params,
-        )
-        _LOGGER.debug("DO_LOGOUT: Method: %s [%s]", method, session_id)
+        try:
+            await self._do_post(
+                session_id=session_id,
+                method=method,
+                extra_params=params,
+            )
+            _LOGGER.debug("DO_LOGOUT: Method: %s [%s]", method, session_id)
+        finally:
+            self.clear_session()
 
     @property
     def _has_credentials(self) -> bool:
         """Return if credentials are available."""
         return self._username is not None and self._username != "" and self._password is not None
 
     async def execute_program(self, pid: str) -> bool:
@@ -349,15 +375,15 @@
 
             if json_result := response[P_RESULT]:
                 _LOGGER.debug(
                     "EXECUTE_PROGRAM: Result while executing program: %s",
                     str(json_result),
                 )
         except ClientException as clex:
-            self._handle_client_exception(method="EXECUTE_PROGRAM", clex=clex)
+            self._handle_exception_log(method="EXECUTE_PROGRAM", exception=clex)
             return False
 
         return True
 
     async def set_system_variable(self, name: str, value: Any) -> bool:
         """Set a system variable on CCU / Homegear."""
 
@@ -386,34 +412,38 @@
             _LOGGER.debug("SET_SYSTEM_VARIABLE: Setting System variable")
             if json_result := response[P_RESULT]:
                 _LOGGER.debug(
                     "SET_SYSTEM_VARIABLE: Result while setting variable: %s",
                     str(json_result),
                 )
         except ClientException as clex:
-            self._handle_client_exception(method="SET_SYSTEM_VARIABLE failed", clex=clex)
+            self._handle_exception_log(method="SET_SYSTEM_VARIABLE failed", exception=clex)
             return False
 
         return True
 
+    def clear_session(self) -> None:
+        """Clear the current session."""
+        self._session_id = None
+
     async def delete_system_variable(self, name: str) -> bool:
         """Delete a system variable from CCU / Homegear."""
         params = {SYSVAR_NAME: name}
         try:
             response = await self._post(
                 "SysVar.deleteSysVarByName",
                 params,
             )
 
             _LOGGER.debug("DELETE_SYSTEM_VARIABLE: Getting System variable")
             if json_result := response[P_RESULT]:
                 deleted = json_result
                 _LOGGER.debug("DELETE_SYSTEM_VARIABLE: Deleted: %s", str(deleted))
         except ClientException as clex:
-            self._handle_client_exception(method="DELETE_SYSTEM_VARIABLE", clex=clex)
+            self._handle_exception_log(method="DELETE_SYSTEM_VARIABLE", exception=clex)
             return False
 
         return True
 
     async def get_system_variable(self, name: str) -> Any:
         """Get single system variable from CCU / Homegear."""
         var = None
@@ -429,15 +459,15 @@
             if json_result := response[P_RESULT]:
                 # This does not yet support strings
                 try:
                     var = float(json_result)
                 except Exception:
                     var = json_result == "true"
         except ClientException as clex:
-            self._handle_client_exception(method="DELETE_SYSTEM_VARIABLE", clex=clex)
+            self._handle_exception_log(method="DELETE_SYSTEM_VARIABLE", exception=clex)
             return None
 
         return var
 
     async def get_all_system_variables(self, include_internal: bool) -> list[SystemVariableData]:
         """Get all system variables from CCU / Homegear."""
         variables: list[SystemVariableData] = []
@@ -488,19 +518,19 @@
                                 extended_sysvar=extended_sysvar,
                             )
                         )
                     except ValueError as verr:
                         _LOGGER.warning(
                             "GET_ALL_SYSTEM_VARIABLES failed: "
                             "ValueError [%s] Failed to parse SysVar %s ",
-                            verr.args,
+                            reduce_args(args=verr.args),
                             name,
                         )
         except ClientException as clex:
-            self._handle_client_exception(method="GET_ALL_SYSTEM_VARIABLES", clex=clex)
+            self._handle_exception_log(method="GET_ALL_SYSTEM_VARIABLES", exception=clex)
             return []
 
         return variables
 
     async def _get_system_variables_ext_markers(self) -> dict[str, Any]:
         """Get all system variables from CCU / Homegear."""
         ext_markers: dict[str, Any] = {}
@@ -530,15 +560,15 @@
                         channel_ids_room[room["id"]] = set()
                     channel_ids_room[room["id"]].add(room["name"])
                     for channel_id in room["channelIds"]:
                         if channel_id not in channel_ids_room:
                             channel_ids_room[channel_id] = set()
                         channel_ids_room[channel_id].add(room["name"])
         except ClientException as clex:
-            self._handle_client_exception(method="GET_ALL_CHANNEL_IDS_PER_ROOM", clex=clex)
+            self._handle_exception_log(method="GET_ALL_CHANNEL_IDS_PER_ROOM", exception=clex)
             return {}
 
         return channel_ids_room
 
     async def get_all_channel_ids_function(self) -> dict[str, set[str]]:
         """Get all channel_ids per function from CCU / Homegear."""
         channel_ids_function: dict[str, set[str]] = {}
@@ -555,15 +585,15 @@
                         channel_ids_function[function["id"]] = set()
                     channel_ids_function[function["id"]].add(function["name"])
                     for channel_id in function["channelIds"]:
                         if channel_id not in channel_ids_function:
                             channel_ids_function[channel_id] = set()
                         channel_ids_function[channel_id].add(function["name"])
         except ClientException as clex:
-            self._handle_client_exception(method="GET_ALL_CHANNEL_IDS_PER_FUNCTION", clex=clex)
+            self._handle_exception_log(method="GET_ALL_CHANNEL_IDS_PER_FUNCTION", exception=clex)
             return {}
 
         return channel_ids_function
 
     async def get_available_interfaces(self) -> list[str]:
         """Get all available interfaces from CCU / Homegear."""
         interfaces: list[str] = []
@@ -574,15 +604,15 @@
             )
 
             _LOGGER.debug("GET_AVAILABLE_INTERFACES: Getting all available interfaces")
             if json_result := response[P_RESULT]:
                 for interface in json_result:
                     interfaces.append(interface[ATTR_NAME])
         except ClientException as clex:
-            self._handle_client_exception(method="GET_AVAILABLE_INTERFACES", clex=clex)
+            self._handle_exception_log(method="GET_AVAILABLE_INTERFACES", exception=clex)
             return []
 
         return interfaces
 
     async def get_device_details(self) -> list[dict[str, Any]]:
         """Get the device details of the backend."""
         device_details: list[dict[str, Any]] = []
@@ -592,15 +622,15 @@
                 method="Device.listAllDetail",
             )
 
             _LOGGER.debug("GET_DEVICE_DETAILS: Getting the device details")
             if json_result := response[P_RESULT]:
                 device_details = json_result
         except ClientException as clex:
-            self._handle_client_exception(method="GET_DEVICE_DETAILS", clex=clex)
+            self._handle_exception_log(method="GET_DEVICE_DETAILS", exception=clex)
             return []
 
         return device_details
 
     async def get_all_device_data(self) -> dict[str, dict[str, dict[str, Any]]]:
         """Get the all device data of the backend."""
         all_device_data: dict[str, dict[str, dict[str, Any]]] = {}
@@ -608,15 +638,15 @@
         try:
             response = await self._post_script(script_name=REGA_SCRIPT_FETCH_ALL_DEVICE_DATA)
 
             _LOGGER.debug("GET_ALL_DEVICE_DATA: Getting all device data")
             if json_result := response[P_RESULT]:
                 all_device_data = _convert_to_values_cache(json_result)
         except ClientException as clex:
-            self._handle_client_exception(method="GET_ALL_DEVICE_DATA", clex=clex)
+            self._handle_exception_log(method="GET_ALL_DEVICE_DATA", exception=clex)
             return {}
 
         return all_device_data
 
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get the all programs of the backend."""
         all_programs: list[ProgramData] = []
@@ -643,15 +673,15 @@
                             name=name,
                             is_active=is_active,
                             is_internal=is_internal,
                             last_execute_time=last_execute_time,
                         )
                     )
         except ClientException as clex:
-            self._handle_client_exception(method="GET_ALL_PROGRAMS", clex=clex)
+            self._handle_exception_log(method="GET_ALL_PROGRAMS", exception=clex)
             return []
 
         return all_programs
 
     async def get_auth_enabled(self) -> bool | None:
         """Get the auth_enabled flag of the backend."""
         auth_enabled: bool | None = None
@@ -659,30 +689,30 @@
         try:
             response = await self._post(method="CCU.getAuthEnabled")
 
             _LOGGER.debug("GET_AUTH_ENABLED: Getting the flag auth_enabled")
             if (json_result := response[P_RESULT]) is not None:
                 auth_enabled = bool(json_result)
         except ClientException as clex:
-            self._handle_client_exception(method="GET_AUTH_ENABLED", clex=clex)
+            self._handle_exception_log(method="GET_AUTH_ENABLED", exception=clex)
             return None
         return auth_enabled
 
     async def get_https_redirect_enabled(self) -> bool | None:
         """Get the auth_enabled flag of the backend."""
         https_redirect_enabled: bool | None = None
 
         try:
             response = await self._post(method="CCU.getHttpsRedirectEnabled")
 
             _LOGGER.debug("GET_HTTPS_REDIRECT_ENABLED: Getting the flag https_redirect_enabled")
             if (json_result := response[P_RESULT]) is not None:
                 https_redirect_enabled = bool(json_result)
         except ClientException as clex:
-            self._handle_client_exception(method="GET_HTTPS_REDIRECT_ENABLED", clex=clex)
+            self._handle_exception_log(method="GET_HTTPS_REDIRECT_ENABLED", exception=clex)
             return None
 
         return https_redirect_enabled
 
     async def get_serial(self) -> str:
         """Get the serial of the backend."""
         serial = "unknown"
@@ -692,26 +722,30 @@
 
             _LOGGER.debug("GET_SERIAL: Getting the backend serial")
             if json_result := response[P_RESULT]:
                 serial = json_result["serial"]
                 if len(serial) > 10:
                     serial = serial[-10:]
         except ClientException as clex:
-            self._handle_client_exception(method="GET_SERIAL", clex=clex)
+            self._handle_exception_log(method="GET_SERIAL", exception=clex)
             return serial
 
         return serial
 
-    def _handle_client_exception(self, method: str, clex: ClientException) -> None:
-        """Handle ClientException."""
+    def _handle_exception_log(self, method: str, exception: BaseHomematicException) -> None:
+        """Handle BaseHomematicException and derivates logging."""
         if self._connection_state.json_issue:
-            _LOGGER.debug("%s failed: %s [%s]", method, clex.name, clex.args)
+            _LOGGER.debug(
+                "%s failed: %s [%s]", method, exception.name, reduce_args(args=exception.args)
+            )
         else:
             self._connection_state.add_issue(issuer=self)
-            _LOGGER.error("%s failed: %s [%s]", method, clex.name, clex.args)
+            _LOGGER.error(
+                "%s failed: %s [%s]", method, exception.name, reduce_args(args=exception.args)
+            )
 
 
 def _get_params(
     session_id: bool | str,
     extra_params: dict[str, Any] | None,
     use_default_params: bool,
 ) -> dict[str, Any]:
```

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/__init__.py` & `hahomematic-2023.8.2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/const.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/light.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/siren.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,24 +153,22 @@
         """Turn the device on."""
 
         acoustic_alarm = kwargs.get(
             _HM_ARG_ACOUSTIC_ALARM, self._e_acoustic_alarm_selection.default
         )
         if self.available_tones and acoustic_alarm and acoustic_alarm not in self.available_tones:
             raise ValueError(
-                f"Invalid tone specified "
-                f"for entity {self.full_name}: {acoustic_alarm}, "
+                f"Invalid tone specified for entity {self.full_name}: {acoustic_alarm}, "
                 "check the available_tones attribute for valid tones to pass in"
             )
 
         optical_alarm = kwargs.get(_HM_ARG_OPTICAL_ALARM, self._e_optical_alarm_selection.default)
         if self.available_lights and optical_alarm and optical_alarm not in self.available_lights:
             raise ValueError(
-                f"Invalid light specified "
-                f"for entity {self.full_name}: {optical_alarm}, "
+                f"Invalid light specified for entity {self.full_name}: {optical_alarm}, "
                 "check the available_lights attribute for valid tones to pass in"
             )
 
         await self._e_acoustic_alarm_selection.send_value(
             value=acoustic_alarm, collector=collector
         )
         await self._e_optical_alarm_selection.send_value(value=optical_alarm, collector=collector)
```

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/support.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.8.2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/device.py` & `hahomematic-2023.8.2/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/entity.py` & `hahomematic-2023.8.2/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/event.py` & `hahomematic-2023.8.2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/action.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/button.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/number.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/select.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.8.2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/button.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/number.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/select.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/hub/text.py` & `hahomematic-2023.8.2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/support.py` & `hahomematic-2023.8.2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/platforms/update.py` & `hahomematic-2023.8.2/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.8.2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.8.2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.8.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic/support.py` & `hahomematic-2023.8.2/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,19 @@
         vol.Required(ATTR_DATA): vol.Schema(
             {vol.Required(vol.Any(str)): vol.Schema(vol.Any(str, int, bool))}
         ),
     }
 )
 
 
+def reduce_args(args: tuple[Any, ...]) -> tuple[Any, ...] | Any:
+    """Return the first arg, if there is only one arg."""
+    return args[0] if len(args) == 1 else args
+
+
 def build_xml_rpc_uri(
     host: str,
     port: int,
     path: str | None,
     tls: bool = False,
 ) -> str:
     """Build XML-RPC API URL from components."""
@@ -78,20 +83,17 @@
     """Check / create directory."""
     if not directory:
         return False
     if not os.path.exists(directory):
         try:
             os.makedirs(directory)
         except OSError as ose:
-            _LOGGER.error(
-                "CHECK_OR_CREATE_DIRECTORY failed: Unable to create directory %s ('%s')",
-                directory,
-                ose.strerror,
-            )
-            raise HaHomematicException from ose
+            message = f"CHECK_OR_CREATE_DIRECTORY failed: Unable to create directory {directory} ('{ose.strerror}')"
+            _LOGGER.error(message)
+            raise HaHomematicException(message) from ose
 
     return True
 
 
 def parse_sys_var(data_type: str | None, raw_value: Any) -> Any:
     """Parse system variables to fix type."""
     # pylint: disable=no-else-return
```

### Comparing `hahomematic-2023.8.1/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.8.2/hahomematic/xml_rpc_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 from typing import Any, Final, TypeVar
 import xmlrpc.client
 
 from hahomematic import central_unit as hmcu
 from hahomematic.const import ATTR_TLS, ATTR_VERIFY_TLS
 from hahomematic.exceptions import AuthFailure, ClientException, NoConnection
-from hahomematic.support import get_tls_context
+from hahomematic.support import get_tls_context, reduce_args
 
 _LOGGER = logging.getLogger(__name__)
 _T = TypeVar("_T")
 
 ATTR_CONTEXT: Final = "context"
 ATTR_ENCODING_ISO_8859_1: Final = "ISO-8859-1"
 
@@ -94,34 +94,34 @@
                     self,
                     *args,
                 )
                 self._connection_state.remove_issue(issuer=self)
                 return result
             raise NoConnection(f"No connection to {self.interface_id}")
         except OSError as ose:
-            message = f"OSError on {self.interface_id}: {ose.args}"
+            message = f"OSError on {self.interface_id}: {reduce_args(args=ose.args)}"
             if ose.args[0] in NO_CONNECTION_ERROR_CODES:
                 if self._connection_state.add_issue(issuer=self):
                     _LOGGER.error(message)
                 else:
                     _LOGGER.debug(message)
             else:
                 _LOGGER.error(message)
             raise NoConnection(message) from ose
         except xmlrpc.client.Fault as fex:
-            raise ClientException(fex) from fex
+            raise ClientException(reduce_args(args=fex.args)) from fex
         except xmlrpc.client.ProtocolError as per:
             if not self._connection_state.has_issue(issuer=self):
                 if per.errmsg == "Unauthorized":
-                    raise AuthFailure(per) from per
-                raise NoConnection(per) from per
-        except NoConnection as noc:
-            raise noc
+                    raise AuthFailure(reduce_args(args=per.args)) from per
+                raise NoConnection(reduce_args(args=per.args)) from per
+        except NoConnection:
+            raise
         except Exception as ex:
-            raise ClientException(ex) from ex
+            raise ClientException(reduce_args(args=ex.args)) from ex
 
     def __getattr__(self, *args, **kwargs):  # type: ignore[no-untyped-def]
         """Magic method dispatcher."""
         return xmlrpc.client._Method(self.__async_request, *args, **kwargs)
 
     def stop(self) -> None:
         """Stop depending services."""
```

### Comparing `hahomematic-2023.8.1/hahomematic/xml_rpc_server.py` & `hahomematic-2023.8.2/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.8.2/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.8.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.8.2/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.1/pyproject.toml` & `hahomematic-2023.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.8.1"
+version     = "2023.8.2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

