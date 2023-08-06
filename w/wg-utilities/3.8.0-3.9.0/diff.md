# Comparing `tmp/wg_utilities-3.8.0.tar.gz` & `tmp/wg_utilities-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.8.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.9.0.tar", max compression
```

## Comparing `wg_utilities-3.8.0.tar` & `wg_utilities-3.9.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
--rw-r--r--   0        0        0     1069 2023-07-12 21:26:00.176983 wg_utilities-3.8.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-07-12 21:26:00.176983 wg_utilities-3.8.0/README.md
--rw-r--r--   0        0        0     4798 2023-07-12 21:26:00.180983 wg_utilities-3.8.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      685 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4207 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    23741 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56658 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7580 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13265 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    15915 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    27248 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    51568 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    22398 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7006 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5786 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 wg_utilities-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-02 14:37:28.502505 wg_utilities-3.9.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-08-02 14:37:28.502505 wg_utilities-3.9.0/README.md
+-rw-r--r--   0        0        0     4873 2023-08-02 14:37:28.502505 wg_utilities-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      749 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4255 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    23785 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56658 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7580 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13262 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0     9984 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/json_api_client.py
+-rw-r--r--   0        0        0    15946 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    18157 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    51568 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    22442 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7006 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5786 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0      565 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0     1982 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/file_handler.py
+-rw-r--r--   0        0        0     4486 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/list_handler.py
+-rw-r--r--   0        0        0     1060 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/stream_handler.py
+-rw-r--r--   0        0        0    11991 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/loggers/warehouse_handler.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-08-02 14:37:28.586508 wg_utilities-3.9.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 wg_utilities-3.9.0/PKG-INFO
```

### Comparing `wg_utilities-3.8.0/LICENSE` & `wg_utilities-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/README.md` & `wg_utilities-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/pyproject.toml` & `wg_utilities-3.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.8.0"
+version = "3.9.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
@@ -19,18 +19,18 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 async-upnp-client = { version = "*", optional = true }
 botocore = { version = "*", optional = true }
 flask = { version = ">=2.0.2", optional = true }
 "jetson.gpio" = { version = "*", platform = "linux", optional = true }
-lxml = { version = "==4.9.2", optional = true }
+lxml = { version = "==4.9.3", optional = true }
 pigpio = { version = "*", optional = true }
 pillow = { version = "*", optional = true }
-pyjwt = { version = ">=2.6,<2.8", optional = true }
+pyjwt = { version = ">=2.6,<2.9", optional = true }
 python-dotenv = { version = "*", optional = true }
 pytz = ">=2022.1"
 requests = { version = ">=2.26.0", optional = true }
 "rpi.gpio" = { version = "*", platform = "linux", optional = true }
 spidev = { version = "*", platform = "linux", optional = true }
 strenum = { version = "*", optional = true }
 tzlocal = { version = "*", optional = true }
@@ -129,14 +129,15 @@
 filterwarnings = [
     "ignore::DeprecationWarning:boto.*:",
     "ignore::DeprecationWarning:pkg_resources.*:",
 ]
 markers = [
     "mocked_operation_lookup: allows setting the mocks in the `mb3c` fixture",
     "upnp_value_path: file with content to set as the value in a `upnp_state_variable` fixture",
+    "add_handler: allows adding a custom handler to the `logger` fixture",
 ]
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "def __repr__", "def __str__", "@overload"]
 
 [tool.coverage.run]
 relative_files = true
```

### Comparing `wg_utilities-3.8.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.9.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.9.0/wg_utilities/clients/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 from __future__ import annotations
 
 from .google_calendar import GoogleCalendarClient
 from .google_drive import IMR, GoogleDriveClient, ItemMetadataRetrieval
 from .google_fit import GoogleFitClient
 from .google_photos import GooglePhotosClient
+from .json_api_client import JsonApiClient
 from .monzo import MonzoClient
 from .oauth_client import OAuthClient
 from .spotify import SpotifyClient
 from .truelayer import TrueLayerClient
 
 __all__ = [
     "GoogleCalendarClient",
     "GoogleDriveClient",
-    "ItemMetadataRetrieval",
-    "IMR",
     "GoogleFitClient",
     "GooglePhotosClient",
+    "ItemMetadataRetrieval",
+    "IMR",
+    "JsonApiClient",
     "MonzoClient",
     "OAuthClient",
     "SpotifyClient",
     "TrueLayerClient",
 ]
