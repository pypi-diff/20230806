# Comparing `tmp/aiohomekit-2.6.8.tar.gz` & `tmp/aiohomekit-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohomekit-2.6.8.tar", max compression
+gzip compressed data, was "aiohomekit-2.6.9.tar", max compression
```

## Comparing `aiohomekit-2.6.8.tar` & `aiohomekit-2.6.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11537 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/LICENSE.md
--rw-r--r--   0        0        0     5841 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/README.md
--rw-r--r--   0        0        0     1867 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/__init__.py
--rw-r--r--   0        0        0    18826 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/__main__.py
--rw-r--r--   0        0        0     4465 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/characteristic_cache.py
--rw-r--r--   0        0        0     1162 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/const.py
--rw-r--r--   0        0        0      697 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/controller/__init__.py
--rw-r--r--   0        0        0    15761 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/controller/abstract.py
--rw-r--r--   0        0        0      704 2023-07-18 04:40:14.212068 aiohomekit-2.6.8/aiohomekit/controller/ble/__init__.py
--rw-r--r--   0        0        0     6832 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/bleak.py
--rw-r--r--   0        0        0     7819 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/client.py
--rw-r--r--   0        0        0     2017 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/connection.py
--rw-r--r--   0        0        0     1310 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/const.py
--rw-r--r--   0        0        0     7067 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/controller.py
--rw-r--r--   0        0        0     7614 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/discovery.py
--rw-r--r--   0        0        0     1894 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/key.py
--rw-r--r--   0        0        0     3747 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/manufacturer_data.py
--rw-r--r--   0        0        0    67891 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/pairing.py
--rw-r--r--   0        0        0    11736 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/structs.py
--rw-r--r--   0        0        0     2140 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ble/values.py
--rw-r--r--   0        0        0      708 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/__init__.py
--rw-r--r--   0        0        0    25692 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/connection.py
--rw-r--r--   0        0        0     1181 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/controller.py
--rw-r--r--   0        0        0     2422 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/discovery.py
--rw-r--r--   0        0        0     9972 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/pairing.py
--rw-r--r--   0        0        0     3431 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/pdu.py
--rw-r--r--   0        0        0    12547 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/coap/structs.py
--rw-r--r--   0        0        0     9288 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/controller.py
--rw-r--r--   0        0        0      757 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ip/__init__.py
--rw-r--r--   0        0        0    22146 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ip/connection.py
--rw-r--r--   0        0        0     1119 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ip/controller.py
--rw-r--r--   0        0        0     4108 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ip/discovery.py
--rw-r--r--   0        0        0    20914 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/controller/ip/pairing.py
--rw-r--r--   0        0        0      868 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/crypto/__init__.py
--rw-r--r--   0        0        0     4789 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/crypto/chacha20poly1305.py
--rw-r--r--   0        0        0     1036 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/crypto/hkdf.py
--rw-r--r--   0        0        0    10728 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/crypto/srp.py
--rw-r--r--   0        0        0     4060 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/debounce.py
--rw-r--r--   0        0        0      985 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/enum.py
--rw-r--r--   0        0        0     7746 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/exceptions.py
--rw-r--r--   0        0        0     2116 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/hkjson.py
--rw-r--r--   0        0        0     2044 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/http/__init__.py
--rw-r--r--   0        0        0     5265 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/http/response.py
--rw-r--r--   0        0        0     2608 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/meshcop.py
--rw-r--r--   0        0        0    12834 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/__init__.py
--rw-r--r--   0        0        0     1244 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/categories.py
--rw-r--r--   0        0        0     1892 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/__init__.py
--rw-r--r--   0        0        0    14169 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/characteristic.py
--rw-r--r--   0        0        0     1815 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/characteristic_formats.py
--rw-r--r--   0        0        0    22463 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/characteristic_types.py
--rw-r--r--   0        0        0     5238 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/const.py
--rw-r--r--   0        0        0    29366 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/data.py
--rw-r--r--   0        0        0      800 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/permissions.py
--rw-r--r--   0        0        0     4407 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/structs.py
--rw-r--r--   0        0        0      731 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/types.py
--rw-r--r--   0        0        0     1067 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/characteristics/units.py
--rw-r--r--   0        0        0     1439 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/entity_map.py
--rw-r--r--   0        0        0      722 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/feature_flags.py
--rw-r--r--   0        0        0      685 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/mixin.py
--rw-r--r--   0        0        0      796 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/services/__init__.py
--rw-r--r--   0        0        0    19993 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/services/data.py
--rw-r--r--   0        0        0     5019 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/services/service.py
--rw-r--r--   0        0        0     5380 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/services/service_types.py
--rw-r--r--   0        0        0      703 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/services/types.py
--rw-r--r--   0        0        0      716 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/model/status_flags.py
--rw-r--r--   0        0        0     4065 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/pdu.py
--rw-r--r--   0        0        0    20539 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/protocol/__init__.py
--rw-r--r--   0        0        0     3493 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/protocol/statuscodes.py
--rw-r--r--   0        0        0     8483 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/protocol/tlv.py
--rw-r--r--   0        0        0        0 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/py.typed
--rw-r--r--   0        0        0    12828 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/testing.py
--rw-r--r--   0        0        0     8265 2023-07-18 04:40:14.216068 aiohomekit-2.6.8/aiohomekit/tlv8.py
--rw-r--r--   0        0        0     3581 2023-07-18 04:40:14.220068 aiohomekit-2.6.8/aiohomekit/utils.py
--rw-r--r--   0        0        0     1662 2023-07-18 04:40:14.220068 aiohomekit-2.6.8/aiohomekit/uuid.py
--rw-r--r--   0        0        0    11606 2023-07-18 04:40:14.220068 aiohomekit-2.6.8/aiohomekit/zeroconf.py
--rw-r--r--   0        0        0     1809 2023-07-18 04:40:14.220068 aiohomekit-2.6.8/pyproject.toml
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11537 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/LICENSE.md
+-rw-r--r--   0        0        0     5841 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/README.md
+-rw-r--r--   0        0        0     1867 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/__init__.py
+-rw-r--r--   0        0        0    18826 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/__main__.py
+-rw-r--r--   0        0        0     4465 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/characteristic_cache.py
+-rw-r--r--   0        0        0     1162 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/const.py
+-rw-r--r--   0        0        0      697 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/__init__.py
+-rw-r--r--   0        0        0    15761 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/abstract.py
+-rw-r--r--   0        0        0      704 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/bleak.py
+-rw-r--r--   0        0        0     8802 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/client.py
+-rw-r--r--   0        0        0     2017 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/connection.py
+-rw-r--r--   0        0        0     1310 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/const.py
+-rw-r--r--   0        0        0     7067 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/controller.py
+-rw-r--r--   0        0        0     7743 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/discovery.py
+-rw-r--r--   0        0        0     1894 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/key.py
+-rw-r--r--   0        0        0     3747 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/manufacturer_data.py
+-rw-r--r--   0        0        0    67891 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/pairing.py
+-rw-r--r--   0        0        0    11736 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/structs.py
+-rw-r--r--   0        0        0     2140 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ble/values.py
+-rw-r--r--   0        0        0      708 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/__init__.py
+-rw-r--r--   0        0        0    25692 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/connection.py
+-rw-r--r--   0        0        0     1181 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/controller.py
+-rw-r--r--   0        0        0     2422 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/discovery.py
+-rw-r--r--   0        0        0     9972 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/pairing.py
+-rw-r--r--   0        0        0     3431 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/pdu.py
+-rw-r--r--   0        0        0    12547 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/coap/structs.py
+-rw-r--r--   0        0        0     9288 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/controller.py
+-rw-r--r--   0        0        0      757 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ip/__init__.py
+-rw-r--r--   0        0        0    22146 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ip/connection.py
+-rw-r--r--   0        0        0     1119 2023-07-20 15:12:16.155505 aiohomekit-2.6.9/aiohomekit/controller/ip/controller.py
+-rw-r--r--   0        0        0     4108 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/controller/ip/discovery.py
+-rw-r--r--   0        0        0    20914 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/controller/ip/pairing.py
+-rw-r--r--   0        0        0      868 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/crypto/__init__.py
+-rw-r--r--   0        0        0     4789 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/crypto/chacha20poly1305.py
+-rw-r--r--   0        0        0     1036 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/crypto/hkdf.py
+-rw-r--r--   0        0        0    10728 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/crypto/srp.py
+-rw-r--r--   0        0        0     4060 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/debounce.py
+-rw-r--r--   0        0        0      985 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/enum.py
+-rw-r--r--   0        0        0     7746 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/exceptions.py
+-rw-r--r--   0        0        0     2116 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/hkjson.py
+-rw-r--r--   0        0        0     2044 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/http/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/http/response.py
+-rw-r--r--   0        0        0     2608 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/meshcop.py
+-rw-r--r--   0        0        0    12834 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/__init__.py
+-rw-r--r--   0        0        0     1244 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/categories.py
+-rw-r--r--   0        0        0     1892 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/__init__.py
+-rw-r--r--   0        0        0    14169 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/characteristic.py
+-rw-r--r--   0        0        0     1815 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/characteristic_formats.py
+-rw-r--r--   0        0        0    22463 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/characteristic_types.py
+-rw-r--r--   0        0        0     5238 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/const.py
+-rw-r--r--   0        0        0    29366 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/data.py
+-rw-r--r--   0        0        0      800 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/permissions.py
+-rw-r--r--   0        0        0     4407 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/structs.py
+-rw-r--r--   0        0        0      731 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/types.py
+-rw-r--r--   0        0        0     1067 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/characteristics/units.py
+-rw-r--r--   0        0        0     1439 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/entity_map.py
+-rw-r--r--   0        0        0      722 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/feature_flags.py
+-rw-r--r--   0        0        0      685 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/mixin.py
+-rw-r--r--   0        0        0      796 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/services/__init__.py
+-rw-r--r--   0        0        0    19993 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/services/data.py
+-rw-r--r--   0        0        0     5019 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/services/service.py
+-rw-r--r--   0        0        0     5380 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/services/service_types.py
+-rw-r--r--   0        0        0      703 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/services/types.py
+-rw-r--r--   0        0        0      716 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/model/status_flags.py
+-rw-r--r--   0        0        0     4065 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/pdu.py
+-rw-r--r--   0        0        0    20539 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/protocol/__init__.py
+-rw-r--r--   0        0        0     3493 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/protocol/statuscodes.py
+-rw-r--r--   0        0        0     8483 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/protocol/tlv.py
+-rw-r--r--   0        0        0        0 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/py.typed
+-rw-r--r--   0        0        0    12828 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/testing.py
+-rw-r--r--   0        0        0     8265 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/tlv8.py
+-rw-r--r--   0        0        0     3581 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/utils.py
+-rw-r--r--   0        0        0     1662 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/uuid.py
+-rw-r--r--   0        0        0    11606 2023-07-20 15:12:16.159505 aiohomekit-2.6.9/aiohomekit/zeroconf.py
+-rw-r--r--   0        0        0     1809 2023-07-20 15:12:16.163505 aiohomekit-2.6.9/pyproject.toml
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.9/PKG-INFO
```

### Comparing `aiohomekit-2.6.8/LICENSE.md` & `aiohomekit-2.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/README.md` & `aiohomekit-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/__init__.py` & `aiohomekit-2.6.9/aiohomekit/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/__main__.py` & `aiohomekit-2.6.9/aiohomekit/__main__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/characteristic_cache.py` & `aiohomekit-2.6.9/aiohomekit/characteristic_cache.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/const.py` & `aiohomekit-2.6.9/aiohomekit/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/__init__.py` & `aiohomekit-2.6.9/aiohomekit/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/abstract.py` & `aiohomekit-2.6.9/aiohomekit/controller/abstract.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/__init__.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/bleak.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/bleak.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/client.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 from __future__ import annotations
 
 from collections.abc import Generator
 import logging
 import random
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, TypeVar, cast
 
 from bleak import BleakClient
 from bleak.backends.characteristic import BleakGATTCharacteristic
 
 from aiohomekit.controller.ble.key import DecryptionKey, EncryptionKey
 from aiohomekit.exceptions import EncryptionError
 from aiohomekit.model.services import ServicesTypes
