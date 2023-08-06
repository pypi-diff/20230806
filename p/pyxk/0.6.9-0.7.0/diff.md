# Comparing `tmp/pyxk-0.6.9.tar.gz` & `tmp/pyxk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.9.tar", last modified: Wed Aug  2 09:01:26 2023, max compression
+gzip compressed data, was "pyxk-0.7.0.tar", last modified: Sun Aug  6 01:41:47 2023, max compression
```

## Comparing `pyxk-0.6.9.tar` & `pyxk-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.603649 pyxk-0.6.9/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.9/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-08-02 09:01:26.603649 pyxk-0.6.9/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.9/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.9/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.9/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    23027 2023-08-02 02:02:37.000000 pyxk-0.6.9/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.9/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.9/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.9/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.603649 pyxk-0.6.9/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.9/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8876 2023-07-31 23:21:30.000000 pyxk-0.6.9/pyxk/m3u8/_initial.py
--rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.9/pyxk/m3u8/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.9/pyxk/m3u8/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    10217 2023-07-31 13:31:37.000000 pyxk-0.6.9/pyxk/m3u8/m3u8parse.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.603649 pyxk-0.6.9/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.9/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.9/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.9/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.9/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.9/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      558 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       62 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-08-02 09:01:26.603649 pyxk-0.6.9/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      898 2023-08-02 09:01:05.000000 pyxk-0.6.9/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.394596 pyxk-0.7.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.7.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-08-06 01:41:47.394596 pyxk-0.7.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.7.0/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.384596 pyxk-0.7.0/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.7.0/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.384596 pyxk-0.7.0/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.7.0/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    23869 2023-08-05 18:13:09.000000 pyxk-0.7.0/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.7.0/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.384596 pyxk-0.7.0/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.7.0/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.7.0/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.384596 pyxk-0.7.0/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.7.0/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8876 2023-07-31 23:21:30.000000 pyxk-0.7.0/pyxk/m3u8/_initial.py
+-rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.7.0/pyxk/m3u8/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.7.0/pyxk/m3u8/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    10217 2023-07-31 13:31:37.000000 pyxk-0.7.0/pyxk/m3u8/m3u8parse.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.384596 pyxk-0.7.0/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.7.0/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.7.0/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.7.0/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.7.0/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    22828 2023-08-06 01:38:01.000000 pyxk-0.7.0/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 01:41:47.384596 pyxk-0.7.0/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-08-06 01:41:47.000000 pyxk-0.7.0/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      558 2023-08-06 01:41:47.000000 pyxk-0.7.0/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-08-06 01:41:47.000000 pyxk-0.7.0/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-08-06 01:41:47.000000 pyxk-0.7.0/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       70 2023-08-06 01:41:47.000000 pyxk-0.7.0/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-08-06 01:41:47.000000 pyxk-0.7.0/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-08-06 01:41:47.394596 pyxk-0.7.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      974 2023-08-06 00:34:05.000000 pyxk-0.7.0/setup.py
```

### Comparing `pyxk-0.6.9/LICENSE` & `pyxk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/PKG-INFO` & `pyxk-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.9
+Version: 0.7.0
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.9/README.md` & `pyxk-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/aclient/client.py` & `pyxk-0.7.0/pyxk/aclient/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 
 from multidict import CIMultiDict
 from pyxk.aclient.typedef import (
     URL, Session, Response, EventLoop, CIMDict, Timeout, URLS
 )
 from pyxk.utils import (
-    LazyLoader, get_user_agent, default_headers
+    LazyLoader, get_user_agent, default_headers, chardet
 )
 
 copy = LazyLoader('copy', globals(), 'copy')
 yarl = LazyLoader('yarl', globals(), 'yarl')
 urllib = LazyLoader('urllib', globals(), 'urllib.parse')
 aiohttp = LazyLoader('aiohttp', globals(), 'aiohttp')
 logging = LazyLoader('logging', globals(), 'logging')
@@ -525,15 +525,15 @@
 
 
 async def xpath(
     self,
     query: str,
     text: Optional[str] = None,
     type: Optional[str] = None,
-    encoding: str = "utf8",
+    encoding: Optional[str] = None,
     base_url: Optional[str] = None,
     namespaces: Optional[Mapping[str, str]] = None,
     **kwargs: Any,
 ):
     """aiohttp.ClientResponse - selector.xpath
 
     :param self: aiohttp.ClientResponse 实例
@@ -544,91 +544,124 @@
     :param base_url: 为文档设置URL
     :param namespaces: `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
         for additional prefixes to those registered with `register_namespace(prefix, uri)`.
         Contrary to `register_namespace()`, these prefixes are not
         saved for future calls.
     :param kwargs: xpath kwargs
     """