```

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/_google.py` & `wg_utilities-3.9.0/wg_utilities/clients/_google.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from copy import deepcopy
 from json import dumps
 from logging import DEBUG, getLogger
 from typing import TYPE_CHECKING, Any, Generic, Literal, TypeAlias, TypedDict, TypeVar
 
 from requests import Response, get
 
-from wg_utilities.clients.oauth_client import OAuthClient, StrBytIntFlt
+from wg_utilities.clients.json_api_client import StrBytIntFlt
+from wg_utilities.clients.oauth_client import OAuthClient
 from wg_utilities.loggers import add_stream_handler
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 add_stream_handler(LOGGER)
```

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.9.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.9.0/wg_utilities/clients/google_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from pydantic import Field, root_validator, validator
 from pytz import UTC, timezone
 from requests import delete
 from tzlocal import get_localzone
 
 from wg_utilities.clients._google import GoogleClient
+from wg_utilities.clients.json_api_client import StrBytIntFlt
 from wg_utilities.clients.oauth_client import (
     BaseModelWithConfig,
     GenericModelWithConfig,
-    StrBytIntFlt,
 )
 
 
 class ResponseStatus(str, Enum):
     """Enumeration for event attendee response statuses."""
 
     ACCEPTED = "accepted"
```

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.9.0/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.9.0/wg_utilities/clients/google_fit.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.9.0/wg_utilities/clients/google_photos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=too-few-public-methods,no-self-argument
 """Custom client for interacting with Google's Photos API."""
 from __future__ import annotations
 
 from datetime import datetime
-from enum import Enum, auto
+from enum import Enum
 from logging import DEBUG, getLogger
 from pathlib import Path
 from typing import Any, Literal, TypeAlias, TypedDict, TypeVar
 
 from pydantic import Field, validator
 from requests import post
 
@@ -63,15 +63,15 @@
 
 
 class MediaType(Enum):
     """Enum for all potential media types."""
 
     IMAGE = "image"
     VIDEO = "video"
-    UNKNOWN = auto()
+    UNKNOWN = "unknown"
 
 
 FJR = TypeVar("FJR", bound="GooglePhotosEntity")
 
 
 class GooglePhotosEntity(GenericModelWithConfig):
     """Base class for Google Photos entities."""
```

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.9.0/wg_utilities/clients/monzo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 from datetime import datetime, timedelta
 from logging import DEBUG, getLogger
 from typing import Any, Literal, TypedDict, final
 
 from pydantic import Field
 from requests import put
 
-from wg_utilities.clients.oauth_client import (
-    BaseModelWithConfig,
-    OAuthClient,
-    StrBytIntFlt,
-)
+from wg_utilities.clients.json_api_client import StrBytIntFlt
+from wg_utilities.clients.oauth_client import BaseModelWithConfig, OAuthClient
 from wg_utilities.functions import DTU, cleanse_string, utcnow
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 
 DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
