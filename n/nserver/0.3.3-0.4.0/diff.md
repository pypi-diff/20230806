# Comparing `tmp/nserver-0.3.3-py3-none-any.whl.zip` & `tmp/nserver-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 19972 bytes, number of entries: 14
--rw-r--r--  2.0 unx      180 b- defN 21-Feb-06 17:59 nserver/__init__.py
--rw-r--r--  2.0 unx     2032 b- defN 23-Apr-23 10:57 nserver/_version.py
+Zip file size: 21636 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      211 b- defN 23-Aug-06 06:03 nserver/__init__.py
+-rw-r--r--  2.0 unx     2032 b- defN 23-Aug-06 08:09 nserver/_version.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Aug-06 06:00 nserver/exceptions.py
 -rw-r--r--  2.0 unx     3275 b- defN 23-Apr-23 10:26 nserver/models.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-01 11:08 nserver/py.typed
 -rw-r--r--  2.0 unx     6362 b- defN 23-Apr-23 10:26 nserver/records.py
 -rw-r--r--  2.0 unx     5030 b- defN 21-Jul-17 15:59 nserver/rules.py
--rw-r--r--  2.0 unx    13760 b- defN 23-Apr-23 10:26 nserver/server.py
--rw-r--r--  2.0 unx    17989 b- defN 23-Apr-23 10:32 nserver/transport.py
--rw-r--r--  2.0 unx     1071 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/LICENCE
--rw-r--r--  2.0 unx     8029 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1067 b- defN 23-Apr-23 10:58 nserver-0.3.3.dist-info/RECORD
-14 files, 59115 bytes uncompressed, 18224 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    13855 b- defN 23-Aug-06 07:59 nserver/server.py
+-rw-r--r--  2.0 unx      898 b- defN 23-Aug-06 05:52 nserver/settings.py
+-rw-r--r--  2.0 unx    19398 b- defN 23-Aug-06 08:02 nserver/transport.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Aug-06 08:10 nserver-0.4.0.dist-info/LICENCE
+-rw-r--r--  2.0 unx     8020 b- defN 23-Aug-06 08:10 nserver-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      220 b- defN 23-Aug-06 08:10 nserver-0.4.0.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 08:10 nserver-0.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Aug-06 08:10 nserver-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1219 b- defN 23-Aug-06 08:10 nserver-0.4.0.dist-info/RECORD
+16 files, 62436 bytes uncompressed, 19656 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: nserver/__init__.py
 Comment: 
 
 Filename: nserver/_version.py
 Comment: 
 
+Filename: nserver/exceptions.py
+Comment: 
+
 Filename: nserver/models.py
 Comment: 
 
 Filename: nserver/py.typed
 Comment: 
 
 Filename: nserver/records.py
@@ -15,29 +18,32 @@
 
 Filename: nserver/rules.py
 Comment: 
 
 Filename: nserver/server.py
 Comment: 
 
+Filename: nserver/settings.py
+Comment: 
+
 Filename: nserver/transport.py
 Comment: 
 
-Filename: nserver-0.3.3.dist-info/LICENCE
+Filename: nserver-0.4.0.dist-info/LICENCE
 Comment: 
 
-Filename: nserver-0.3.3.dist-info/METADATA
+Filename: nserver-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: nserver-0.3.3.dist-info/NOTICE
+Filename: nserver-0.4.0.dist-info/NOTICE
 Comment: 
 
-Filename: nserver-0.3.3.dist-info/WHEEL
+Filename: nserver-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: nserver-0.3.3.dist-info/top_level.txt
+Filename: nserver-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nserver-0.3.3.dist-info/RECORD
+Filename: nserver-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nserver/__init__.py

```diff
@@ -1,4 +1,5 @@
-from .server import NameServer
 from .models import Query, Response
 from .rules import RegexRule, WildcardStringRule
 from .records import A, AAAA, NS, CNAME, PTR, SOA, MX, TXT, CAA
+from .server import NameServer
+from .settings import Settings
```

## nserver/_version.py