-    if not text:
-        text = await self.text()
+    try:
+        if not text:
+            text = await self.text(encoding, errors='ignore')
+
+    except UnicodeError:
+        text = await self.read()
+        encoding = chardet(text).encoding
+        text = text.decode(encoding, errors="ignore")
+
     # selector
     sel = selector.Selector(
-        text=text, type=type, base_url=base_url, encoding=encoding, namespaces=namespaces
+        text=text,
+        type=type,
+        base_url=base_url,
+        encoding=encoding or self.get_encoding(),
+        namespaces=namespaces
     )
     # xpath
     return sel.xpath(query=query, **kwargs)
 
 
 async def css(
     self,
     query: str,
     text: Optional[str] = None,
     type: Optional[str] = None,
-    encoding: str = "utf8",
+    encoding: Optional[str] = None,
     base_url: Optional[str] = None,
     namespaces: Optional[Mapping[str, str]] = None,
 ):
     """aiohttp.ClientResponse - selector.css
 
     :param self: aiohttp.ClientResponse 实例
     :param query: xpath查询字符串
     :param text: str对象
     :param type: 文件类型 - "html"(default), "json", or "xml"
     :param encoding: text encoding
     :param base_url: 为文档设置URL
     :param namespaces:
-    `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
-    for additional prefixes to those registered with `register_namespace(prefix, uri)`.
-    Contrary to `register_namespace()`, these prefixes are not
-    saved for future calls.
+        `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
+        for additional prefixes to those registered with `register_namespace(prefix, uri)`.
+        Contrary to `register_namespace()`, these prefixes are not
+        saved for future calls.
     """
-    if not text:
-        text = await self.text()
+    try:
+        if not text:
+            text = await self.text(encoding, errors='ignore')
+
+    except UnicodeError:
+        text = await self.read()
+        encoding = chardet(text).encoding
+        text = text.decode(encoding, errors="ignore")
+
     # selector
     sel = selector.Selector(
-        text=text, type=type, base_url=base_url, encoding=encoding, namespaces=namespaces
+        text=text,
+        type=type,
+        base_url=base_url,
+        encoding=encoding or self.get_encoding(),
+        namespaces=namespaces
     )
     # css
     return sel.css(query=query)
 
 
 async def re(
     self,
     regex: str,
     text: Optional[str] = None,
     type: Optional[str] = None,
-    encoding: str = "utf8",
+    encoding: Optional[str] = None,
     base_url: Optional[str] = None,
     namespaces: Optional[Mapping[str, str]] = None,
     replace_entities: bool = True,
 ):
     """aiohttp.ClientResponse - selector.re
 
     :param self: aiohttp.ClientResponse 实例
     :param regex: 编译的正则表达式 或者 字符串
     :param text: str对象
     :param type: 文件类型 - "html"(default), "json", or "xml"
     :param encoding: text encoding
     :param base_url: 为文档设置URL
     :param namespaces:
-    `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
-    for additional prefixes to those registered with `register_namespace(prefix, uri)`.
-    Contrary to `register_namespace()`, these prefixes are not
-    saved for future calls.
+        `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
+        for additional prefixes to those registered with `register_namespace(prefix, uri)`.
+        Contrary to `register_namespace()`, these prefixes are not
+        saved for future calls.
     :param replace_entities:
-    By default, character entity references are replaced by their
-    corresponding character (except for ``&amp;`` and ``&lt;``).
-    Passing ``replace_entities`` as ``False`` switches off these
-    replacements.
+        By default, character entity references are replaced by their
+        corresponding character (except for ``&amp;`` and ``&lt;``).
+        Passing ``replace_entities`` as ``False`` switches off these
+        replacements.
     """