```

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.9.0/wg_utilities/clients/oauth_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # pylint: disable=too-few-public-methods
 """Generic OAuth client to allow for reusable authentication flows/checks etc."""
 from __future__ import annotations
 
-from collections.abc import Callable, Iterable, Mapping
-from copy import deepcopy
+from collections.abc import Callable
 from datetime import datetime
-from http import HTTPStatus
-from json import JSONDecodeError, dumps
+from json import dumps
 from logging import DEBUG, getLogger
 from os import getenv
 from pathlib import Path
 from random import choice
 from string import ascii_letters
 from time import time
-from typing import Any, Generic, Literal, TypeAlias, TypeVar
+from typing import Any, Literal
 from urllib.parse import urlencode
 from webbrowser import open as open_browser
 
 from jwt import DecodeError, decode
 from pydantic import BaseModel, Extra, validate_model
 from pydantic.generics import GenericModel
-from requests import Response, get, post
 
 from wg_utilities.api import TempAuthServer
+from wg_utilities.clients.json_api_client import GetJsonResponse, JsonApiClient
 from wg_utilities.functions import user_data_dir
 from wg_utilities.functions.file_management import force_mkdir
-from wg_utilities.loggers import add_stream_handler
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
-add_stream_handler(LOGGER)
 
 
 class _ModelBase:
     """Base class for `BaseModelWithConfig` and `GenericModelWithConfig`.
 
     This is just to prevent duplicating the methods in both classes.
     """
@@ -204,38 +200,30 @@
 
         Returns:
             bool: True if the token is expired, False otherwise
         """
         return self.expiry_epoch < time()
 
 
-GetJsonResponse = TypeVar("GetJsonResponse", bound=Mapping[Any, Any])
-
-StrBytIntFlt: TypeAlias = str | bytes | int | float
-
-
-class OAuthClient(Generic[GetJsonResponse]):
+class OAuthClient(JsonApiClient[GetJsonResponse]):
     """Custom client for interacting with OAuth APIs.
 
     Includes all necessary/basic authentication functionality
     """
 
     ACCESS_TOKEN_ENDPOINT: str
     AUTH_LINK_BASE: str
-    BASE_URL: str
 
     ACCESS_TOKEN_EXPIRY_THRESHOLD = 150
 
     # Second env var added for compatibility
     DEFAULT_CACHE_DIR = getenv(
         "WG_UTILITIES_CACHE_DIR", getenv("WG_UTILITIES_CREDS_CACHE_DIR")
     )
-    DEFAULT_PARAMS: dict[
-        StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None
-    ] = {}
+
     DEFAULT_SCOPES: list[str] = []
 
     HEADLESS_MODE = getenv("WG_UTILITIES_HEADLESS_MODE", "0") == "1"
 
     def __init__(
         self,
         *,
@@ -248,305 +236,51 @@
         oauth_redirect_uri_override: str | None = None,
         headless_auth_link_callback: Callable[[str], None] | None = None,
         use_existing_credentials_only: bool = False,
         access_token_endpoint: str | None = None,
         auth_link_base: str | None = None,
         base_url: str | None = None,
     ):
+        super().__init__(log_requests=log_requests, base_url=base_url)
+
         self._client_id = client_id
         self._client_secret = client_secret
-        self.base_url = base_url or self.BASE_URL
         self.access_token_endpoint = access_token_endpoint or self.ACCESS_TOKEN_ENDPOINT
         self.auth_link_base = auth_link_base or self.AUTH_LINK_BASE
-        self.log_requests = log_requests
         self._creds_cache_path = creds_cache_path
         self.oauth_login_redirect_host = oauth_login_redirect_host
         self.oauth_redirect_uri_override = oauth_redirect_uri_override
         self.headless_auth_link_callback = headless_auth_link_callback
         self.use_existing_credentials_only = use_existing_credentials_only
 
         self.scopes = scopes or self.DEFAULT_SCOPES
 
         self._credentials: OAuthCredentials
         self._temp_auth_server: TempAuthServer
 
         if self._creds_cache_path:
             self._load_local_credentials()
 
-    def _get(
-        self,
-        url: str,
-        *,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
-        header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
-        json: Any | None = None,
-        data: Any | None = None,
-    ) -> Response:
-        """Wrap all GET requests to cover authentication, URL parsing, etc. etc.
-
-        Args:
-            url (str): the URL path to the endpoint (not necessarily including the
-                base URL)
-            params (dict): the parameters to be passed in the HTTP request
-            header_overrides (dict): any headers to override the default headers
-            timeout (float | tuple[float, float] | tuple[float, None] | None): the
-                timeout for the request
-            json (Any): the JSON to be passed in the HTTP request
-            data (Any): the data to be passed in the HTTP request
-
-        Returns:
-            Response: the response from the HTTP request
-        """
-        return self._request(
-            method=get,
-            url=url,
-            params=params,
-            header_overrides=header_overrides,
-            timeout=timeout,
-            json=json,
-            data=data,
-        )
-
     def _load_local_credentials(self) -> bool:
         """Load credentials from the local cache.
 
         Returns:
             bool: True if the credentials were loaded successfully, False otherwise
         """
         try:
             self._credentials = OAuthCredentials.parse_file(self.creds_cache_path)
         except FileNotFoundError:
             return False
 
         return True
 
-    def _post(
-        self,
-        url: str,
-        *,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
-        header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
-        json: Any | None = None,
-        data: Any | None = None,
-    ) -> Response:
-        """Wrap all POST requests to cover authentication, URL parsing, etc. etc.
-
-        Args:
-            url (str): the URL path to the endpoint (not necessarily including the
-                base URL)
-            json (dict): the data to be passed in the HTTP request
-            params (dict): the parameters to be passed in the HTTP request
-            header_overrides (dict): any headers to override the default headers
-            timeout (float | tuple[float, float] | tuple[float, None] | None): the
-                timeout for the request
-            json (Any): the JSON to be passed in the HTTP request
-            data (Any): the data to be passed in the HTTP request
-
-        Returns:
-            Response: the response from the HTTP request
-        """
-        return self._request(
-            method=post,
-            url=url,
-            params=params,
-            header_overrides=header_overrides,
-            timeout=timeout,
-            json=json,
-            data=data,
-        )
-
-    def _request(
-        self,
-        *,
-        method: Callable[..., Response],
-        url: str,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
-        header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
-        json: Any | None = None,
-        data: Any | None = None,
-    ) -> Response:
-        """Make a HTTP request.
-
-        Args:
-            method (Callable): the HTTP method to use
-            url (str): the URL path to the endpoint (not necessarily including the
-                base URL)
-            params (dict): the parameters to be passed in the HTTP request
-            header_overrides (dict): any headers to override the default headers
-            timeout (float | tuple[float, float] | tuple[float, None] | None): the
-                timeout for the request
-            json (dict): the data to be passed in the HTTP request
-            data (dict): the data to be passed in the HTTP request
-        """
-        if params is not None:
-            params.update(
-                {k: v for k, v in self.DEFAULT_PARAMS.items() if k not in params}
-            )
-        else:
-            params = deepcopy(self.DEFAULT_PARAMS)
-
-        params = {k: v for k, v in params.items() if v is not None}
-
-        if url.startswith("/"):
-            url = f"{self.base_url}{url}"
-
-        if self.log_requests:
-            LOGGER.debug(
-                "%s %s: %s", method.__name__.upper(), url, dumps(params, default=str)
-            )
-
-        res = method(
-            url,
-            headers=header_overrides
-            if header_overrides is not None
-            else self.request_headers,
-            params=params,
-            timeout=timeout,
-            json=json,
-            data=data,
-        )
-
-        res.raise_for_status()
-
-        return res
-
-    def _request_json_response(
-        self,
-        *,
-        method: Callable[..., Response],
-        url: str,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
-        header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
-        json: Any | None = None,
-        data: Any | None = None,
-    ) -> GetJsonResponse:
-        res = self._request(
-            method=method,
-            url=url,
-            params=params,
-            header_overrides=header_overrides,
-            timeout=timeout,
-            json=json,
-            data=data,
-        )
-        if res.status_code == HTTPStatus.NO_CONTENT:
-            return {}  # type: ignore[return-value]
-
-        try:
-            return res.json()  # type: ignore[no-any-return]
-        except JSONDecodeError as exc:
-            if not res.content:
-                return {}  # type: ignore[return-value]
-
-            raise ValueError(res.text) from exc
-
     def delete_creds_file(self) -> None:
         """Delete the local creds file."""
         self.creds_cache_path.unlink(missing_ok=True)
 
-    def get_json_response(
-        self,
-        url: str,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
-        header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: float | None = None,
-        json: Any | None = None,
-        data: Any | None = None,
-    ) -> GetJsonResponse:
-        """Get a simple JSON object from a URL.
-
-        Args:
-            url (str): the API endpoint to GET
-            params (dict): the parameters to be passed in the HTTP request
-            header_overrides (dict): headers to add to/overwrite the headers in
-                `self.request_headers`. Setting this to an empty dict will erase all
-                headers; `None` will use `self.request_headers`.
-            timeout (float): How many seconds to wait for the server to send data
-                before giving up
-            json (dict): a JSON payload to pass in the request
-            data (dict): a data payload to pass in the request
-
-        Returns:
-            dict: the JSON from the response
-        """
-
-        return self._request_json_response(
-            method=get,
-            url=url,
-            params=params,
-            header_overrides=header_overrides,
-            timeout=timeout,
-            json=json,
-            data=data,
-        )
-
-    def post_json_response(
-        self,
-        url: str,
-        params: dict[
-            StrBytIntFlt,
-            StrBytIntFlt | Iterable[StrBytIntFlt] | None,
-        ]
-        | None = None,
-        header_overrides: Mapping[str, str | bytes] | None = None,
-        timeout: (float | tuple[float, float] | tuple[float, None] | None) = None,
-        json: Any | None = None,
-        data: Any | None = None,
-    ) -> GetJsonResponse:
-        """Get a simple JSON object from a URL from a POST request.
-
-        Args:
-            url (str): the API endpoint to GET
-            params (dict): the parameters to be passed in the HTTP request
-            header_overrides (dict): headers to add to/overwrite the headers in
-                `self.request_headers`. Setting this to an empty dict will erase all
-                headers; `None` will use `self.request_headers`.
-            timeout (float): How many seconds to wait for the server to send data
-                before giving up
-            json (dict): a JSON payload to pass in the request
-            data (dict): a data payload to pass in the request
-
-        Returns:
-            dict: the JSON from the response
-        """
-
-        return self._request_json_response(
-            method=post,
-            url=url,
-            params=params,
-            header_overrides=header_overrides,
-            timeout=timeout,
-            json=json,
-            data=data,
-        )
-
     def refresh_access_token(self) -> None:
         """Refresh access token."""
 
         if not hasattr(self, "_credentials") and not self._load_local_credentials():
             # If we don't have any credentials, we can't refresh the access token -
             # perform first time login and leave it at that
             self.run_first_time_login()
```

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.9.0/wg_utilities/clients/spotify.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.9.0/wg_utilities/clients/truelayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from pathlib import Path
 from typing import Any, ClassVar, Literal, TypeAlias, TypedDict, TypeVar
 
 from pydantic import Field, validator
 from requests import HTTPError
 from strenum import StrEnum  # type: ignore[import]
 