```diff
@@ -8,21 +8,21 @@
 ## Application
 
 ### CONSTANTS
 ### ============================================================================
 ## Version Information - DO NOT EDIT
 ## -----------------------------------------------------------------------------
 # These variables will be set during the build process. Do not attempt to edit.
-PACKAGE_VERSION = "0.3.3"
-BUILD_VERSION = "0.3.3"
-BUILD_GIT_HASH = "62bb4f9029e729045588e1545a8f0f2920905a86"
-BUILD_GIT_HASH_SHORT = "62bb4f9"
+PACKAGE_VERSION = "0.4.0"
+BUILD_VERSION = "0.4.0"
+BUILD_GIT_HASH = "16023e31cef9d194a2b3def96975425cc285305a"
+BUILD_GIT_HASH_SHORT = "16023e3"
 BUILD_GIT_BRANCH = "main"
-BUILD_TIMESTAMP = 1682247461
-BUILD_DATETIME = datetime.datetime.utcfromtimestamp(1682247461)
+BUILD_TIMESTAMP = 1691309381
+BUILD_DATETIME = datetime.datetime.utcfromtimestamp(1691309381)
 
 VERSION_VARS = vars()  # Don't have f-strings until py36
 
 ## Version Information Templates
 ## -----------------------------------------------------------------------------
 # You can customise the templates used for version information here.
 VERSION_INFO_TEMPLATE_SHORT = "{BUILD_VERSION}"
```

## nserver/server.py