-    if not text:
-        text = await self.text()
+    try:
+        if not text:
+            text = await self.text(encoding, errors='ignore')
+
+    except UnicodeError:
+        text = await self.read()
+        encoding = chardet(text).encoding
+        text = text.decode(encoding, errors="ignore")
+
     # selector
     sel = selector.Selector(
-        text=text, type=type, base_url=base_url, encoding=encoding, namespaces=namespaces
+        text=text,
+        type=type,
+        base_url=base_url,
+        encoding=encoding or self.get_encoding(),
+        namespaces=namespaces
     )
     # re
     return sel.re(regex=regex, replace_entities=replace_entities)
 
 
 def urljoin(self, _url):
     """urljoin
@@ -637,16 +670,18 @@
     :param _url: url
     :return: url
     """
     if isinstance(_url, str):
         _url = yarl.URL(_url)
     elif not isinstance(_url, yarl.URL):
         return _url
+
     if _url.is_absolute():
         return _url
+
     return self.url.join(_url)
 
 
 def add_instance_method(response):
     """为异步response添加实例方法 - re, css, xpath, urljoin"""
     setattr(response, 're', MethodType(re, response))
     setattr(response, 'css', MethodType(css, response))
```

### Comparing `pyxk-0.6.9/pyxk/aclient/typedef.py` & `pyxk-0.7.0/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/aes/cryptor.py` & `pyxk-0.7.0/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/m3u8/_initial.py` & `pyxk-0.7.0/pyxk/m3u8/_initial.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/m3u8/downloader.py` & `pyxk-0.7.0/pyxk/m3u8/downloader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/m3u8/entry_point.py` & `pyxk-0.7.0/pyxk/m3u8/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/m3u8/m3u8parse.py` & `pyxk-0.7.0/pyxk/m3u8/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/requests/api.py` & `pyxk-0.7.0/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/requests/entry_point.py` & `pyxk-0.7.0/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/requests/sessions.py` & `pyxk-0.7.0/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/pyxk/utils.py` & `pyxk-0.7.0/pyxk/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from types import ModuleType
 from importlib import import_module
 from collections import namedtuple
 from typing import IO, Any, Union, Optional
 
 
 __all__ = [
-    'LazyLoader', 'runtime', 'runtime_coro', 'make_open',
+    'LazyLoader', 'runtime', 'runtime_coro', 'make_open', 'Chardet',
     'get_user_agent', 'default_headers', 'md5', 'hash256', 'normpath',
     'is_base64_from_regex', 'base64_conversion_bytes', 'rename_file', 'rename_folder', 'rename',
     'str_conversion_digit', 'human_playtime', 'pycode_conversion_lazy_loader', 'pyfile_conversion_lazy_loader',
     'units_conversion_from_byte', 'download_progress', 'tasks_progress', 'chardet', 'read_file_by_generator'
 ]
 
 
@@ -58,27 +58,39 @@
         return getattr(module, item)
 
     def __dir__(self):
         module = self._load()
         return dir(module)
 
 
+# 延迟加载模块
 os = LazyLoader('os', globals(), 'os')
 re = LazyLoader('re', globals(), 're')
 time = LazyLoader('time', globals(), 'time')
 base64 = LazyLoader('base64', globals(), 'base64')
 hashlib = LazyLoader('hashlib', globals(), 'hashlib')
 difflib = LazyLoader('difflib', globals(), 'difflib')
+_chardet = LazyLoader('_chardet', globals(), 'chardet')
 warnings = LazyLoader('warnings', globals(), 'warnings')
 functools = LazyLoader('functools', globals(), 'functools')
 itertools = LazyLoader('itertools', globals(), 'itertools')
 collections = LazyLoader('collections', globals(), 'collections')
 _console = LazyLoader('_console', globals(), 'rich.console')
 
 
+# 命名元组
+_md5_nametuple = namedtuple('MD5NameTuple', 'ciphertext,plaintext')
+_hash256_nametuple = namedtuple('Hash256NameTuple', 'ciphertext,plaintext')
+_base64_nametuple = namedtuple('Base64NameTuple', 'result,is_base64')
+_rename_nametuple = namedtuple('RenameNameTuple', 'result,dirname,basename')
+_str_conversion_digit_nametuple = namedtuple('StrConversionDigitNameTuple', 'result,raw,is_digit')
+_units_conversion_nametuple = namedtuple('UnitsConversionNameTuple', 'result,raw,units')
+_chardet_nametuple = namedtuple('ChardetNameTuple', 'encoding,language,confidence')
+
+
 def runtime(func):
     """装饰器: 计算函数运行时间"""
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         con = _console.Console()
         start_time = time.perf_counter()