+from wg_utilities.clients.json_api_client import StrBytIntFlt
 from wg_utilities.clients.oauth_client import (
     BaseModelWithConfig,
     GenericModelWithConfig,
     OAuthClient,
-    StrBytIntFlt,
 )
 from wg_utilities.functions import user_data_dir
 from wg_utilities.functions.file_management import force_mkdir
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
```

### Comparing `wg_utilities-3.8.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.9.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.9.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.9.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.9.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.9.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.9.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.9.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.9.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.9.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.9.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/json.py` & `wg_utilities-3.9.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/processes.py` & `wg_utilities-3.9.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.9.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/functions/xml.py` & `wg_utilities-3.9.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.9.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.8.0/PKG-INFO` & `wg_utilities-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.8.0
+Version: 3.9.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
@@ -19,19 +19,19 @@
 Provides-Extra: devices-yamaha-yas-209
 Provides-Extra: exceptions
 Provides-Extra: functions
 Requires-Dist: async-upnp-client ; extra == "devices-yamaha-yas-209"
 Requires-Dist: botocore
 Requires-Dist: flask (>=2.0.2) ; extra == "clients"
 Requires-Dist: jetson.gpio ; sys_platform == "linux"
-Requires-Dist: lxml (==4.9.2) ; extra == "functions"
+Requires-Dist: lxml (==4.9.3) ; extra == "functions"
 Requires-Dist: pigpio ; extra == "devices-dht22"
 Requires-Dist: pillow ; extra == "devices-epd"
 Requires-Dist: pydantic (<2.0.0) ; extra == "clients" or extra == "devices-yamaha-yas-209"
-Requires-Dist: pyjwt (>=2.6,<2.8) ; extra == "clients"
+Requires-Dist: pyjwt (>=2.6,<2.9) ; extra == "clients"
 Requires-Dist: python-dotenv ; extra == "clients" or extra == "exceptions"
 Requires-Dist: pytz (>=2022.1) ; extra == "clients"
 Requires-Dist: requests (>=2.26.0) ; extra == "clients" or extra == "exceptions"
 Requires-Dist: rpi.gpio ; (sys_platform == "linux") and (extra == "devices-epd")
 Requires-Dist: spidev ; (sys_platform == "linux") and (extra == "devices-epd")
 Requires-Dist: strenum ; extra == "clients"
 Requires-Dist: tzlocal ; extra == "clients"
```