```diff
@@ -1,32 +1,44 @@
 ### IMPORTS
 ### ============================================================================
 ## Standard Library
-from argparse import Namespace
 import logging
-from typing import List, Callable, Dict, Pattern
+
+# Note: Optional can only be replaced with `| None` in 3.10+
+from typing import List, Callable, Dict, Pattern, Optional, Type
 
 ## Installed
 import dnslib
 
 ## Application
-from .rules import RuleBase, WildcardStringRule, RegexRule
+from .exceptions import InvalidMessageError
 from .models import Query, Response
-from .transport import UDPv4Transport, TCPv4Transport, TransportBase, InvalidMessageError
 from .records import RecordBase
+from .rules import RuleBase, WildcardStringRule, RegexRule
+from .settings import Settings
+from .transport import TransportBase, UDPv4Transport, UDPv6Transport, TCPv4Transport
+
+
+### CONSTANTS
+### ============================================================================
+TRANSPORT_MAP: Dict[str, Type[TransportBase]] = {
+    "UDPv4": UDPv4Transport,
+    "UDPv6": UDPv6Transport,
+    "TCPv4": TCPv4Transport,
+}
 
 
-### NAME SERVER
+### Classes
 ### ============================================================================
 class NameServer:
     """NameServer for responding to requests."""
 
     # pylint: disable=too-many-instance-attributes
 
-    def __init__(self, name: str) -> None:
+    def __init__(self, name: str, settings: Optional[Settings] = None) -> None:
         """Initialise NameServer
 
         args:
             name: The name of the server. This is used for internal logging.
         """
         self.name = name
         self.rules: List[RuleBase] = []
@@ -34,25 +46,22 @@
             "before_first_query": [],
             "before_query": [],
             "after_query": [],
         }
         self._logger = logging.getLogger(f"nserver.i.{self.name}")
         self._before_first_query_run = False
 
-        self.settings = Namespace()
-        self.settings.SERVER_TYPE = "UDPv4"
-        self.settings.SERVER_ADDRESS = "localhost"
-        self.settings.SERVER_PORT = 9953
-        self.settings.DEBUG = False
-        self.settings.HEALTH_CHECK = False
-        self.settings.STATS = False
-        self.settings.REMOTE_ADMIN = False
-        self.settings.CONSOLE_LOG_LEVEL = logging.INFO
-        self.settings.FILE_LOG_LEVEL = logging.INFO
-        self.settings.MAX_ERRORS = 5
+        self.settings = settings if settings is not None else Settings()
+
+        transport = TRANSPORT_MAP.get(self.settings.server_transport)
+        if transport is None:
+            raise ValueError(
+                f"Invalid settings.server_transport {self.settings.server_transport!r}"
+            )
+        self.transport = transport(self.settings)
 
         self.shutdown_server = False
         self.exit_code = 0
         return
 
     def register_rule(self, rule: RuleBase) -> None:
         """Register the given rule."""
@@ -98,70 +107,64 @@
         self.hooks["after_query"].append(func)
         return
 
     def run(self) -> int:
         """Start running the server"""
         # Setup Logging
         console_logger = logging.StreamHandler()
-        console_logger.setLevel(self.settings.CONSOLE_LOG_LEVEL)
+        console_logger.setLevel(self.settings.console_log_level)
 
         console_formatter = logging.Formatter(
             "[{asctime}][{levelname}][{name}] {message}", style="{"
         )
 
         console_logger.setFormatter(console_formatter)
 
         self._logger.addHandler(console_logger)
-        self._logger.setLevel(min(self.settings.CONSOLE_LOG_LEVEL, self.settings.FILE_LOG_LEVEL))
+        self._logger.setLevel(min(self.settings.console_log_level, self.settings.file_log_level))
 
         # Start Server
-        server_type = self.settings.SERVER_TYPE
-        server: TransportBase
-
-        if server_type == "TCPv4":
-            server = TCPv4Transport(self.settings.SERVER_ADDRESS, self.settings.SERVER_PORT)
-        elif server_type == "UDPv4":
-            server = UDPv4Transport(self.settings.SERVER_ADDRESS, self.settings.SERVER_PORT)
-        else:
-            raise ValueError(f"Unknown SERVER_TYPE: {server_type}")
+        # TODO: Do we want to recreate the transport instance or do we assume that
+        # transport.shutdown_server puts it back into a ready state?
+        # We could make this configurable? :thonking:
 
-        self._info(f"Starting {server}")
+        self._info(f"Starting {self.transport}")
         try:
-            server.start_server()
+            self.transport.start_server()
         except Exception as e:  # pylint: disable=broad-except
             self._critical(e)
             self.exit_code = 1
             return self.exit_code
 
-        error_count = 0
         # Process Requests
+        error_count = 0
         while True:
             if self.shutdown_server:
                 break
             try:
-                message = server.receive_message()
+                message = self.transport.receive_message()
                 response = self._process_dns_record(message.message)
                 message.response = response
-                server.send_message_response(message)
+                self.transport.send_message_response(message)
             except InvalidMessageError as e:
                 self._warning(f"{e}")
             except Exception as e:  # pylint: disable=broad-except
                 self._error(f"Uncaught error occured. {e}", exc_info=True)
                 error_count += 1
-                if error_count >= self.settings.MAX_ERRORS:
+                if error_count >= self.settings.max_errors:
                     self._critical(f"Max errors hit ({error_count})")
                     self.shutdown_server = True
                     self.exit_code = 1
             except KeyboardInterrupt:
                 self._info("KeyboardInterrupt received.")
                 self.shutdown_server = True
 
         # Stop Server
         self._info("Shutting down server")
-        server.stop_server()
+        self.transport.stop_server()
 
         # Teardown Logging
         self._logger.removeHandler(console_logger)
         return self.exit_code
 
     ## Decorators
     ## -------------------------------------------------------------------------
```

## nserver/transport.py