@@ -113,15 +125,15 @@
     """内置方法open装饰器 - 文件模式 w/a 下，创建不存在的目录"""
 
     @functools.wraps(func)
     def wrapper(
         file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None
     ) -> IO:
         if not isinstance(mode, str):
-            raise TypeError(f"{func.__name__}() argument 'mode' must be str, not {type(mode).__name__!r}")
+            raise TypeError(f"{func.__name__}() argument the 'mode' type must be str, got: {type(mode)}")
 
         # collections.Counter 统计可迭代对象 每项出现的次数 & itertools.product 求多个可迭代对象的笛卡尔积
         mode_list = [collections.Counter(i + j) for i, j in itertools.product('wa', ('b', 'b+', '', '+'))]
         if collections.Counter(mode) in mode_list:
             os.makedirs(os.path.dirname(file), exist_ok=True)
 
         # 二进制模式下 encoding=None
@@ -132,26 +144,21 @@
         return func(file, mode, buffering, encoding, errors, newline, closefd, opener)
     return wrapper
 
 
 make_open = _make_open(io.open)
 
 
-def get_user_agent(ua: Optional[str] = 'android', overwrite: bool = False) -> Union[str, Any]:
+def get_user_agent(ua: Optional[str] = 'android', overwrite: bool = False) -> str:
     """获取 UserAgent，默认 Android
 
     :param ua: 模糊查找内置字典User-Agent (android, windows, mac, iphone, ipad, symbian, apad)
     :param overwrite: 若为True, 直接返回  User-Agent
     :return: str
     """
-    # 重写 UserAgent
-    if overwrite:
-        return str(ua)
-
-    # UserAgent 全部字典
     user_agent_dict = {
         'android': 'Mozilla/5.0 (Linux; Android 11; Pixel 5) AppleWebKit/537.36 (KHTML, like Gecko) '
                    'Chrome/90.0.4430.91 Mobile Safari/537.36',
         'windows': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
                    'Chrome/86.0.4240.198 Safari/537.36',
         'mac': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) '
                'Chrome/86.0.4240.198 Safari/537.36',
@@ -162,43 +169,54 @@
         'symbian': 'Mozilla/5.0 (Symbian/3; Series60/5.2 NokiaN8-00/012.002; Profile/MIDP-2.1 Configuration/CLDC-1.1 ) '
                    'AppleWebKit/533.4 (KHTML, like Gecko) NokiaBrowser/7.3.0 Mobile Safari/533.4 3gpp-gba',
         'apad': 'Mozilla/5.0 (Linux; Android 11; Phh-Treble vanilla Build/RQ3A.211001.001;) '
                 'AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/90.0.4430.91 Safari/537.36',
     }
 
     if not isinstance(ua, str):
+        if ua is not None:
+            raise TypeError(f"'ua' type must be a str, got: {type(ua)}")
+
         return user_agent_dict['android']
 
+    # 重写 UserAgent
+    if overwrite:
+        return ua
+
     # 模糊查找 UserAgent
     ua = difflib.get_close_matches(ua.lower(), user_agent_dict.keys(), 1)
     if not ua:
         return user_agent_dict['android']
     return user_agent_dict[ua[0]]
 
 
-def default_headers(ua: Optional[str] = 'android'):
+def default_headers(ua: Optional[str] = 'android', **kwargs) -> dict:
     """Headers
 
     :param ua: user-agent
     :return: dict -> {'User-Agent': str}
     """
-    return {'User-Agent': get_user_agent(ua)}
+    _headers = {'User-Agent': get_user_agent(ua)}
+    _headers.update(kwargs)
+    return _headers
 
 
-def md5(plaintext: Union[str, bytes], encoding: str = 'utf-8', default: Any = None):
+def md5(
+    plaintext: Union[str, bytes],
+    encoding: str = 'utf-8',
+    default: Any = None
+) -> _md5_nametuple:
     """MD5加密
 
     :param plaintext: 需加密明文
     :param encoding: plaintext编码
     :param default: ciphertext默认值
     :return: tuple -> (plaintext: 'plaintext', ciphertext: 'ciphertext')
     """
-
-    _tuple = namedtuple('MD5NameTuple', 'ciphertext,plaintext')
-    result = _tuple(default, plaintext)
+    result = _md5_nametuple(default, plaintext)
 
     if not isinstance(plaintext, (str, bytes)):
         return result
 
     # plaintext type str
     if isinstance(plaintext, str):
         plaintext = plaintext.encode(encoding=encoding)