@@ -31,15 +31,19 @@
     PDUStatus,
     decode_pdu,
     decode_pdu_continuation,
     encode_pdu,
 )
 from aiohomekit.protocol.tlv import TLV
 
-from .bleak import AIOHomeKitBleakClient
+from .bleak import (
+    AIOHomeKitBleakClient,
+    BleakCharacteristicMissing,
+    BleakServiceMissing,
+)
 from .const import AdditionalParameterTypes
 from .structs import BleRequest
 
 logger = logging.getLogger(__name__)
 
 WrapFuncType = TypeVar("WrapFuncType", bound=Callable[..., Any])
 
@@ -54,14 +58,40 @@
 
     def __init__(self, status: PDUStatus, message: str) -> None:
         """Initialize a PDUStatusError."""
         super().__init__(message)
         self.status = status
 
 
+def disconnect_on_missing_services(func: WrapFuncType) -> WrapFuncType:
+    """Define a wrapper to disconnect on missing services and characteristics.
+
+    This must be placed after the retry_bluetooth_connection_error
+    decorator.
+    """
+
+    async def _async_disconnect_on_missing_services_wrap(
+        self, *args: Any, **kwargs: Any
+    ) -> None:
+        try:
+            return await func(self, *args, **kwargs)
+        except (BleakServiceMissing, BleakCharacteristicMissing) as ex:
+            logger.warning(
+                "%s: Missing service or characteristic, disconnecting to force refetch of GATT services: %s",
+                self.name,
+                ex,
+            )
+            if self.client:
+                await self.client.clear_cache()
+                await self.client.disconnect()
+            raise
+
+    return cast(WrapFuncType, _async_disconnect_on_missing_services_wrap)
+
+
 async def ble_request(
     client: AIOHomeKitBleakClient,
     encryption_key: EncryptionKey | None,
     decryption_key: DecryptionKey | None,
     opcode: OpCode,
     handle: BleakGATTCharacteristic,
     iid: int,
```

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/connection.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/const.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/controller.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/discovery.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/discovery.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 from aiohomekit.controller.abstract import AbstractDiscovery, FinishPairing
 from aiohomekit.model import CharacteristicsTypes, ServicesTypes
 from aiohomekit.model.feature_flags import FeatureFlags
 from aiohomekit.protocol import perform_pair_setup_part1, perform_pair_setup_part2
 from aiohomekit.utils import check_pin_format, pair_with_auth
 
 from .bleak import AIOHomeKitBleakClient
-from .client import char_read, char_write, drive_pairing_state_machine
+from .client import (
+    char_read,
+    char_write,
+    disconnect_on_missing_services,
+    drive_pairing_state_machine,
+)
 from .connection import establish_connection
 from .manufacturer_data import HomeKitAdvertisement
 from .pairing import BlePairing
 
 if TYPE_CHECKING:
     from aiohomekit.controller.ble.controller import BleController
 
@@ -143,19 +148,21 @@
             CharacteristicsTypes.PAIR_SETUP,
             perform_pair_setup_part1(
                 with_auth=pair_with_auth(ff),
             ),
         )
 
     @retry_bluetooth_connection_error()
+    @disconnect_on_missing_services
     async def async_start_pairing(self, alias: str) -> FinishPairing:
         salt, pub_key = await self._async_start_pairing(alias)
         attempt = 0
 
         @retry_bluetooth_connection_error()
+        @disconnect_on_missing_services
         async def finish_pairing(pin: str) -> BlePairing:
             logger.debug("%s: finish pairing; rssi=%s", self.name, self.rssi)
 
             nonlocal attempt
             nonlocal salt
             nonlocal pub_key
```

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/key.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/key.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/manufacturer_data.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/manufacturer_data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/pairing.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/structs.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ble/values.py` & `aiohomekit-2.6.9/aiohomekit/controller/ble/values.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/__init__.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/connection.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/controller.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/discovery.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/pairing.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/pdu.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/coap/structs.py` & `aiohomekit-2.6.9/aiohomekit/controller/coap/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/controller.py` & `aiohomekit-2.6.9/aiohomekit/controller/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ip/__init__.py` & `aiohomekit-2.6.9/aiohomekit/controller/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ip/connection.py` & `aiohomekit-2.6.9/aiohomekit/controller/ip/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ip/controller.py` & `aiohomekit-2.6.9/aiohomekit/controller/ip/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ip/discovery.py` & `aiohomekit-2.6.9/aiohomekit/controller/ip/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/controller/ip/pairing.py` & `aiohomekit-2.6.9/aiohomekit/controller/ip/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/crypto/__init__.py` & `aiohomekit-2.6.9/aiohomekit/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/crypto/chacha20poly1305.py` & `aiohomekit-2.6.9/aiohomekit/crypto/chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/crypto/hkdf.py` & `aiohomekit-2.6.9/aiohomekit/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/crypto/srp.py` & `aiohomekit-2.6.9/aiohomekit/crypto/srp.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/debounce.py` & `aiohomekit-2.6.9/aiohomekit/debounce.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/enum.py` & `aiohomekit-2.6.9/aiohomekit/enum.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/exceptions.py` & `aiohomekit-2.6.9/aiohomekit/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/hkjson.py` & `aiohomekit-2.6.9/aiohomekit/hkjson.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/http/__init__.py` & `aiohomekit-2.6.9/aiohomekit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/http/response.py` & `aiohomekit-2.6.9/aiohomekit/http/response.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/meshcop.py` & `aiohomekit-2.6.9/aiohomekit/meshcop.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/__init__.py` & `aiohomekit-2.6.9/aiohomekit/model/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/categories.py` & `aiohomekit-2.6.9/aiohomekit/model/categories.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/__init__.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/characteristic.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/characteristic.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/characteristic_formats.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/characteristic_formats.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/characteristic_types.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/characteristic_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/const.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/data.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/permissions.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/permissions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/structs.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/types.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/characteristics/units.py` & `aiohomekit-2.6.9/aiohomekit/model/characteristics/units.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/entity_map.py` & `aiohomekit-2.6.9/aiohomekit/model/entity_map.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/feature_flags.py` & `aiohomekit-2.6.9/aiohomekit/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/mixin.py` & `aiohomekit-2.6.9/aiohomekit/model/mixin.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/services/__init__.py` & `aiohomekit-2.6.9/aiohomekit/model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/services/data.py` & `aiohomekit-2.6.9/aiohomekit/model/services/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/services/service.py` & `aiohomekit-2.6.9/aiohomekit/model/services/service.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/services/service_types.py` & `aiohomekit-2.6.9/aiohomekit/model/services/service_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/services/types.py` & `aiohomekit-2.6.9/aiohomekit/model/services/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/model/status_flags.py` & `aiohomekit-2.6.9/aiohomekit/model/status_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/pdu.py` & `aiohomekit-2.6.9/aiohomekit/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/protocol/__init__.py` & `aiohomekit-2.6.9/aiohomekit/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/protocol/statuscodes.py` & `aiohomekit-2.6.9/aiohomekit/protocol/statuscodes.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/protocol/tlv.py` & `aiohomekit-2.6.9/aiohomekit/protocol/tlv.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/testing.py` & `aiohomekit-2.6.9/aiohomekit/testing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/tlv8.py` & `aiohomekit-2.6.9/aiohomekit/tlv8.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/utils.py` & `aiohomekit-2.6.9/aiohomekit/utils.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/uuid.py` & `aiohomekit-2.6.9/aiohomekit/uuid.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/aiohomekit/zeroconf.py` & `aiohomekit-2.6.9/aiohomekit/zeroconf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.8/pyproject.toml` & `aiohomekit-2.6.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohomekit"
-version = "2.6.8"
+version = "2.6.9"
 description = "An asyncio HomeKit client"
 authors = ["John Carr <john.carr@unrouted.co.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Jc2k/aiohomekit"
 repository = "https://github.com/Jc2k/aiohomekit"
 keywords = ["HomeKit", "home", "automation"]
```

### Comparing `aiohomekit-2.6.8/PKG-INFO` & `aiohomekit-2.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohomekit
-Version: 2.6.8
+Version: 2.6.9
 Summary: An asyncio HomeKit client
 Home-page: https://github.com/Jc2k/aiohomekit
 License: Apache-2.0
 Keywords: HomeKit,home,automation
 Author: John Carr
 Author-email: john.carr@unrouted.co.uk
 Requires-Python: >=3.9,<4.0
```