```diff
@@ -1,29 +1,32 @@
 ### IMPORTS
 ### ============================================================================
 ## Standard Library
-import base64
 from collections import deque
 from dataclasses import dataclass
-from enum import IntEnum
+import enum
 import selectors
 import socket
 import struct
 import time
-from typing import Tuple, Optional, Dict, List, Deque, NewType, cast
+
+# Note: Union can only be replaced with `X | Y` in 3.10+
+from typing import Tuple, Optional, Dict, List, Deque, NewType, Any, Union, cast
 
 ## Installed
 import dnslib
 
 ## Application
+from .exceptions import InvalidMessageError
+from .settings import Settings
 
 
 ### CONSTANTS
 ### ============================================================================
-class TcpState(IntEnum):
+class TcpState(enum.IntEnum):
     """State of a TCP connection.
 
     General usage:
     `TcpState(get_tcp_info(connection)[0])`
     """
 
     TCP_ESTABLISHED = 1
@@ -60,79 +63,90 @@
     "Get the TcpState of a socket"
     return TcpState(get_tcp_info(connection)[0])
 
 
 def recv_data(
     data_length: int, connection: socket.socket, existing_data: bytes = b"", timeout: int = 10
 ) -> bytes:
-    """Receive data a given amount of data from a socket."""
+    """Receive a given amount of data from a socket."""
     data = bytes(existing_data)
     data_remaining = data_length - len(data)
     start_time = time.time()
     while data_remaining > 0:
         data += connection.recv(data_remaining)
         data_remaining = data_length - len(data)
         if data_remaining and time.time() - start_time > timeout:
-            msg = f"timeout reading data from {connection.getpeername()}"
-            raise TimeoutError(msg)
+            raise TimeoutError(f"timeout reading data from {connection.getpeername()}")
     return data
 
 
 ### CLASSES
 ### ============================================================================
 class MessageContainer:  # pylint: disable=too-few-public-methods
-    """Class for holding DNS messages and the socket they originated from.
+    """Class for holding DNS messages and the transport they originated from.
 
     Used to simplify the interface (and allow for threading etc later).
     """
 
-    SOCKET_TYPES = {"UDPv4", "TCPv4"}
-
     def __init__(
         self,
         raw_data: bytes,
-        socket_: Optional[socket.socket],
-        socket_type: str,
-        remote_address: Tuple[str, int],
+        transport: "TransportBase",
+        transport_data: Any,
+        remote_client: Union[str, Tuple[str, int]],
     ):
-        if socket_type not in self.SOCKET_TYPES:
-            raise ValueError(f"Unkown socket_type {socket_type!r}")
+        """Create new message container
 
+        `raw_data` is the raw message pulled from the transport. It will parsed
+        as a DNS message.
+        `transport` is the transport instance that created this message (e.g. `self`).
+        Messages must only be returned to this transport instance when responding (even
+        if it would be possible for another instance to respond (e.g. with UDP processing)).
+        As such transports should rely on only receiving messages that they created
+        (opposed to `assert message.transport is self`).
+        `transport_data` is data that the transport instance wishes to store with
+        this message for later use. What is stored is up to the transport, and it is
+        up to the transport implementation to correctly handle it.
+        `remote_client` is a representation of the remote client that sent this DNS
+        request. This value is primarily to allow logging and debugging of invalid
+        requests. Whilst transport instances must set this value, they should not
+        use it for processing.
+        """
+        # Note: We used to have checks on the validity of the input arguments.
+        # However as this function is internal to this package and this package
+        # is now mature enough to have unit tests, linters, and type checkers,
+        # then we /should/ always have the correct values.
         try:
             self.message = dnslib.DNSRecord.parse(raw_data)
         except dnslib.dns.DNSError as e:
-            raise InvalidMessageError(e, raw_data, remote_address) from e
-        self.socket = socket_
-        self.socket_type = socket_type
-        self.remote_address = remote_address
+            raise InvalidMessageError(e, raw_data, remote_client) from e
+
+        self.transport = transport
+        self.transport_data = transport_data
+        self.remote_client = remote_client
         self.response: Optional[dnslib.DNSRecord] = None
         return
 
     def get_response_bytes(self):
         """Convert response object to bytes"""
         if self.response is None:
-            raise RuntimeError("response not set!")
+            raise AttributeError("response not set!")
         return self.response.pack()
 
 
-class InvalidMessageError(ValueError):
-    """Class for holding invalid messages."""
-
-    def __init__(self, error: Exception, raw_data: bytes, remote_address: Tuple[str, int]):
-        encoded_data = base64.b64encode(raw_data).decode("ascii")
-        message = f"{error} Remote: {remote_address} Bytes: {encoded_data}"
-        super().__init__(message)
-        return
-
-
 ## Transport Classes
 ## -----------------------------------------------------------------------------
 class TransportBase:
     """Base class for all transports"""
 
+    def __init__(self, settings: Settings) -> None:
+        self.settings = settings
+        # TODO: setup logging
+        return
+
     def start_server(self, timeout=60) -> None:
         """Start transport's server"""
         raise NotImplementedError()
 
     def stop_server(self) -> None:
         """Stop transport's server"""
         raise NotImplementedError()
@@ -142,23 +156,33 @@
         raise NotImplementedError()
 
     def send_message_response(self, message: MessageContainer) -> None:
         """Respond to a message that was received by the server"""
         raise NotImplementedError()
 
 
+# UDP Transports
+# ..............................................................................
+@dataclass
+class UDPMessageData:
+    """Message.transport_data for UDP transports"""
+
+    remote_address: Tuple[str, int]
+
+
 class UDPv4Transport(TransportBase):
     """Transport class for IPv4 UDP."""
 
-    SOCKET_TYPE = "UDPv4"
+    _SOCKET_AF = socket.AF_INET
 
-    def __init__(self, address: str, port: int):
-        self.address = address
-        self.port = port
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    def __init__(self, settings: Settings):
+        super().__init__(settings)
+        self.address = self.settings.server_address
+        self.port = self.settings.server_port
+        self.socket = socket.socket(self._SOCKET_AF, socket.SOCK_DGRAM)
         return
 
     def start_server(self, timeout=60) -> None:
         start_time = time.time()
         while (time.time() - start_time) < timeout:
             try:
                 self.socket.bind((self.address, self.port))
@@ -171,35 +195,46 @@
                 raise e
         else:
             raise RuntimeError(f"Failed to bind server after {timeout} seconds")
         return
 
     def receive_message(self) -> MessageContainer:
         data, remote_address = self.socket.recvfrom(512)
-        message = MessageContainer(data, None, self.SOCKET_TYPE, remote_address)
+        message = MessageContainer(data, self, UDPMessageData(remote_address), remote_address)
         return message
 
     def send_message_response(self, message: MessageContainer) -> None:
-        if message.socket_type != self.SOCKET_TYPE:
-            raise RuntimeError(f"Invalid socket_type: {message.socket_type} != {self.SOCKET_TYPE}")
         data = message.get_response_bytes()
-        self.socket.sendto(data, message.remote_address)
+        self.socket.sendto(data, message.transport_data.remote_address)
         return
 
     def stop_server(self) -> None:
         self.socket.close()
         return
 
     def __repr__(self):
         return f"{self.__class__.__name__}(address={self.address!r}, port={self.port!r})"
 
 
-# TCPv4 Server
+class UDPv6Transport(UDPv4Transport):
+    """Transport class for IPv6 UDP."""
+
+    _SOCKET_AF = socket.AF_INET6
+
+
+# TCP Transport
 # ..............................................................................
 @dataclass
+class TCPMessageData:
+    """Message.transport_data for TCP transports"""
+
+    socket: socket.socket
+
+
+@dataclass
 class CachedConnection:
     "Dataclass for storing information about a TCP connection"
     connection: socket.socket
     remote_address: Tuple[str, int]
     last_data_time: float
     selector_key: selectors.SelectorKey
     cache_key: CacheKey
@@ -210,25 +245,25 @@
 
     References:
         - https://tools.ietf.org/html/rfc7766#section-8
     """
 
     # pylint: disable=too-many-instance-attributes
 
-    SOCKET_TYPE = "TCPv4"
     SELECT_TIMEOUT = 0.1
     CONNECTION_KEEPALIVE_LIMIT = 30  # seconds
     CONNECTION_CACHE_LIMIT = 200
     CONNECTION_CACHE_VACUUM_PERCENT = 0.9
     CONNECTION_CACHE_TARGET = int(CONNECTION_CACHE_LIMIT * CONNECTION_CACHE_VACUUM_PERCENT)
     CONNECTION_CACHE_CLEAN_INTERVAL = 10  # seconds
 
-    def __init__(self, address: str, port: int) -> None:
-        self.address = address
-        self.port = port
+    def __init__(self, settings: Settings) -> None:
+        super().__init__(settings)
+        self.address = self.settings.server_address
+        self.port = self.settings.server_port
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.socket.setblocking(False)
         # Allow taking over of socket when in TIME_WAIT (i.e. previously released)
         self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
         self.selector = selectors.DefaultSelector()
         self.cached_connections: Dict[CacheKey, CachedConnection] = {}
@@ -259,27 +294,25 @@
     def receive_message(self) -> MessageContainer:
         connection, remote_address = self._get_next_connection()
         packed_length = recv_data(2, connection)
 
         data_length = struct.unpack("!H", packed_length)[0]
         data = recv_data(data_length, connection)
 
-        return MessageContainer(data, connection, self.SOCKET_TYPE, remote_address)
+        return MessageContainer(data, self, TCPMessageData(connection), remote_address)
 
     def send_message_response(self, message: MessageContainer) -> None:
-        if message.socket_type != self.SOCKET_TYPE or message.socket is None:
-            raise RuntimeError(f"Invalid socket_type: {message.socket_type} != {self.SOCKET_TYPE}")
         data = message.get_response_bytes()
         encoded_length = struct.pack("!H", len(data))
         try:
-            message.socket.sendall(encoded_length + data)
+            message.transport_data.socket.sendall(encoded_length + data)
         except BrokenPipeError:
             # Remote closed connection
             # Drop response per https://datatracker.ietf.org/doc/html/rfc7766#section-6.2.4
-            self._remove_connection(message.socket)
+            self._remove_connection(message.transport_data.socket)
 
         # Note that we don't close the socket here in order to allow TCP request streaming
         # print(f"Sent response to {self._get_cache_key(message.socket)} {message.remote_address}")
         return
 
     def stop_server(self) -> None:
         # Stop listening
```