@@ -206,24 +224,28 @@
     # md5加密
     result = result._replace(
         ciphertext=hashlib.md5(plaintext).hexdigest()
     )
     return result
 
 
-def hash256(plaintext: Union[str, bytes], encoding: str = 'utf-8', default: Any = None):
+def hash256(
+    plaintext: Union[str, bytes],
+    encoding: str = 'utf-8',
+    default: Any = None
+) -> _hash256_nametuple:
     """HASH_256加密
 
     :param plaintext: 需加密明文
     :param encoding: plaintext编码
     :param default: ciphertext默认值
     :return: tuple -> (plaintext: 'plaintext', ciphertext: 'ciphertext')
     """
-    _tuple = namedtuple('Hash256NameTuple', 'ciphertext,plaintext')
-    result = _tuple(default, plaintext)
+
+    result = _hash256_nametuple(default, plaintext)
 
     if not isinstance(plaintext, (str, bytes)):
         return result
 
     # plaintext type str
     if isinstance(plaintext, str):
         plaintext = plaintext.encode(encoding=encoding)
@@ -246,28 +268,32 @@
         pattern_from_bytes = re.compile(rb'^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$')
         return bool(pattern_from_bytes.match(data))
 
     # base64 数据类型 正则表达式判断
     if isinstance(data, str):
         pattern_from_string = re.compile(r'^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$')
         return bool(pattern_from_string.match(data))
+
     # str 或 bytes 以外类型返回 False
     return False
 
 
-def base64_conversion_bytes(data: Union[str, bytes], encoding: str = 'utf-8', default: Any = None):
+def base64_conversion_bytes(
+    data: Union[str, bytes],
+    encoding: str = 'utf-8',
+    default: Any = None
+) -> _base64_nametuple:
     """base64数据类型 转化为bytes
 
     :param data: data: data
     :param encoding: data数据编码
     :param default: 返回默认值
     :return: tuple -> (result: 'result', is_base64: 'is_base64')
     """
-    _tuple = namedtuple('Base64NameTuple', 'result,is_base64')
-    result = _tuple(default, False)
+    result = _base64_nametuple(default, False)
 
     if (
         not isinstance(data, (str, bytes))
         or not is_base64_from_regex(data)
     ):
         return result
 
@@ -282,20 +308,20 @@
 
     return result
 
 
 def normpath(_path) -> str:
     """规范文件路径"""
     if not isinstance(_path, str):
-        raise TypeError(f'_path must be a str, got {type(_path).__name__!r}')
+        raise TypeError(f"'_path' type must be a str, got: {type(_path)}")
 
     return os.path.normpath(_path.strip()).replace('\\', '/')
 
 
-def rename_file(file: str, suffix: Optional[str] = None, create: bool = False):
+def rename_file(file: str, suffix: Optional[str] = None, create: bool = False) -> _rename_nametuple:
     """重命名本地存在的文件
 
     :param file: 文件路径
     :param suffix: 文件后缀名
     :param create: 创建文件
     :return: tuple -> (result, dirname, basename)
     """
@@ -317,70 +343,67 @@
     # 拼接完整file
     if not file.endswith(suffix):
         file += suffix
 
     # 重命名文件
     def _rename(f):
         """rename a file"""
-        _tuple = namedtuple('RenameFileNameTuple', 'result,dirname,basename')
 
         if create:
             from pathlib import Path
             Path(f).touch()
-        return _tuple(f, *os.path.split(f))
+        return _rename_nametuple(f, *os.path.split(f))
 
     if not os.path.isfile(file):
         return _rename(file)
 
     for index in itertools.count(1):
         newfile = file.removesuffix(suffix) + f'.{index}{suffix}'
         if not os.path.isfile(newfile):
             return _rename(newfile)
 
 
 rename = rename_file
 
 
-def rename_folder(folder: str, create: bool = False):
+def rename_folder(folder: str, create: bool = False) -> _rename_nametuple:
     """重命名本地存在的文件夹
 
     :param folder: 文件夹路径
     :param create: 创建文件夹
     :return: Tuple(result, dirname, basename)
     """
     # 获取folder绝对路径
     folder = normpath(os.path.abspath(folder))
 
     def get_folder(f):
         """获取重命名文件数据"""
-        _tuple = namedtuple('RenameFolderNameTuple', 'result,dirname,basename')
 
         if create:
             os.makedirs(f, exist_ok=True)
