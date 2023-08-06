# Comparing `tmp/curl_cffi-0.5.7.tar.gz` & `tmp/curl_cffi-0.5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_cffi-0.5.7.tar", last modified: Tue Jul  4 10:50:13 2023, max compression
+gzip compressed data, was "curl_cffi-0.5.8.1.tar", last modified: Sun Aug  6 15:24:25 2023, max compression
```

## Comparing `curl_cffi-0.5.7.tar` & `curl_cffi-0.5.8.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12654 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/curl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/ffi/cdef.c
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/ffi/shim.c
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/ffi/shim.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18640 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/curl_cffi/requests/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/curl_cffi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 10:50:13.000000 curl_cffi-0.5.7/curl_cffi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:50:13.530351 curl_cffi-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 10:50:00.000000 curl_cffi-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:24:25.950080 curl_cffi-0.5.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-08-06 15:24:25.950080 curl_cffi-0.5.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:24:25.946080 curl_cffi-0.5.8.1/curl_cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/curl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:24:25.946080 curl_cffi-0.5.8.1/curl_cffi/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/ffi/cdef.c
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/ffi/shim.c
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/ffi/shim.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:24:25.950080 curl_cffi-0.5.8.1/curl_cffi/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/requests/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/requests/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27928 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/curl_cffi/requests/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:24:25.946080 curl_cffi-0.5.8.1/curl_cffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-08-06 15:24:25.000000 curl_cffi-0.5.8.1/curl_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-06 15:24:25.000000 curl_cffi-0.5.8.1/curl_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:24:25.000000 curl_cffi-0.5.8.1/curl_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-06 15:24:25.000000 curl_cffi-0.5.8.1/curl_cffi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 15:24:25.000000 curl_cffi-0.5.8.1/curl_cffi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 15:24:25.950080 curl_cffi-0.5.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 15:24:16.000000 curl_cffi-0.5.8.1/setup.py
```

### Comparing `curl_cffi-0.5.7/LICENSE` & `curl_cffi-0.5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.7/README.md` & `curl_cffi-0.5.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,101 @@
+Metadata-Version: 2.1
+Name: curl_cffi
+Version: 0.5.8.1
+Summary: libcurl ffi bindings for Python, with impersonation support
+Author-email: Yifei Kong <kong@yifei.me>
+License: MIT License
+        
+        Copyright (c) 2018 multippt
+        Copyright (c) 2022 Yifei Kong
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/yifeikong/curl_cffi
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: build
+Provides-Extra: test
+License-File: LICENSE
+
 # curl_cffi
 
 Python binding for [curl-impersonate](https://github.com/lwthiker/curl-impersonate)
-via [CFFI](https://cffi.readthedocs.io/en/latest/).
+via [cffi](https://cffi.readthedocs.io/en/latest/).
 
-[中文文档](README-zh.md)
+[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/master/README-zh.md)
 
-Unlike other pure python http clients like `httpx` or `requests`, this package can
+Unlike other pure python http clients like `httpx` or `requests`, `curl_cffi` can
 impersonate browsers' TLS signatures or JA3 fingerprints. If you are blocked by some
 website for no obvious reason, you can give this package a try.
 
-## Note on Chrome 110+ JA3 fingerprints
-
-Chrome introduces ClientHello permutation in version 110, which means the order of
-extensions will be random, thus JA3 fingerprints will be random. So, when comparing
-JA3 fingerprints of `curl_cffi` and a browser, they may differ. However, this does not
-mean that TLS fingerprints will not be a problem, ClientHello extension order is just
-one factor of how servers can tell automated requests from browsers.
+## Features
 
-See more from [this article](https://www.fastly.com/blog/a-first-look-at-chromes-tls-clienthello-permutation-in-the-wild)
-and [curl-impersonate notes](https://github.com/lwthiker/curl-impersonate/pull/148)
+- Supports JA3/TLS and http2 fingerprints impersonation.
+- Much faster than requests/httpx/tls_client, on par with aiohttp/pycurl, see [benchmarks](https://github.com/yifeikong/curl_cffi/tree/master/benchmark).
+- Mimics requests API, no need to learn another one.
+- Pre-compiled, so you don't have to compile on your machine.
+- Supports `asyncio` with proxy rotation on each request.
+- Supports http 2.0, which requests does not.
 
 ## Install
 
-    pip install --upgrade curl_cffi
+    pip install curl_cffi --upgrade
 
-This should work for Linux(x86_64/aarch64), macOS(Intel/Apple Silicon), Windows(amd64).
-If it does not work, you may need to compile and install `curl-impersonate` first.
+This should work on Linux(x86_64/aarch64), macOS(Intel/Apple Silicon) and Windows(amd64).
+If it does not work on you platform, you may need to compile and install `curl-impersonate`
+first and set some environment variables like `LD_LIBRARY_PATH`.
 
 ## Usage
 
-`requests/httpx`-like API:
+### requests-like
 
 ```python
 from curl_cffi import requests
 
 # Notice the impersonate parameter
-r = requests.get("https://tls.browserleaks.com/json", impersonate="chrome101")
+r = requests.get("https://tls.browserleaks.com/json", impersonate="chrome110")
 
 print(r.json())
-# output: {'ja3_hash': '53ff64ddf993ca882b70e1c82af5da49'
-# the fingerprint should be the same as target browser
+# output: {..., "ja3n_hash": "aa56c057ad164ec4fdcb7a5a283be9fc", ...}
+# the js3n fingerprint should be the same as target browser
 
-# proxies are supported
+# http/socks proxies are supported
 proxies = {"https": "http://localhost:3128"}
-r = requests.get("https://tls.browserleaks.com/json", impersonate="chrome101", proxies=proxies)
+r = requests.get("https://tls.browserleaks.com/json", impersonate="chrome110", proxies=proxies)
 
-# socks proxies are also supported
 proxies = {"https": "socks://localhost:3128"}
-r = requests.get("https://tls.browserleaks.com/json", impersonate="chrome101", proxies=proxies)
+r = requests.get("https://tls.browserleaks.com/json", impersonate="chrome110", proxies=proxies)
 ```
 
 ### Sessions
 
 ```python
 # sessions are supported
 s = requests.Session()
@@ -60,122 +104,78 @@
 print(s.cookies)
 # <Cookies[<Cookie foo=bar for httpbin.org />]>
 r = s.get("https://httpbin.org/cookies")
 print(r.json())
 # {'cookies': {'foo': 'bar'}}
 ```
 
-Supported impersonate versions:
+Supported impersonate versions, as supported by [curl-impersonate](https://github.com/lwthiker/curl-impersonate):
 
 - chrome99
 - chrome100
 - chrome101
 - chrome104
 - chrome107
 - chrome110
 - chrome99_android
 - edge99
 - edge101
 - safari15_3
 - safari15_5
 
+### asyncio
+
+```python
+from curl_cffi.requests import AsyncSession
+
+async with AsyncSession() as s:
+    r = await s.get("https://example.com")
+```
+
+More concurrency:
+
+```python
+import asyncio
+from curl_cffi.requests import AsyncSession
+
+urls = [
+    "https://googel.com/",
+    "https://facebook.com/",
+    "https://twitter.com/",
+]
+
+async with AsyncSession() as s:
+    tasks = []
+    for url in urls:
+        task = s.get("https://example.com")
+        tasks.append(task)
+    results = await asyncio.gather(*tasks)
+```
+
+### curl-like
+
 Alternatively, you can use the low-level curl-like API:
 
 ```python
 from curl_cffi import Curl, CurlOpt
 from io import BytesIO
 
 buffer = BytesIO()
 c = Curl()
 c.setopt(CurlOpt.URL, b'https://tls.browserleaks.com/json')
 c.setopt(CurlOpt.WRITEDATA, buffer)
 
-c.impersonate("chrome101")
+c.impersonate("chrome110")
 
 c.perform()
 c.close()
 body = buffer.getvalue()
 print(body.decode())
 ```
 
-See `example.py` or `tests/` for more examples.
-
-## API
-
-Requests: almost the same as requests.
-
-Curl object:
-
-* `setopt(CurlOpt, value)`: Sets curl options as in `curl_easy_setopt`
-* `perform()`: Performs curl request, as in `curl_easy_perform`
-* `getinfo(CurlInfo)`: Gets information in response after curl perform, as in `curl_easy_getinfo`
-* `close()`: Closes and cleans up the curl object, as in `curl_easy_cleanup`
-
-Enum values to be used with `setopt` and `getinfo`, and can be accessed from `CurlOpt` and `CurlInfo`.
-
-## Trouble Shooting
-
-### Pyinstaller `ModuleNotFoundError: No module named '_cffi_backend'`
-
-You need to tell pyinstaller to pack cffi and data files inside the package:
-
-    pyinstaller -F .\example.py --hidden-import=_cffi_backend --collect-all curl_cffi
-
-### Using https proxy, error: `OPENSSL_internal:WRONG_VERSION_NUMBER`
-
-You are messing up https-over-http proxy and https-over-https proxy, for most cases, you
-should change `{"https": "https://localhost:3128"}` to `{"https": "http://localhost:3128"}`.
-Note the protocol in the url for https proxy is `http` not `https`.
-
-See [this issue](https://github.com/yifeikong/curl_cffi/issues/6#issuecomment-1415162495) for a detailed explaination.
-
-## Current Status
-
-This implementation is very hacky now, but it works for most common systems.
-
-When people installing other python curl bindings, like `pycurl`, they often face
-compiling issues or OpenSSL issues, so I really hope that this package can be distributed
-as a compiled binary package, uses would be able to use it by a simple `pip install`, no
-more compile errors.
-
-For now, I just download the pre-compiled `libcurl-impersonate` from github and build a
-bdist wheel, which is a binary package format used by PyPI, and upload it. However, the
-right way is to download curl and curl-impersonate sources on our side and compile them
-all together.
-
-Help wanted!
-
-TODOs:
-
-- [ ] Write docs.
-- [x] Binary package for macOS(Intel/AppleSilicon) and Windows.
-- [ ] Support musllinux(alpine) bdist by building from source.
-- [x] Exclude the curl headers from source, download them when building.
-- [x] Update curl header files and constants via scripts.
-- [x] Implement `requests.Session/httpx.Client`.
-- [x] Create [ABI3 wheels](https://cibuildwheel.readthedocs.io/en/stable/faq/#abi3) to reduce package size and build time.
-- [ ] Set default headers as in curl-impersonate wrapper scripts.
-- [ ] Support stream in asyncio mode
-    <!--use loop.call_soon(q.put_nowait), wait for headers, then let user iter over content -->
-
-## Change Log
-
-- 0.5.0
-    - Added asyncio support
-
-- 0.4.0
-    - Removed c shim callback function, use cffi native callback function
-
-- 0.3.6
-    - Updated to curl-impersonate v0.5.4, supported chrome107 and chrome110
-
-- 0.3.0, copied more code from `httpx` to support session
-    - Add `requests.Session`
-    - Breaking change: `Response.cookies` changed from `http.cookies.SimpleCookie` to `curl_cffi.requests.Cookies`
-    - Using ABI3 wheels to reduce package size.
+See the [docs](https://curl-cffi.readthedocs.io) for more details.
 
 ## Acknowledgement
 
-- This package was originally forked from https://github.com/multippt/python_curl_cffi , which is under the MIT license.
-- headers/cookies files are copied from https://github.com/encode/httpx/blob/master/httpx/_models.py , which is under the BSD license.
+- Originally forked from [multippt/python_curl_cffi](https://github.com/multippt/python_curl_cffi), which is under the MIT license.
+- Headers/Cookies files are copied from [httpx](https://github.com/encode/httpx/blob/master/httpx/_models.py), which is under the BSD license.
 - Asyncio support is inspired by Tornado's curl http client.
-
```

### Comparing `curl_cffi-0.5.7/curl_cffi/aio.py` & `curl_cffi-0.5.8.1/curl_cffi/aio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __all__ = ["AsyncCurl"]
 
 
 import asyncio
 import os
 from typing import Any
+import warnings
 
 from ._wrapper import ffi, lib  # type: ignore
 from .const import CurlMOpt
 from .curl import Curl, CurlError, CurlInfo
 
 DEFAULT_CACERT = os.path.join(os.path.dirname(__file__), "cacert.pem")
 
@@ -65,72 +66,87 @@
         loop.add_writer(sockfd, async_curl.process_data, sockfd, CURL_CSELECT_OUT)
         async_curl._sockfds.add(sockfd)
     if what & CURL_POLL_REMOVE:
         async_curl._sockfds.remove(sockfd)
 
 
 class AsyncCurl:
+    """Wrapper around curl_multi handle to provide asyncio support. It uses the libcurl
+    socket_action APIs."""
     def __init__(self, cacert: str = DEFAULT_CACERT, loop=None):
         self._curlm = lib.curl_multi_init()
         self._cacert = cacert
         self._curl2future = {}  # curl to future map
         self._curl2curl = {}  # c curl to Curl
         self._sockfds = set()  # sockfds
         self.loop = loop if loop is not None else asyncio.get_running_loop()
         self._checker = self.loop.create_task(self._force_timeout())
         self._timers = []
-        self.setup()
+        self._setup()
 
-    def setup(self):
+    def _setup(self):
         self.setopt(CurlMOpt.TIMERFUNCTION, lib.timer_function)
         self.setopt(CurlMOpt.SOCKETFUNCTION, lib.socket_function)
         self._self_handle = ffi.new_handle(self)
         self.setopt(CurlMOpt.SOCKETDATA, self._self_handle)
         self.setopt(CurlMOpt.TIMERDATA, self._self_handle)
 
     def close(self):
+        """Close and cleanup running timers, readers, writers and handles."""
+        # Close force timeout checker
         self._checker.cancel()
+        # Close all pending futures
         for curl, future in self._curl2future.items():
             lib.curl_multi_remove_handle(self._curlm, curl._curl)
             if not future.done() and not future.cancelled():
                 future.set_result(None)
+        # Cleanup curl_multi handle
         lib.curl_multi_cleanup(self._curlm)
         self._curlm = None
+        # Remove add readers and writers
         for sockfd in  self._sockfds:
             self.loop.remove_reader(sockfd)
             self.loop.remove_writer(sockfd)
+        # Cancel all time functions
         for timer in self._timers:
             timer.cancel()
 
     async def _force_timeout(self):
         while True:
             if not self._curlm:
                 break
             await asyncio.sleep(1)
             # print("force timeout")
             self.socket_action(CURL_SOCKET_TIMEOUT, CURL_POLL_NONE)
 
     async def add_handle(self, curl: Curl, wait=True):
+        """Add a curl handle to be managed by curl_multi. This is the equivalent of
+        `perform` in the async world."""
         # import pdb; pdb.set_trace()
-        curl.ensure_cacert()
+        curl._ensure_cacert()
         lib.curl_multi_add_handle(self._curlm, curl._curl)
         future = self.loop.create_future()
         self._curl2future[curl] = future
         self._curl2curl[curl._curl] = curl
         if wait:
-            await future
+            try:
+                await future
+            finally:
+                curl.clean_after_perform()
 
     def socket_action(self, sockfd: int, ev_bitmask: int) -> int:
+        """Call libcurl socket_action function"""
         running_handle = ffi.new("int *")
         lib.curl_multi_socket_action(self._curlm, sockfd, ev_bitmask, running_handle)
         return running_handle[0]
 
     def process_data(self, sockfd: int, ev_bitmask: int):
+        """Call curl_multi_info_read to read data for given socket."""
         if not self._curlm:
-            print("Curlm alread closed! quitting from process_data")
+            warnings.warn("Curlm alread closed! quitting from process_data")
             return
 
         self.socket_action(sockfd, ev_bitmask)
 
         msg_in_queue = ffi.new("int *")
         while True:
             curl_msg = lib.curl_multi_info_read(self._curlm, msg_in_queue)
@@ -143,30 +159,34 @@
                 retcode = curl_msg.data.result
                 if retcode == 0:
                     self.set_result(curl)
                 else:
                     # import pdb; pdb.set_trace()
                     self.set_exception(curl, curl._get_error(retcode, "perform"))
             else:
-                print("NOT DONE")
+                print("NOT DONE")  # Will not reach, for no other code being defined.
 
     def _pop_future(self, curl: Curl):
         lib.curl_multi_remove_handle(self._curlm, curl._curl)
         self._curl2curl.pop(curl._curl)
         return self._curl2future.pop(curl)
 
     def cancel_handle(self, curl: Curl):
+        """Cancel a future for given curl handle."""
         future = self._pop_future(curl)
         future.cancel()
 
     def set_result(self, curl: Curl):
+        """Mark a future as done for given curl handle."""
         future = self._pop_future(curl)
         if not future.done() and not future.cancelled():
             future.set_result(None)
 
     def set_exception(self, curl: Curl, exception):
+        """Raise exception of a future for given curl handle."""
         future = self._pop_future(curl)
         if not future.done() and not future.cancelled():
             future.set_exception(exception)
 
     def setopt(self, option, value):
+        """Wrapper around curl_multi_setopt."""
         return lib.curl_multi_setopt(self._curlm, option, value)
```

### Comparing `curl_cffi-0.5.7/curl_cffi/build.py` & `curl_cffi-0.5.8.1/curl_cffi/build.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.7/curl_cffi/curl.py` & `curl_cffi-0.5.8.1/curl_cffi/curl.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,38 +7,39 @@
 from ._wrapper import ffi, lib  # type: ignore
 from .const import CurlInfo, CurlOpt
 
 DEFAULT_CACERT = os.path.join(os.path.dirname(__file__), "cacert.pem")
 
 
 class CurlError(Exception):
-    pass
+    """Base exception for curl_cffi package"""
+
+    def __init__(self, msg, code: int = 0, *args, **kwargs):
+        super().__init__(msg, *args, **kwargs)
+        self.code = code
 
 
 CURLINFO_TEXT = 0
 CURLINFO_HEADER_IN = 1
 CURLINFO_HEADER_OUT = 2
 CURLINFO_DATA_IN = 3
 CURLINFO_DATA_OUT = 4
 CURLINFO_SSL_DATA_IN = 5
 CURLINFO_SSL_DATA_OUT = 6
-CURLINFO_DATA_OUT = 4
 
 
 @ffi.def_extern()
 def debug_function(curl, type: int, data, size, clientp) -> int:
     text = ffi.buffer(data, size)[:]
-    if type == 0:
-        print("CURLINFO", text)
-    elif type == 2:
-        print("HEADER OUT", text)
-    elif type == 4:
-        print("DATA OUT", text)
-    elif type == 6:
+    if type in (CURLINFO_SSL_DATA_IN, CURLINFO_SSL_DATA_OUT):
         print("SSL OUT", text)
+    elif type in (CURLINFO_DATA_IN, CURLINFO_DATA_OUT):
+        print(text.decode())
+    else:
+        print(text.decode(), end="")
     return 0
 
 
 @ffi.def_extern()
 def buffer_callback(ptr, size, nmemb, userdata):
     # assert size == 1
     buffer = ffi.from_handle(userdata)
@@ -50,31 +51,51 @@
 def write_callback(ptr, size, nmemb, userdata):
     # although similar enough to the function above, kept here for performance reasons
     callback = ffi.from_handle(userdata)
     callback(ffi.buffer(ptr, nmemb)[:])
     return nmemb * size
 
 
+# Credits: @alexio777 on https://github.com/yifeikong/curl_cffi/issues/4
+def slist_to_list(head) -> List[bytes]:
+    result = []
+    ptr = head
+    while ptr:
+        result.append(ffi.string(ptr.data))
+        ptr = ptr.next
+    lib.curl_slist_free_all(head)
+    return result
+
+
 class Curl:
-    def __init__(self, cacert: str = DEFAULT_CACERT, debug: bool=False):
+    """
+    Wrapper for `curl_easy_*` functions of libcurl.
+    """
+
+    def __init__(self, cacert: str = DEFAULT_CACERT, debug: bool = False):
+        """
+        Parameters:
+            cacert: CA cert path to use, by default, curl_cffi uses its own bundled cert.
+            debug: whether to show curl debug messages.
+        """
         self._curl = lib.curl_easy_init()
         self._headers = ffi.NULL
         self._cacert = cacert
         self._is_cert_set = False
         self._write_handle = None
         self._header_handle = None
         # TODO: use CURL_ERROR_SIZE
         self._error_buffer = ffi.new("char[]", 256)
         self._debug = debug
-        self.set_error_buffer()
+        self._set_error_buffer()
 
-    def set_error_buffer(self):
+    def _set_error_buffer(self):
         ret = lib._curl_easy_setopt(self._curl, CurlOpt.ERRORBUFFER, self._error_buffer)
         if ret != 0:
-            warnings.warn(f"Failed to set error buffer")
+            warnings.warn("Failed to set error buffer")
         if self._debug:
             self.setopt(CurlOpt.VERBOSE, 1)
             lib._curl_easy_setopt(self._curl, CurlOpt.DEBUGFUNCTION, lib.debug_function)
 
     def __del__(self):
         self.close()
 
@@ -83,18 +104,27 @@
         if error is not None:
             raise error
 
     def _get_error(self, errcode: int, action: str):
         if errcode != 0:
             errmsg = ffi.string(self._error_buffer).decode()
             return CurlError(
-                f"Failed to {action}, ErrCode: {errcode}, Reason: '{errmsg}'"
+                f"Failed to {action}, ErrCode: {errcode}, Reason: '{errmsg}'. "
+                "This may be a libcurl error, "
+                "See https://curl.se/libcurl/c/libcurl-errors.html first for more details.",
+                code=errcode,
             )
 
     def setopt(self, option: CurlOpt, value: Any):
+        """Wrapper for curl_easy_setopt.
+
+        Parameters:
+            option: option to set, use the constants from CurlOpt enum
+            value: value to set, strings will be handled automatically
+        """
         input_option = {
             # this should be int in curl, but cffi requires pointer for void*
             # it will be convert back in the glue c code.
             0: "int*",
             10000: "char*",
             20000: "void*",
             30000: "int*",  # offset type
@@ -128,15 +158,15 @@
             lib._curl_easy_setopt(self._curl, CurlOpt.WRITEFUNCTION, lib.write_callback)
             option = CurlOpt.HEADERDATA
         elif value_type == "char*":
             if isinstance(value, str):
                 c_value = value.encode()
             else:
                 c_value = value
-            # Must keep a reference, otherwisd may be GCed.
+            # Must keep a reference, otherwise may be GCed.
             if option == CurlOpt.POSTFIELDS:
                 self._body_handle = c_value
         else:
             raise NotImplementedError("Option unsupported: %s" % option)
 
         if option == CurlOpt.HTTPHEADER:
             for header in value:
@@ -147,79 +177,114 @@
         self._check_error(ret, "setopt(%s, %s)" % (option, value))
 
         if option == CurlOpt.CAINFO:
             self._is_cert_set = True
 
         return ret
 
-    def getinfo(self, option: CurlInfo) -> Union[bytes, int, float]:
+    def getinfo(self, option: CurlInfo) -> Union[bytes, int, float, List]:
+        """Wrapper for curl_easy_getinfo. Gets information in response after curl perform.
+
+        Parameters:
+            option: option to get info of, use the constants from CurlInfo enum
+        """
         ret_option = {
             0x100000: "char**",
             0x200000: "long*",
             0x300000: "double*",
+            0x400000: "struct curl_slist **",
         }
         ret_cast_option = {
             0x100000: ffi.string,
             0x200000: int,
             0x300000: float,
         }
         c_value = ffi.new(ret_option[option & 0xF00000])
         ret = lib.curl_easy_getinfo(self._curl, option, c_value)
         self._check_error(ret, action="getinfo(%s)" % option)
+        # cookielist and ssl_engines starts with 0x400000, see also: const.py
+        if option & 0xF00000 == 0x400000:
+            return slist_to_list(c_value[0])
         if c_value[0] == ffi.NULL:
             return b""
         return ret_cast_option[option & 0xF00000](c_value[0])
 
     def version(self) -> bytes:
+        """Get the underlying libcurl version."""
         return ffi.string(lib.curl_version())
 
     def impersonate(self, target: str, default_headers: bool = True) -> int:
+        """Set the browser type to impersonate.
+
+        Parameters:
+            target: browser to impersonate.
+            default_headers: whether to add default headers, like User-Agent.
+        """
         return lib.curl_easy_impersonate(
             self._curl, target.encode(), int(default_headers)
         )
 
-    def ensure_cacert(self):
+    def _ensure_cacert(self):
         if not self._is_cert_set:
             ret = self.setopt(CurlOpt.CAINFO, self._cacert)
             self._check_error(ret, action="set cacert")
 
     def perform(self, clear_headers: bool = True):
+        """Wrapper for curl_easy_perform, performs a curl request.
+
+        Parameters:
+            clear_headers: clear header slist used in this perform
+        """
         # make sure we set a cacert store
-        self.ensure_cacert()
+        self._ensure_cacert()
 
         # here we go
         ret = lib.curl_easy_perform(self._curl)
-        self._check_error(ret, action="perform")
 
-        # cleaning
-        self.clean_after_perform(clear_headers)
+        try:
+            self._check_error(ret, action="perform")
+        finally:
+            # cleaning
+            self.clean_after_perform(clear_headers)
 
     def clean_after_perform(self, clear_headers: bool = True):
+        """Clean up handles and buffers after perform, called at the end of `perform`."""
         self._write_handle = None
         self._header_handle = None
         self._body_handle = None
         if clear_headers:
             if self._headers != ffi.NULL:
                 lib.curl_slist_free_all(self._headers)
             self._headers = ffi.NULL
 
     def reset(self):
+        """Reset all curl options, wrapper for curl_easy_reset."""
         self._is_cert_set = False
         lib.curl_easy_reset(self._curl)
-        self.set_error_buffer()
+        self._set_error_buffer()
 
     def parse_cookie_headers(self, headers: List[bytes]) -> SimpleCookie:
+        """Extract cookies.SimpleCookie from header lines.
+
+        Parameters:
+            headers: list of headers in bytes.
+
+        Returns:
+            A parsed cookies.SimpleCookie instance.
+        """
         cookie = SimpleCookie()
         for header in headers:
             if header.lower().startswith(b"set-cookie: "):
                 cookie.load(header[12:].decode())  # len("set-cookie: ") == 12
         return cookie
 
     def get_reason_phrase(self, status_line: bytes) -> bytes:
+        """Extract reason phrase, like `OK`, `Not Found` from response status line."""
         m = re.match(rb"HTTP/\d\.\d [0-9]{3} (.*)", status_line)
         return m.group(1) if m else b""
 
     def close(self):
+        """Close and cleanup curl handle, wrapper for curl_easy_cleanup"""
         if self._curl:
             lib.curl_easy_cleanup(self._curl)
             self._curl = None
         ffi.release(self._error_buffer)
```

### Comparing `curl_cffi-0.5.7/curl_cffi/ffi/cdef.c` & `curl_cffi-0.5.8.1/curl_cffi/ffi/cdef.c`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 int _curl_easy_setopt(void *curl, int option, void *param);
 int curl_easy_getinfo(void *curl, int option, void *ret);
 int curl_easy_perform(void *curl);
 void curl_easy_cleanup(void *curl);
 void curl_easy_reset(void *curl);
 char *curl_version();
 int curl_easy_impersonate(void *curl, char *target, int default_headers);
+struct curl_slist {
+   char *data;
+   struct curl_slist *next;
+};
 struct curl_slist *curl_slist_append(struct curl_slist *list, char *string);
 void curl_slist_free_all(struct curl_slist *list);
 extern "Python" size_t buffer_callback(void *ptr, size_t size, size_t nmemb, void *userdata);
 extern "Python" size_t write_callback(void *ptr, size_t size, size_t nmemb, void *userdata);
 extern "Python" int debug_function(void *curl, int type, char *data, size_t size, void *clientp);
 
 // multi interfaces
```

### Comparing `curl_cffi-0.5.7/curl_cffi/ffi/shim.c` & `curl_cffi-0.5.8.1/curl_cffi/ffi/shim.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.7/curl_cffi/requests/headers.py` & `curl_cffi-0.5.8.1/curl_cffi/requests/headers.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.7/curl_cffi/requests/session.py` & `curl_cffi-0.5.8.1/curl_cffi/requests/session.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import asyncio
 import sys
 import re
 import threading
 import warnings
 from enum import Enum
+from http.cookiejar import Cookie
 from functools import partialmethod
 from io import BytesIO
 from json import dumps
 from typing import Callable, Dict, List, Optional, Tuple, Union, cast
 from urllib.parse import ParseResult, parse_qsl, unquote, urlencode, urlparse
 
-from .. import AsyncCurl, Curl, CurlError, CurlInfo, CurlOpt
-from .cookies import Cookies, CookieTypes, Request, Response
+from .. import AsyncCurl, Curl, CurlError, CurlInfo, CurlOpt, CurlHttpVersion
+from .cookies import Cookies, CookieTypes
 from .errors import RequestsError
 from .headers import Headers, HeaderTypes
+from .models import Request, Response
 
 try:
     import gevent
 except ImportError:
     pass
 
 try:
@@ -27,14 +29,15 @@
 
 
 WINDOWS_WARN = """
 WindowsProactorEventLoopPolicy is not supported, you can use the selector loop by:
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 """
 
+
 class BrowserType(str, Enum):
     edge99 = "edge99"
     edge101 = "edge101"
     chrome99 = "chrome99"
     chrome100 = "chrome100"
     chrome101 = "chrome101"
     chrome104 = "chrome104"
@@ -48,17 +51,20 @@
     def has(cls, item):
         return item in cls.__members__
 
 
 def _update_url_params(url: str, params: Dict) -> str:
     """Add GET params to provided URL being aware of existing.
 
-    :param url: string of target URL
-    :param params: dict containing requested params to be added
-    :return: string with updated URL
+    Parameters:
+        url: string of target URL
+        params: dict containing requested params to be added
+
+    Returns:
+        string with updated URL
 
     >> url = 'http://stackoverflow.com/test?answers=true'
     >> new_params = {'answers': False, 'data': ['some','values']}
     >> _update_url_params(url, new_params)
     'http://stackoverflow.com/test?data=some&data=values&answers=false'
     """
     # Unquoting URL first so we don't loose existing args
@@ -91,32 +97,34 @@
         parsed_url.fragment,
     ).geturl()
 
     return new_url
 
 
 def _update_header_line(header_lines: List[str], key: str, value: str):
+    """Update header line list by key value pair."""
     for idx, line in enumerate(header_lines):
-        if line.lower().startswith(key + ":"):
+        if line.lower().startswith(key.lower() + ":"):
             header_lines[idx] = f"{key}: {value}"
             break
     else:  # if not break
         header_lines.append(f"{key}: {value}")
 
 
 class BaseSession:
+    """Provide common methods for setting curl options and reading info in sessions."""
+
     __attrs__ = [
         "headers",
         "cookies",
         "auth",
         "proxies",
         "params",
         "verify",
         "cert",
-        "stream",  # TODO
         "trust_env",  # TODO
         "max_redirects",
         "impersonate",
         "timeout",
     ]
 
     def __init__(
@@ -128,25 +136,103 @@
         proxies: Optional[dict] = None,
         params: Optional[dict] = None,
         verify: bool = True,
         timeout: Union[float, Tuple[float, float]] = 30,
         trust_env: bool = True,
         max_redirects: int = -1,
         impersonate: Optional[Union[str, BrowserType]] = None,
+        default_headers: bool = True,
+        curl_options: Optional[dict] = None,
+        http_version: Optional[CurlHttpVersion] = None,
+        debug: bool = False,
+        interface: Optional[str] = None,
     ):
         self.headers = Headers(headers)
         self.cookies = Cookies(cookies)
         self.auth = auth
         self.proxies = proxies
         self.params = params
         self.verify = verify
         self.timeout = timeout
         self.trust_env = trust_env
         self.max_redirects = max_redirects
         self.impersonate = impersonate
+        self.default_headers = default_headers
+        self.curl_options = curl_options or {}
+        self.http_version = http_version
+        self.debug = debug
+        self.interface = interface
+
+    def _set_cookies(self, curl, cookies: Cookies):
+        curl.setopt(CurlOpt.COOKIELIST, "ALL")  # remove all the old cookies first.
+        # Credits: @coletdjnz
+        # encoder = SimpleCookie()
+        for cookie in cookies.jar:
+            values = []
+            # _, value = encoder.value_encode(cookie.value)
+            # values.append(f"{cookie.name}={value}")
+            # Let curl decide how to encode cookies
+            values.append(f"{cookie.name}={cookie.value}")
+            if cookie.domain:
+                values.append(f"Domain={cookie.domain}")
+            if cookie.path:
+                values.append(f"Path={cookie.path}")
+            if cookie.secure:
+                values.append("Secure")
+            if cookie.expires:
+                values.append(f"Expires={cookie.expires}")
+            if cookie.version:
+                values.append(f"Version={cookie.version}")
+            cookie_line = "set-cookie: " + ("; ".join(values))
+            # print(cookie_line)
+            # https://curl.se/libcurl/c/CURLOPT_COOKIELIST.html
+            curl.setopt(CurlOpt.COOKIELIST, cookie_line.encode())
+
+    def _extract_cookies(self, curl) -> List[Cookie]:
+        cookie_lines = curl.getinfo(CurlInfo.COOKIELIST)
+        cookies = []
+        for cookie_line in cookie_lines:
+            (
+                hostname,
+                subdomains,
+                path,
+                secure,
+                expires,
+                name,
+                value,
+            ) = cookie_line.decode().split("\t")
+            if hostname and hostname[0] == "#":
+                http_only = True
+                # e.g. #HttpOnly_postman-echo.com
+                domain = hostname[10:]  # len("#HttpOnly_") == 10
+            else:
+                http_only = False
+                domain = hostname
+            cookies.append(
+                Cookie(
+                    version=0,
+                    name=name,
+                    value=value,
+                    port=None,
+                    port_specified=False,
+                    domain=domain,
+                    domain_specified=bool(domain),
+                    domain_initial_dot=(subdomains == "TRUE"),
+                    path=path,
+                    path_specified=bool(path),
+                    secure=(secure == "TRUE"),
+                    expires=int(expires),
+                    discard=False,
+                    comment=None,
+                    comment_url=None,
+                    rest=dict(http_only=http_only),  # type: ignore
+                    rfc2109=False,
+                )
+            )
+        return cookies
 
     def _set_curl_options(
         self,
         curl,
         method: str,
         url: str,
         params: Optional[dict] = None,
@@ -156,19 +242,22 @@
         cookies: Optional[CookieTypes] = None,
         files: Optional[Dict] = None,
         auth: Optional[Tuple[str, str]] = None,
         timeout: Optional[Union[float, Tuple[float, float]]] = None,
         allow_redirects: bool = True,
         max_redirects: Optional[int] = None,
         proxies: Optional[dict] = None,
-        verify: Optional[bool] = None,
+        verify: Optional[Union[bool, str]] = None,
         referer: Optional[str] = None,
         accept_encoding: Optional[str] = "gzip, deflate, br",
         content_callback: Optional[Callable] = None,
         impersonate: Optional[Union[str, BrowserType]] = None,
+        default_headers: Optional[bool] = None,
+        http_version: Optional[CurlHttpVersion] = None,
+        interface: Optional[str] = None,
     ):
         c = curl
 
         # method
         c.setopt(CurlOpt.CUSTOMREQUEST, method.encode())
 
         # url
@@ -198,37 +287,32 @@
             # necessary if body contains '\0'
             c.setopt(CurlOpt.POSTFIELDSIZE, len(body))
 
         # headers
         h = Headers(self.headers)
         h.update(headers)
 
-        # cookies
-        co = Cookies(self.cookies)
-        co.update(cookies)
-        req = Request(url=url, headers=h, method=method)
-        co.set_cookie_header(req)
-
-        # An alternative way to implement cookiejar is to use curl's builtin cookiejar,
-        # However, it would be diffcult to interploate with Headers and get cookies as
-        # dicta
-        # c.setopt(CurlOpt.COOKIE, cookies_str.encode())
-
         header_lines = []
         for k, v in h.multi_items():
             header_lines.append(f"{k}: {v}")
         if json:
             _update_header_line(header_lines, "Content-Type", "application/json")
         if isinstance(data, dict):
             _update_header_line(
                 header_lines, "Content-Type", "application/x-www-form-urlencoded"
             )
         # print("header lines", header_lines)
         c.setopt(CurlOpt.HTTPHEADER, [h.encode() for h in header_lines])
 
+        # cookies
+        c.setopt(CurlOpt.COOKIEFILE, b"")  # always enable the curl cookie engine first
+        co = Cookies(self.cookies)
+        co.update(cookies)
+        self._set_cookies(c, co)
+
         # files
         if files:
             raise NotImplementedError("Files has not been implemented.")
 
         # auth
         if self.auth or auth:
             if self.auth:
@@ -274,47 +358,76 @@
                         c.setopt(CurlOpt.HTTPPROXYTUNNEL, 1)
 
         # verify
         if verify is False or not self.verify and verify is None:
             c.setopt(CurlOpt.SSL_VERIFYPEER, 0)
             c.setopt(CurlOpt.SSL_VERIFYHOST, 0)
 
+        # cert for this single request
+        if isinstance(verify, str):
+            c.setopt(CurlOpt.CAINFO, verify)
+
+        # cert for the session
+        if verify in (None, True) and isinstance(self.verify, str):
+            c.setopt(CurlOpt.CAINFO, self.verify)
+
         # referer
         if referer:
             c.setopt(CurlOpt.REFERER, referer.encode())
 
         # accept_encoding
         if accept_encoding is not None:
             c.setopt(CurlOpt.ACCEPT_ENCODING, accept_encoding.encode())
 
         # impersonate
         impersonate = impersonate or self.impersonate
+        default_headers = (
+            self.default_headers if default_headers is None else default_headers
+        )
         if impersonate:
             if not BrowserType.has(impersonate):
                 raise RequestsError(f"impersonate {impersonate} is not supported")
-            c.impersonate(impersonate)
+            c.impersonate(impersonate, default_headers=default_headers)
+
+        # http_version, after impersonate, which will change this to http2
+        http_version = http_version or self.http_version
+        if http_version:
+            c.setopt(CurlOpt.HTTP_VERSION, http_version)
+
+        # set extra curl options, must come after impersonate, because it will alter some options
+        for k, v in self.curl_options.items():
+            c.setopt(k, v)
 
         # import pdb; pdb.set_trace()
         if content_callback is None:
             buffer = BytesIO()
             c.setopt(CurlOpt.WRITEDATA, buffer)
         else:
             buffer = None
             c.setopt(CurlOpt.WRITEFUNCTION, content_callback)
         header_buffer = BytesIO()
         c.setopt(CurlOpt.HEADERDATA, header_buffer)
 
-        return req, buffer, header_buffer
+        if method == "HEAD":
+            c.setopt(CurlOpt.NOBODY, 1)
+
+        # interface
+        interface = interface or self.interface
+        if interface:
+            c.setopt(CurlOpt.INTERFACE, interface.encode())
+
+        return Request(url, h, method), buffer, header_buffer
 
-    def _parse_response(self, curl, req: Request, buffer, header_buffer):
+    def _parse_response(self, curl, buffer, header_buffer):
         c = curl
-        rsp = Response(c, req)
+        rsp = Response(c)
         rsp.url = cast(bytes, c.getinfo(CurlInfo.EFFECTIVE_URL)).decode()
         if buffer:
             rsp.content = buffer.getvalue()  # type: ignore
+        rsp.http_version = cast(int, c.getinfo(CurlInfo.HTTP_VERSION))
         rsp.status_code = cast(int, c.getinfo(CurlInfo.RESPONSE_CODE))
         rsp.ok = 200 <= rsp.status_code < 400
         header_lines = header_buffer.getvalue().splitlines()
 
         # TODO history urls
         header_list = []
         for header_line in header_lines:
@@ -326,16 +439,19 @@
                 # empty header list for new redirected response
                 header_list = [
                     h for h in header_lines if h.lower().startswith(b"set-cookie")
                 ]
                 continue
             header_list.append(header_line)
         rsp.headers = Headers(header_list)
+
+        cookies = self._extract_cookies(c)
+        for cookie in cookies:
+            self.cookies.jar.set_cookie(cookie)
         rsp.cookies = self.cookies
-        self.cookies.extract_cookies(rsp)
         # print("Cookies after extraction", self.cookies)
 
         content_type = rsp.headers.get("Content-Type", default="")
         m = re.search(r"charset=([\w-]+)", content_type)
         charset = m.group(1) if m else "utf-8"
 
         rsp.charset = charset
@@ -348,42 +464,87 @@
         return rsp
 
 
 # ThreadType = Literal["eventlet", "gevent", None]
 
 
 class Session(BaseSession):
+    """A request session, cookies and connections will be reused. This object is thread-safe,
+    but it's recommended to use a seperate session for each thread."""
+
     def __init__(
-        self, curl: Optional[Curl] = None, thread: Optional[str] = None, **kwargs
+        self,
+        curl: Optional[Curl] = None,
+        thread: Optional[str] = None,
+        use_thread_local_curl: bool = True,
+        **kwargs,
     ):
+        """
+        Parameters set in the init method will be override by the same parameter in request method.
+
+        Parameters:
+            curl: curl object to use in the session. If not provided, a new one will be
+                created. Also, a fresh curl object will always be created when accessed
+                from another thread.
+            thread: thread engine to use for working with other thread implementations.
+                choices: eventlet, gevent., possible values: eventlet, gevent.
+            headers: headers to use in the session.
+            cookies: cookies to add in the session.
+            auth: HTTP basic auth, a tuple of (username, password), only basic auth is supported.
+            proxies: dict of proxies to use, format: {"http": proxy_url, "https": proxy_url}.
+            params: query string for the session.
+            verify: whether to verify https certs.
+            timeout: how many seconds to wait before giving up.
+            trust_env: use http_proxy/https_proxy and other environments, default True.
+            max_redirects: max redirect counts, default unlimited(-1).
+            impersonate: which browser version to impersonate in the session.
+            interface: which interface use in request to server.
+
+        Notes:
+            This class can be used as a context manager.
+            ```
+            from curl_cffi.requests import Session
+
+            with Session() as s:
+                r = s.get("https://example.com")
+            ```
+        """
         super().__init__(**kwargs)
         self._thread = thread
-        self._local = threading.local()
-        if curl:
-            self._is_customized_curl = True
-            self._local.curl = curl
+        self._use_thread_local_curl = use_thread_local_curl
+        if use_thread_local_curl:
+            self._local = threading.local()
+            if curl:
+                self._is_customized_curl = True
+                self._local.curl = curl
+            else:
+                self._is_customized_curl = False
+                self._local.curl = Curl(debug=self.debug)
         else:
-            self._is_customized_curl = False
-            self._local.curl = Curl()
+            self._curl = curl if curl else Curl(debug=self.debug)
 
     @property
     def curl(self):
-        if self._is_customized_curl:
-            warnings.warn("Creating fresh curl in different thread.")
-        if not getattr(self._local, "curl", None):
-            self._local.curl = Curl()
-        return self._local.curl
+        if self._use_thread_local_curl:
+            if self._is_customized_curl:
+                warnings.warn("Creating fresh curl in different thread.")
+            if not getattr(self._local, "curl", None):
+                self._local.curl = Curl(debug=self.debug)
+            return self._local.curl
+        else:
+            return self._curl
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def close(self):
+        """Close the session."""
         self.curl.close()
 
     def request(
         self,
         method: str,
         url: str,
         params: Optional[dict] = None,
@@ -398,71 +559,109 @@
         max_redirects: Optional[int] = None,
         proxies: Optional[dict] = None,
         verify: Optional[bool] = None,
         referer: Optional[str] = None,
         accept_encoding: Optional[str] = "gzip, deflate, br",
         content_callback: Optional[Callable] = None,
         impersonate: Optional[Union[str, BrowserType]] = None,
+        default_headers: Optional[bool] = None,
+        http_version: Optional[CurlHttpVersion] = None,
+        interface: Optional[str] = None,
     ) -> Response:
+        """Send the request, see [curl_cffi.requests.request](/api/curl_cffi.requests/#curl_cffi.requests.request) for details on parameters."""
         c = self.curl
         req, buffer, header_buffer = self._set_curl_options(
             c,
-            method,
-            url,
-            params,
-            data,
-            json,
-            headers,
-            cookies,
-            files,
-            auth,
-            timeout,
-            allow_redirects,
-            max_redirects,
-            proxies,
-            verify,
-            referer,
-            accept_encoding,
-            content_callback,
-            impersonate,
+            method=method,
+            url=url,
+            params=params,
+            data=data,
+            json=json,
+            headers=headers,
+            cookies=cookies,
+            files=files,
+            auth=auth,
+            timeout=timeout,
+            allow_redirects=allow_redirects,
+            max_redirects=max_redirects,
+            proxies=proxies,
+            verify=verify,
+            referer=referer,
+            accept_encoding=accept_encoding,
+            content_callback=content_callback,
+            impersonate=impersonate,
+            default_headers=default_headers,
+            http_version=http_version,
+            interface=interface,
         )
         try:
             if self._thread == "eventlet":
                 # see: https://eventlet.net/doc/threading.html
                 eventlet.tpool.execute(c.perform)
             elif self._thread == "gevent":
                 # see: https://www.gevent.org/api/gevent.threadpool.html
                 gevent.get_hub().threadpool.spawn(c.perform).get()
             else:
                 c.perform()
         except CurlError as e:
             raise RequestsError(e)
-
-        rsp = self._parse_response(c, req, buffer, header_buffer)
-        self.curl.reset()
-        return rsp
+        else:
+            rsp = self._parse_response(c, buffer, header_buffer)
+            rsp.request = req
+            return rsp
+        finally:
+            self.curl.reset()
 
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
     delete = partialmethod(request, "DELETE")
     options = partialmethod(request, "OPTIONS")
 
 
 class AsyncSession(BaseSession):
+    """An async request session, cookies and connections will be reused."""
+
     def __init__(
         self,
         *,
         loop=None,
         async_curl: Optional[AsyncCurl] = None,
         max_clients: int = 10,
         **kwargs,
     ):
+        """
+        Parameters set in the init method will be override by the same parameter in request method.
+
+        Parameters:
+            loop: loop to use, if not provided, the running loop will be used.
+            async_curl: [AsyncCurl](/api/curl_cffi#curl_cffi.AsyncCurl) object to use.
+            max_clients: maxmium curl handle to use in the session, this will affect the concurrency ratio.
+            headers: headers to use in the session.
+            cookies: cookies to add in the session.
+            auth: HTTP basic auth, a tuple of (username, password), only basic auth is supported.
+            proxies: dict of proxies to use, format: {"http": proxy_url, "https": proxy_url}.
+            params: query string for the session.
+            verify: whether to verify https certs.
+            timeout: how many seconds to wait before giving up.
+            trust_env: use http_proxy/https_proxy and other environments, default True.
+            max_redirects: max redirect counts, default unlimited(-1).
+            impersonate: which browser version to impersonate in the session.
+
+        Notes:
+            This class can be used as a context manager, and it's recommended to use via `async with`.
+            ```
+            from curl_cffi.requests import AsyncSession
+
+            async with AsyncSession() as s:
+                r = await s.get("https://example.com")
+            ```
+        """
         super().__init__(**kwargs)
         self.loop = loop if loop is not None else asyncio.get_running_loop()
         self.acurl = async_curl if async_curl is not None else AsyncCurl(loop=self.loop)
         self.max_clients = max_clients
         self.reset()
         if sys.version_info >= (3, 8) and sys.platform.lower().startswith("win"):
             if isinstance(
@@ -478,15 +677,15 @@
             except asyncio.QueueFull:
                 break
         self._running_curl = []
 
     async def pop_curl(self):
         curl = await self.pool.get()
         if curl is None:
-            curl = Curl()
+            curl = Curl(debug=self.debug)
             self._running_curl.append(curl)
         return curl
 
     def push_curl(self, curl):
         try:
             self.pool.put_nowait(curl)
         except asyncio.QueueFull:
@@ -496,14 +695,15 @@
         return self
 
     async def __aexit__(self, *args):
         self.close()
         return None
 
     def close(self):
+        """Close the session."""
         self.acurl.close()
 
     async def request(
         self,
         method: str,
         url: str,
         params: Optional[dict] = None,
@@ -518,48 +718,57 @@
         max_redirects: Optional[int] = None,
         proxies: Optional[dict] = None,
         verify: Optional[bool] = None,
         referer: Optional[str] = None,
         accept_encoding: Optional[str] = "gzip, deflate, br",
         content_callback: Optional[Callable] = None,
         impersonate: Optional[Union[str, BrowserType]] = None,
+        default_headers: Optional[bool] = None,
+        http_version: Optional[CurlHttpVersion] = None,
+        interface: Optional[str] = None,
     ):
+        """Send the request, see [curl_cffi.requests.request](/api/curl_cffi.requests/#curl_cffi.requests.request) for details on parameters."""
         curl = await self.pop_curl()
         req, buffer, header_buffer = self._set_curl_options(
-            curl,
-            method,
-            url,
-            params,
-            data,
-            json,
-            headers,
-            cookies,
-            files,
-            auth,
-            timeout,
-            allow_redirects,
-            max_redirects,
-            proxies,
-            verify,
-            referer,
-            accept_encoding,
-            content_callback,
-            impersonate,
+            curl=curl,
+            method=method,
+            url=url,
+            params=params,
+            data=data,
+            json=json,
+            headers=headers,
+            cookies=cookies,
+            files=files,
+            auth=auth,
+            timeout=timeout,
+            allow_redirects=allow_redirects,
+            max_redirects=max_redirects,
+            proxies=proxies,
+            verify=verify,
+            referer=referer,
+            accept_encoding=accept_encoding,
+            content_callback=content_callback,
+            impersonate=impersonate,
+            default_headers=default_headers,
+            http_version=http_version,
+            interface=interface,
         )
         try:
             # curl.debug()
             await self.acurl.add_handle(curl)
             # print(curl.getinfo(CurlInfo.CAINFO))
-            curl.clean_after_perform()
         except CurlError as e:
             raise RequestsError(e)
-        rsp = self._parse_response(curl, req, buffer, header_buffer)
-        curl.reset()
-        self.push_curl(curl)
-        return rsp
+        else:
+            rsp = self._parse_response(curl, buffer, header_buffer)
+            rsp.request = req
+            return rsp
+        finally:
+            curl.reset()
+            self.push_curl(curl)
 
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
     post = partialmethod(request, "POST")
     put = partialmethod(request, "PUT")
     patch = partialmethod(request, "PATCH")
     delete = partialmethod(request, "DELETE")
```

### Comparing `curl_cffi-0.5.7/curl_cffi.egg-info/SOURCES.txt` & `curl_cffi-0.5.8.1/curl_cffi.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 curl_cffi/ffi/cdef.c
 curl_cffi/ffi/shim.c
 curl_cffi/ffi/shim.h
 curl_cffi/requests/__init__.py
 curl_cffi/requests/cookies.py
 curl_cffi/requests/errors.py
 curl_cffi/requests/headers.py
+curl_cffi/requests/models.py
 curl_cffi/requests/session.py
```

### Comparing `curl_cffi-0.5.7/curl_cffi.egg-info/requires.txt` & `curl_cffi-0.5.8.1/curl_cffi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.5.7/pyproject.toml` & `curl_cffi-0.5.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curl_cffi"
-version = "0.5.7"
+version = "0.5.8.1"
 authors = [{ name = "Yifei Kong", email = "kong@yifei.me" }]
 description = "libcurl ffi bindings for Python, with impersonation support"
 license = { file = "LICENSE" }
 dependencies = ["cffi>=1.12.0"]
 readme = "README.md"
 requires-python = ">=3.7"
 urls = { "repository" = "https://github.com/yifeikong/curl_cffi" }
```

### Comparing `curl_cffi-0.5.7/setup.py` & `curl_cffi-0.5.8.1/setup.py`

 * *Files identical despite different names*