## Comparing `nserver-0.3.3.dist-info/LICENCE` & `nserver-0.4.0.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `nserver-0.3.3.dist-info/METADATA` & `nserver-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nserver
-Version: 0.3.3
+Version: 0.4.0
 Summary: DNS Name Server Framework
 Author-email: Nicholas Hairs <info+nserver@nicholashairs.com>
 License: MIT License
         
         Copyright (c) 2020 Nicholas Hairs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,27 +46,27 @@
 Requires-Dist: setuptools ; extra == 'dev'
 Requires-Dist: wheel ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: mkdocs ; extra == 'dev'
-Requires-Dist: mkdocs-material (>=8.5) ; extra == 'dev'
+Requires-Dist: mkdocs-material >=8.5 ; extra == 'dev'
 Requires-Dist: mkdocs-awesome-pages-plugin ; extra == 'dev'
 Requires-Dist: mdx-truly-sane-lists ; extra == 'dev'
 Requires-Dist: bpython ; extra == 'dev'
 
 # NServer: a high-level Python DNS Name Server Framework.
 
 [![PyPi](https://img.shields.io/pypi/v/nserver.svg)](https://pypi.python.org/pypi/nserver/)
 [![PyPI - Status](https://img.shields.io/pypi/status/nserver)](https://pypi.python.org/pypi/nserver/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/nserver.svg)](https://github.com/nhairs/nserver)
 [![License](https://img.shields.io/github/license/nhairs/nserver.svg)](https://github.com/nhairs/nserver)
 
-NServer is a Python (3.6+) framework for building customised DNS name servers with a focuses on ease of use over completeness. It implements high level APIs for interacting with DNS queries whilst making very few assumptions about how responses are generated.
+NServer is a Python framework for building customised DNS name servers with a focuses on ease of use over completeness. It implements high level APIs for interacting with DNS queries whilst making very few assumptions about how responses are generated.
 
 It is not intended to act like traditional DNS servers such as [BIND](https://www.isc.org/bind/) or [CoreDNS](https://github.com/coredns/coredns) and should not be considered a general DNS resolver.
 
 NServer has been built upon [dnslib](https://github.com/paulc/dnslib) however uses high level abstractions that does not give access to the full DNS specification. If this is your desired behaviour I suggest using dnslib and its [server API](https://github.com/paulc/dnslib/blob/master/dnslib/server.py).
 
 NServer has been inspired by easy to use high level frameworks such as [Flask](https://github.com/pallets/flask) or [Requests](https://github.com/psf/requests).
```

## Comparing `nserver-0.3.3.dist-info/RECORD` & `nserver-0.4.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-nserver/__init__.py,sha256=MajwZ4WrYaWvsA8_lrOFWgZnsAJ-lpdG3BsmDlDA4NU,180
-nserver/_version.py,sha256=vRb8BYhmHsSGPl9aZIkth1iDd7tvhRCTE7o1ybtrTLI,2032
+nserver/__init__.py,sha256=4GwiWL-3-DUYUGKz1puty5e4HxESgvQTJgq--oKHYMw,211
+nserver/_version.py,sha256=S08cwb4qNCdLkDqbqpLmPqfZuAGFNhcQsa40gQHn4Gc,2032
+nserver/exceptions.py,sha256=1BqOl31BUtZQ4eN3U6_k8Qssp4I0Tez4VLGsjjyYkgs,745
 nserver/models.py,sha256=acuUUF_I_mH8H7e8gGzKTsRnU0RE68e8lzIuTG2K7dw,3275
 nserver/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nserver/records.py,sha256=ZZY-_vN-1B0gcyohHTdhtkGqebemEmdVK6vAHVOzXeM,6362
 nserver/rules.py,sha256=j6XbD8kVcfiAtzbkNWlKpsm45Gc22WYVa8HLGfhpL_w,5030
-nserver/server.py,sha256=wFP14f44wenIrBZ4LaS4dHDzwWCW7v4p626MsSgvgwg,13760
-nserver/transport.py,sha256=YrP5BeZ2yWVULdKh-MwFpHD4ndnywa6fgZk7xkUBxKg,17989
-nserver-0.3.3.dist-info/LICENCE,sha256=W1bDNCHGJddUmYNElLUEbbOlBPQmFISUR8uja44sOWs,1071
-nserver-0.3.3.dist-info/METADATA,sha256=gRB1tvosJop9Wcho-3NMbGd3j9Yy-WBJYrPpXs7yV_M,8029
-nserver-0.3.3.dist-info/NOTICE,sha256=Qq6ErnuPr87l7y6-8UDasbfi5d7AWFHnWmz1-1N5b2M,220
-nserver-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nserver-0.3.3.dist-info/top_level.txt,sha256=C11DUdis7SN6wOzDVcD08kmX7CQMRY03bxhZaEYX8ZQ,8
-nserver-0.3.3.dist-info/RECORD,,
+nserver/server.py,sha256=NkDhYcezj2W3jOZIiYzvLm8ZjwnroUvpeJGJtT-dVI8,13855
+nserver/settings.py,sha256=meeZ8BJG_PqtA5pdnQdQGSlP-eR7UfEsysvsXAWGvVM,898
+nserver/transport.py,sha256=hT4lTdpAwyZqqQ1J1ToCNQBd1Wl8ljYtBVcgS8YXvwE,19398
+nserver-0.4.0.dist-info/LICENCE,sha256=W1bDNCHGJddUmYNElLUEbbOlBPQmFISUR8uja44sOWs,1071
+nserver-0.4.0.dist-info/METADATA,sha256=ILW5RbwvRNb7SbE2_9oYiEsCjTcDX8a5GemuNEAMbGQ,8020
+nserver-0.4.0.dist-info/NOTICE,sha256=Qq6ErnuPr87l7y6-8UDasbfi5d7AWFHnWmz1-1N5b2M,220
+nserver-0.4.0.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+nserver-0.4.0.dist-info/top_level.txt,sha256=C11DUdis7SN6wOzDVcD08kmX7CQMRY03bxhZaEYX8ZQ,8
+nserver-0.4.0.dist-info/RECORD,,
```