-        return _tuple(f, *os.path.split(f))
+        return _rename_nametuple(f, *os.path.split(f))
 
     if not os.path.isdir(folder):
         return get_folder(folder)
 
     # 重命名folder
     for index in itertools.count(1):
         new_folder = folder + f".{index}"
         if not os.path.isdir(new_folder):
             return get_folder(new_folder)
 
 
-def str_conversion_digit(target: Union[str, int, float], default: Any = None):
+def str_conversion_digit(target: Union[str, int, float], default: Any = None) -> _str_conversion_digit_nametuple:
     """字符串转换为数字
 
     :param target: 需要转换的目标
     :param default: 返回默认值
     :return: tuple -> (result: digits, raw, is_digit: bool)
     """
-    _tuple = namedtuple('StrConversionDigitNameTuple', 'result,raw,is_digit')
-    result = _tuple(default, target, False)
+    result = _str_conversion_digit_nametuple(default, target, False)
 
     # target type = `int` or `float`
     if isinstance(target, (int, float)):
         return result._replace(
             is_digit=True, result=target
         )
 
@@ -400,15 +423,15 @@
     if _result["is_digits"]:
         result = result._replace(
             is_digit=True, result=_result["type"](target)
         )
     return result
 
 
-def human_playtime(playtime: Union[str, int, float], default: Any = None):
+def human_playtime(playtime: Union[str, int, float], default: Any = None) -> Union[str, Any]:
     """人类直观时间展示
 
     :param playtime: 传入一个时间(秒), 返回人类能理解的时间格式
     :param default: 返回默认值
     :return: str
     """
     digit = str_conversion_digit(playtime)
@@ -421,20 +444,23 @@
 
     hour, second = divmod(playtime, 3600)
     minute, second = divmod(second, 60)
 
     return f"{symbol}{hour}:{minute:0>2}:{second:0>2}"
 
 
-def pycode_conversion_lazy_loader(string: str):
+def pycode_conversion_lazy_loader(string: str) -> str:
     """python代码中的导入模块转换为懒加载
 
     :param string: python代码
     :return: str
     """
+    if not isinstance(string, str):
+        raise TypeError(f"'string' type must be a str, got: {type(string)}")
+
     def repl_string(match):
         """替换懒加载"""
         match_dict, import_name, alias = match.groupdict(), None, None
         repl = '{alias} = LazyLoader("{alias}", globals(), "{import_name}")'
 
         # from导入
         if match_dict["from_name"]:
@@ -456,44 +482,42 @@
         r'^from\s+?(?P<from_name>\S+)\s+?import\s+?(?P<from_import_name>\S+)'
         r'\s*?(as\s+?(?P<from_import_alias>\S+))?$',
         r'^import\s+?(?P<import_name>\S+)(\s+?as\s+(?P<import_alias>\S+?))?\s*?$',
     ]
     return re.sub(pattern='|'.join(pattern), repl=repl_string, string=string, flags=re.M)
 
 
-def pyfile_conversion_lazy_loader(read_file: str, write_file: str, encoding: Optional[str] = None):
+def pyfile_conversion_lazy_loader(read_file: str, write_file: str, encoding: Optional[str] = None) -> None:
     """python文件中的导入模块转换为懒加载
 
     :param read_file: 读取python代码文件
     :param write_file: 写入转换后的python代码文件
     :param encoding: 文件编码
     """
     with open(read_file, "r", encoding=encoding) as read_file_obj:
         content = pycode_conversion_lazy_loader(read_file_obj.read())
     with open(write_file, "w", encoding=encoding) as write_file_obj:
         write_file_obj.write(content)
 
 
-def units_conversion_from_byte(target: Union[str, int, float], default: Any = None):
+def units_conversion_from_byte(target: Union[str, int, float], default: Any = None) -> _units_conversion_nametuple:
     """字节单位自动换算
 
     :param target: 换算目标(Bytes)
     :param default: 返回默认值
     :return: tuple -> (result, raw, units)
     """
-    _tuple = namedtuple('UnitsConversionNameTuple', 'result,raw,units')
-    result = _tuple(default, target, None)
+    result = _units_conversion_nametuple(default, target, None)
     _temp = str_conversion_digit(target)
 
     if not _temp.is_digit:
         return result
 
     target = abs(_temp.result)
     target_units = 'Bytes'
-    del _temp
 
     units_dict = {
         'Bytes': 1, 'KB': 1024, 'MB': 1024,
         'GB': 1024, 'TB': 1024, 'PB': 1024,
         'EB': 1024, 'ZB': 1024, 'YB': 1024, 'BB': 1024
     }
 
@@ -507,35 +531,94 @@
         units=target_units,
         result= f'{round(target, 2)}{target_units}'
 
     )
     return result
 
 
-def chardet(byte_str: bytes, **kwargs):
+class Chardet:
+    """字符集编码探测"""
+
+    def __init__(self, should_rename_legacy: bool = False):
+        """Chardet初始化
+
+        :param should_rename_legacy: should_rename_legacy
+        """
+        # 编码探测器
+        self.detector = _chardet.UniversalDetector(
+            should_rename_legacy=should_rename_legacy
+        )
+
+    @classmethod
+    def chardet(
+        cls,
+        byte_str: Union[bytes, bytearray],
+        should_rename_legacy: bool = False
+    ) -> _chardet_nametuple:
+        """字符编码探测
+
+        :param byte_str: bytes数据
+        :param should_rename_legacy: should_rename_legacy:
+        :return: tuple -> (encoding: str, language: str, confidence: float)
+        """
+        # 无效数据类型
+        if not isinstance(byte_str, bytearray):
+            if not isinstance(byte_str, bytes):
+                raise TypeError(
+                    f"'byte_str' type must be a bytes or bytearray, got: {type(byte_str)}"
+                )
+            byte_str = bytearray(byte_str)
+
+        self = cls(
+            should_rename_legacy=should_rename_legacy
+        )
+        self.feed(byte_str)
+        return self.close()
+
+    def feed(self, byte_str: Union[bytes, bytearray]) -> None:
+        self.detector.feed(bytearray(byte_str))
+
+    def reset(self) -> None:
+        self.detector.reset()
+
+    @property
+    def done(self) -> bool:
+        return self.detector.done
+
+    def close(self) -> _chardet_nametuple:
+        """字符集编码结果
+
+        :return: tuple -> (encoding: str, language: str, confidence: float)
+        """
+        ret = self.detector.close()
+        return _chardet_nametuple(
+            encoding=ret.get("encoding"),
+            language=ret.get("language"),
+            confidence=ret.get("confidence")
+        )
+
+    def __enter__(self):
+        self.reset()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.reset()
+
+
+def chardet(
+    byte_str: Union[bytes, bytearray],
+    should_rename_legacy: bool = False
+) -> _chardet_nametuple:
     """字符编码判断
 
     :param byte_str: bytes数据
-    :param kwargs: kwargs
+    :param should_rename_legacy: should_rename_legacy
     :return: tuple -> (encoding: str, language: str, confidence: float)
     """
-    try:
-        import chardet as _chardet
-    except ImportError:
-        import charset_normalizer as _chardet
-
-    _tuple = namedtuple('ChardetNameTuple', 'encoding,language,confidence')
-    result = _chardet.detect(byte_str=byte_str, **kwargs)
-
-    return _tuple(
-        encoding=result.get('encoding'),
-        language=result.get('language'),
-        confidence=result.get('confidence')
-    )
-
+    return Chardet.chardet(byte_str, should_rename_legacy)
 
 
 def download_progress(
     *,
     transient: bool = False,
     console: object = None,
     text_column: Optional[str] = '[progress.description]{task.description}',
```

### Comparing `pyxk-0.6.9/pyxk.egg-info/PKG-INFO` & `pyxk-0.7.0/pyxk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.9
+Version: 0.7.0
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.9/pyxk.egg-info/SOURCES.txt` & `pyxk-0.7.0/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.9/setup.py` & `pyxk-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as read_file_obj:
     long_description = read_file_obj.read()
 
 setuptools.setup(
     name='pyxk',
-    version='0.6.9',
+    version='0.7.0',
     author='kai139',
     install_requires=[
-        'requests', 'pycryptodome', 'rich', 'm3u8', 'aiohttp', 'aiofiles', 'click', 'parsel'
+        'requests',
+        'pycryptodome',
+        'rich',
+        'm3u8',
+        'aiohttp',
+        'aiofiles',
+        'click',
+        'parsel',
+        'chardet',
     ],
     entry_points={
         'console_scripts': [
             'm3u8 = pyxk.m3u8.entry_point:main',
             'req = pyxk.requests.entry_point:main'
         ],
     },
```

