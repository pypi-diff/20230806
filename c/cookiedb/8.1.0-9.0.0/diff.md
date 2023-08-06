# Comparing `tmp/cookiedb-8.1.0.tar.gz` & `tmp/cookiedb-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiedb-8.1.0.tar", last modified: Tue Apr  4 01:09:46 2023, max compression
+gzip compressed data, was "cookiedb-9.0.0.tar", last modified: Sun Aug  6 19:02:23 2023, max compression
```

## Comparing `cookiedb-8.1.0.tar` & `cookiedb-9.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-04 01:09:46.791199 cookiedb-8.1.0/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    11357 2023-03-09 18:11:02.000000 cookiedb-8.1.0/LICENSE
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3031 2023-04-04 01:09:46.787198 cookiedb-8.1.0/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2087 2023-04-01 03:41:07.000000 cookiedb-8.1.0/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-04 01:09:46.783198 cookiedb-8.1.0/cookiedb/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      333 2023-04-04 01:03:30.000000 cookiedb-8.1.0/cookiedb/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1858 2023-03-10 17:10:49.000000 cookiedb-8.1.0/cookiedb/_document.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2970 2023-04-01 03:10:42.000000 cookiedb-8.1.0/cookiedb/_encrypt.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     5470 2023-04-04 01:02:41.000000 cookiedb-8.1.0/cookiedb/cookiedb.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1025 2023-04-01 03:41:07.000000 cookiedb-8.1.0/cookiedb/exceptions.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-04 01:09:46.787198 cookiedb-8.1.0/cookiedb.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3031 2023-04-04 01:09:46.000000 cookiedb-8.1.0/cookiedb.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      338 2023-04-04 01:09:46.000000 cookiedb-8.1.0/cookiedb.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-04-04 01:09:46.000000 cookiedb-8.1.0/cookiedb.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       19 2023-04-04 01:09:46.000000 cookiedb-8.1.0/cookiedb.egg-info/requires.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        9 2023-04-04 01:09:46.000000 cookiedb-8.1.0/cookiedb.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-04-04 01:09:46.791199 cookiedb-8.1.0/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1213 2023-04-04 01:05:33.000000 cookiedb-8.1.0/setup.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-04 01:09:46.787198 cookiedb-8.1.0/tests/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     5268 2023-04-01 03:41:07.000000 cookiedb-8.1.0/tests/test_database.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1123 2023-03-09 18:11:02.000000 cookiedb-8.1.0/tests/test_encrypt.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-08-06 19:02:23.934364 cookiedb-9.0.0/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)    11357 2023-06-17 22:36:53.000000 cookiedb-9.0.0/LICENSE
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3384 2023-08-06 19:02:23.934364 cookiedb-9.0.0/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2436 2023-06-19 02:53:42.000000 cookiedb-9.0.0/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-08-06 19:02:23.914364 cookiedb-9.0.0/cookiedb/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      660 2023-07-20 22:30:23.000000 cookiedb-9.0.0/cookiedb/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     7770 2023-08-06 15:45:15.000000 cookiedb-9.0.0/cookiedb/_document.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3656 2023-07-12 04:27:08.000000 cookiedb-9.0.0/cookiedb/_encrypt.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3720 2023-08-06 18:41:01.000000 cookiedb-9.0.0/cookiedb/_item.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3358 2023-07-30 21:49:40.000000 cookiedb-9.0.0/cookiedb/cookiedb.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1474 2023-07-19 03:14:38.000000 cookiedb-9.0.0/cookiedb/exceptions.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-08-06 19:02:23.926365 cookiedb-9.0.0/cookiedb.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3384 2023-08-06 19:02:23.000000 cookiedb-9.0.0/cookiedb.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      356 2023-08-06 19:02:23.000000 cookiedb-9.0.0/cookiedb.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-08-06 19:02:23.000000 cookiedb-9.0.0/cookiedb.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       19 2023-08-06 19:02:23.000000 cookiedb-9.0.0/cookiedb.egg-info/requires.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        9 2023-08-06 19:02:23.000000 cookiedb-9.0.0/cookiedb.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-08-06 19:02:23.938364 cookiedb-9.0.0/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1221 2023-08-06 16:19:41.000000 cookiedb-9.0.0/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-08-06 19:02:23.930364 cookiedb-9.0.0/tests/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3677 2023-08-06 18:56:02.000000 cookiedb-9.0.0/tests/test_database.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      971 2023-07-19 02:44:23.000000 cookiedb-9.0.0/tests/test_encrypt.py
```

### Comparing `cookiedb-8.1.0/LICENSE` & `cookiedb-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiedb-8.1.0/PKG-INFO` & `cookiedb-9.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: cookiedb
-Version: 8.1.0
+Version: 9.0.0
 Summary: CookieDB is a noSQL document database.
 Home-page: https://github.com/jaedsonpys/cookiedb
 Author: Jaedson Silva
 Author-email: jaedson.dev@proton.me
 License: Apache License
 Project-URL: License, https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE
 Project-URL: Documentation, https://jaedsonpys.github.io/cookiedb/
-Keywords: database,noSQL,document,JSON
+Keywords: database,noSQL,document,db,engine
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Database Engines/Servers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">CookieDB database</h1>
+<h1 align="center">CookieDB</h1>
+<p align="center">A safe, fast and simple database.</p>
 
 <p align="center" style="margin-bottom: 15px">
     <a href="https://github.com/jaedsonpys/cookiedb/releases">
-        <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/jaedsonpys/cookiedb?include_prereleases">
+        <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/jaedsonpys/cookiedb?include_prereleases&color=green&label=version">
     </a>
     <a href="https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/cookiedb">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/cookiedb?color=yellow">
     </a>
     <a href="https://pypi.org/project/cookiedb">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/cookiedb">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/cookiedb?color=blue">
     </a>
 </p>
 
-CookieDB is a noSQL database that uses the `document` model with all data encrypted, take advantage of the *performance and security* to create your projects that need a **quick storage** and are simple to use. Read the [CookieDB full documentation](https://jaedsonpys.github.io/cookiedb) to understand the methods available for creating, reading, updating and deleting data in the database.
+CookieDB is a noSQL database that uses the `document` model with all data encrypted using AES-256, take advantage of *performance and security* to create your projects that need **fast storage** and simple to use, where you have full control over the data. Read the [full CookieDB documentation](https://jaedsonpys.github.io/cookiedb) to understand the methods available to create, read, update, and delete data in the database.
 
 ## Getting started
 
 First, let's start by performing a quick installation of CookieDB using the PIP package manager:
 
 ```
 pip install cookiedb
 ```
 
+If you prefer, you can perform the installation manually using Git. See below how to do this:
+
+```
+git clone https://github.com/jaedsonpys/cookiedb.git
+cd cookiedb/
+python3 setup.py install
+```
+
+### Usage example
+
 Take a look at this **simple example of using** the database, where we create and get some data (the complete example can be found in [examples/example.py](https://github.com/jaedsonpys/cookiedb/blob/master/examples/example.py))
 
 ```python
 from cookiedb import CookieDB
 
 database = CookieDB('MyDatabase', key='secret')
 database.add('languages/python', {'name': 'Python', 'ext': '.py'})
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: cookiedb Version: 8.1.0 Summary: CookieDB is a
+Metadata-Version: 2.1 Name: cookiedb Version: 9.0.0 Summary: CookieDB is a
 noSQL document database. Home-page: https://github.com/jaedsonpys/cookiedb
 Author: Jaedson Silva Author-email: jaedson.dev@proton.me License: Apache
 License Project-URL: License, https://github.com/jaedsonpys/cookiedb/blob/
 master/LICENSE Project-URL: Documentation, https://jaedsonpys.github.io/
-cookiedb/ Keywords: database,noSQL,document,JSON Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Development Status :: 5 -
+cookiedb/ Keywords: database,noSQL,document,db,engine Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: System Administrators Classifier: Intended Audience ::
 Science/Research Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Database Engines/Servers Description-Content-
 Type: text/markdown License-File: LICENSE
-                        ****** CookieDB database ******
+                            ****** CookieDB ******
+                       A safe, fast and simple database.
 [GitHub_release_(latest_by_date_including_pre-releases)] [PyPI_-_License] [PyPI
                                  -_Downloads]
 CookieDB is a noSQL database that uses the `document` model with all data
-encrypted, take advantage of the *performance and security* to create your
-projects that need a **quick storage** and are simple to use. Read the
-[CookieDB full documentation](https://jaedsonpys.github.io/cookiedb) to
-understand the methods available for creating, reading, updating and deleting
-data in the database. ## Getting started First, let's start by performing a
-quick installation of CookieDB using the PIP package manager: ``` pip install
-cookiedb ``` Take a look at this **simple example of using** the database,
+encrypted using AES-256, take advantage of *performance and security* to create
+your projects that need **fast storage** and simple to use, where you have full
+control over the data. Read the [full CookieDB documentation](https://
+jaedsonpys.github.io/cookiedb) to understand the methods available to create,
+read, update, and delete data in the database. ## Getting started First, let's
+start by performing a quick installation of CookieDB using the PIP package
+manager: ``` pip install cookiedb ``` If you prefer, you can perform the
+installation manually using Git. See below how to do this: ``` git clone https:
+//github.com/jaedsonpys/cookiedb.git cd cookiedb/ python3 setup.py install ```
+### Usage example Take a look at this **simple example of using** the database,
 where we create and get some data (the complete example can be found in
 [examples/example.py](https://github.com/jaedsonpys/cookiedb/blob/master/
 examples/example.py)) ```python from cookiedb import CookieDB database =
 CookieDB('MyDatabase', key='secret') database.add('languages/python', {'name':
 'Python', 'ext': '.py'}) python_ext = database.get('languages/python/ext')
 print(f'Python extension: {python_ext}') ``` You can find more usage examples
 in the [examples/ directory](https://github.com/jaedsonpys/cookiedb/tree/
```

### Comparing `cookiedb-8.1.0/README.md` & `cookiedb-9.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-<h1 align="center">CookieDB database</h1>
+<h1 align="center">CookieDB</h1>
+<p align="center">A safe, fast and simple database.</p>
 
 <p align="center" style="margin-bottom: 15px">
     <a href="https://github.com/jaedsonpys/cookiedb/releases">
-        <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/jaedsonpys/cookiedb?include_prereleases">
+        <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/jaedsonpys/cookiedb?include_prereleases&color=green&label=version">
     </a>
     <a href="https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/cookiedb">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/cookiedb?color=yellow">
     </a>
     <a href="https://pypi.org/project/cookiedb">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/cookiedb">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/cookiedb?color=blue">
     </a>
 </p>
 
-CookieDB is a noSQL database that uses the `document` model with all data encrypted, take advantage of the *performance and security* to create your projects that need a **quick storage** and are simple to use. Read the [CookieDB full documentation](https://jaedsonpys.github.io/cookiedb) to understand the methods available for creating, reading, updating and deleting data in the database.
+CookieDB is a noSQL database that uses the `document` model with all data encrypted using AES-256, take advantage of *performance and security* to create your projects that need **fast storage** and simple to use, where you have full control over the data. Read the [full CookieDB documentation](https://jaedsonpys.github.io/cookiedb) to understand the methods available to create, read, update, and delete data in the database.
 
 ## Getting started
 
 First, let's start by performing a quick installation of CookieDB using the PIP package manager:
 
 ```
 pip install cookiedb
 ```
 
+If you prefer, you can perform the installation manually using Git. See below how to do this:
+
+```
+git clone https://github.com/jaedsonpys/cookiedb.git
+cd cookiedb/
+python3 setup.py install
+```
+
+### Usage example
+
 Take a look at this **simple example of using** the database, where we create and get some data (the complete example can be found in [examples/example.py](https://github.com/jaedsonpys/cookiedb/blob/master/examples/example.py))
 
 ```python
 from cookiedb import CookieDB
 
 database = CookieDB('MyDatabase', key='secret')
 database.add('languages/python', {'name': 'Python', 'ext': '.py'})
@@ -39,8 +50,8 @@
 # License
 
 ```
 Apache License
 Copyright 2023 Jaedson Silva
 ```
 
-This project uses the *Apache License*, anyone can use this project as long as the license conditions allow. [See more about the license](https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE).
+This project uses the *Apache License*, anyone can use this project as long as the license conditions allow. [See more about the license](https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE).
```

#### html2text {}

```diff
@@ -1,18 +1,22 @@
-                        ****** CookieDB database ******
+                            ****** CookieDB ******
+                       A safe, fast and simple database.
 [GitHub_release_(latest_by_date_including_pre-releases)] [PyPI_-_License] [PyPI
                                  -_Downloads]
 CookieDB is a noSQL database that uses the `document` model with all data
-encrypted, take advantage of the *performance and security* to create your
-projects that need a **quick storage** and are simple to use. Read the
-[CookieDB full documentation](https://jaedsonpys.github.io/cookiedb) to
-understand the methods available for creating, reading, updating and deleting
-data in the database. ## Getting started First, let's start by performing a
-quick installation of CookieDB using the PIP package manager: ``` pip install
-cookiedb ``` Take a look at this **simple example of using** the database,
+encrypted using AES-256, take advantage of *performance and security* to create
+your projects that need **fast storage** and simple to use, where you have full
+control over the data. Read the [full CookieDB documentation](https://
+jaedsonpys.github.io/cookiedb) to understand the methods available to create,
+read, update, and delete data in the database. ## Getting started First, let's
+start by performing a quick installation of CookieDB using the PIP package
+manager: ``` pip install cookiedb ``` If you prefer, you can perform the
+installation manually using Git. See below how to do this: ``` git clone https:
+//github.com/jaedsonpys/cookiedb.git cd cookiedb/ python3 setup.py install ```
+### Usage example Take a look at this **simple example of using** the database,
 where we create and get some data (the complete example can be found in
 [examples/example.py](https://github.com/jaedsonpys/cookiedb/blob/master/
 examples/example.py)) ```python from cookiedb import CookieDB database =
 CookieDB('MyDatabase', key='secret') database.add('languages/python', {'name':
 'Python', 'ext': '.py'}) python_ext = database.get('languages/python/ext')
 print(f'Python extension: {python_ext}') ``` You can find more usage examples
 in the [examples/ directory](https://github.com/jaedsonpys/cookiedb/tree/
```

### Comparing `cookiedb-8.1.0/cookiedb/_encrypt.py` & `cookiedb-9.0.0/cookiedb/_encrypt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# Copyright 2023 Jaedson Silva
+# 
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# 
+#     http://www.apache.org/licenses/LICENSE-2.0
+# 
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import struct
+from io import BytesIO
 from hashlib import sha256
 from secrets import token_bytes
 
 from Crypto.Cipher import AES
 from Crypto.Util import Padding
 from Crypto.Hash import HMAC, SHA256
 
@@ -36,63 +52,59 @@
         else:
             return True
     
     def encrypt(self, data: bytes) -> bytes:
         """Encrypt a data in bytes.
 
         The result will be a string in bytes containing
-        the length of the encrypted data, initialization
-        vector (IV), encrypted data and a MAC hash.
+        the initialization vector (IV), encrypted data
+        and a MAC hash.
 
         :param data: Any data in bytes
         :type data: bytes
         :return: Encrypted data
         :rtype: bytes
         """
 
         random_iv = token_bytes(16)
         padding_data = Padding.pad(data, AES.block_size)
 
         cipher = AES.new(self._encryption_key, AES.MODE_CBC, iv=random_iv)
         encrypted_data = cipher.encrypt(padding_data)
 
-        result = b''.join((len(data).to_bytes(4, 'big'), random_iv, encrypted_data))
-        return b''.join((result, self._get_hmac(result)))
+        enc_data_mac = self._get_hmac(encrypted_data)
+        enc_data_len = len(encrypted_data)
+        enc_data_mac_len = len(enc_data_mac)
+
+        pack_values = (enc_data_len, enc_data_mac_len,
+                       random_iv, encrypted_data, enc_data_mac)
+        result = struct.pack(f'<HH 16s {enc_data_len}s {enc_data_mac_len}s', *pack_values)
+
+        return result
 
     def decrypt(self, token: bytes) -> bytes:
         """Decrypt a token in bytes.
 
         :param token: Encrypted token
         :type token: bytes
-        :raises Exception: If token is invalid
-        :raises Exception: If token has a invalid signature
+        :raises InvalidTokenError: If token is invalid
+        :raises InvalidSignatureError: If token has a invalid signature
         :return: Decrypted data
         :rtype: bytes
         """
 
-        random_iv = token[4:20]
-        mac = token[-32:]
-        encrypted_data = token[20:-32]
+        token_buf = BytesIO(token)
+        enc_len, mac_len = struct.unpack('<HH', token_buf.read(4))
+        flen = (enc_len + mac_len) + 16
+        iv, encrypted_data, mac = struct.unpack(f'<16s {enc_len}s {mac_len}s', token_buf.read(flen))
 
-        cipher = AES.new(self._encryption_key, AES.MODE_CBC, iv=random_iv)
+        cipher = AES.new(self._encryption_key, AES.MODE_CBC, iv=iv)
         
-        if self._valid_hmac(mac, token[:-32]):
+        if self._valid_hmac(mac, encrypted_data):
             try:
                 decrypted_data = cipher.decrypt(encrypted_data)
                 unpad_data = Padding.unpad(decrypted_data, AES.block_size)
             except ValueError:
                 raise exceptions.InvalidTokenError('The token is invalid') from None
             return unpad_data
         else:
             raise exceptions.InvalidSignatureError('Token signature don\'t match')
-
-    def get_data_size(self, token: bytes) -> int:
-        """Return the encrypted data size.
-
-        :param token: Encrypted token
-        :type token: bytes
-        :return: Data size in bytes
-        :rtype: int
-        """
-
-        size = int.from_bytes(token[:4], 'big')
-        return size
```

### Comparing `cookiedb-8.1.0/cookiedb.egg-info/PKG-INFO` & `cookiedb-9.0.0/cookiedb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: cookiedb
-Version: 8.1.0
+Version: 9.0.0
 Summary: CookieDB is a noSQL document database.
 Home-page: https://github.com/jaedsonpys/cookiedb
 Author: Jaedson Silva
 Author-email: jaedson.dev@proton.me
 License: Apache License
 Project-URL: License, https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE
 Project-URL: Documentation, https://jaedsonpys.github.io/cookiedb/
-Keywords: database,noSQL,document,JSON
+Keywords: database,noSQL,document,db,engine
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Database Engines/Servers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">CookieDB database</h1>
+<h1 align="center">CookieDB</h1>
+<p align="center">A safe, fast and simple database.</p>
 
 <p align="center" style="margin-bottom: 15px">
     <a href="https://github.com/jaedsonpys/cookiedb/releases">
-        <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/jaedsonpys/cookiedb?include_prereleases">
+        <img alt="GitHub release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/jaedsonpys/cookiedb?include_prereleases&color=green&label=version">
     </a>
     <a href="https://github.com/jaedsonpys/cookiedb/blob/master/LICENSE" style="margin-right: 5px; margin-left: 5px">
-        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/cookiedb">
+        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/cookiedb?color=yellow">
     </a>
     <a href="https://pypi.org/project/cookiedb">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/cookiedb">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/cookiedb?color=blue">
     </a>
 </p>
 
-CookieDB is a noSQL database that uses the `document` model with all data encrypted, take advantage of the *performance and security* to create your projects that need a **quick storage** and are simple to use. Read the [CookieDB full documentation](https://jaedsonpys.github.io/cookiedb) to understand the methods available for creating, reading, updating and deleting data in the database.
+CookieDB is a noSQL database that uses the `document` model with all data encrypted using AES-256, take advantage of *performance and security* to create your projects that need **fast storage** and simple to use, where you have full control over the data. Read the [full CookieDB documentation](https://jaedsonpys.github.io/cookiedb) to understand the methods available to create, read, update, and delete data in the database.
 
 ## Getting started
 
 First, let's start by performing a quick installation of CookieDB using the PIP package manager:
 
 ```
 pip install cookiedb
 ```
 
+If you prefer, you can perform the installation manually using Git. See below how to do this:
+
+```
+git clone https://github.com/jaedsonpys/cookiedb.git
+cd cookiedb/
+python3 setup.py install
+```
+
+### Usage example
+
 Take a look at this **simple example of using** the database, where we create and get some data (the complete example can be found in [examples/example.py](https://github.com/jaedsonpys/cookiedb/blob/master/examples/example.py))
 
 ```python
 from cookiedb import CookieDB
 
 database = CookieDB('MyDatabase', key='secret')
 database.add('languages/python', {'name': 'Python', 'ext': '.py'})
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: cookiedb Version: 8.1.0 Summary: CookieDB is a
+Metadata-Version: 2.1 Name: cookiedb Version: 9.0.0 Summary: CookieDB is a
 noSQL document database. Home-page: https://github.com/jaedsonpys/cookiedb
 Author: Jaedson Silva Author-email: jaedson.dev@proton.me License: Apache
 License Project-URL: License, https://github.com/jaedsonpys/cookiedb/blob/
 master/LICENSE Project-URL: Documentation, https://jaedsonpys.github.io/
-cookiedb/ Keywords: database,noSQL,document,JSON Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Development Status :: 5 -
+cookiedb/ Keywords: database,noSQL,document,db,engine Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: System Administrators Classifier: Intended Audience ::
 Science/Research Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Database :: Database Engines/Servers Description-Content-
 Type: text/markdown License-File: LICENSE
-                        ****** CookieDB database ******
+                            ****** CookieDB ******
+                       A safe, fast and simple database.
 [GitHub_release_(latest_by_date_including_pre-releases)] [PyPI_-_License] [PyPI
                                  -_Downloads]
 CookieDB is a noSQL database that uses the `document` model with all data
-encrypted, take advantage of the *performance and security* to create your
-projects that need a **quick storage** and are simple to use. Read the
-[CookieDB full documentation](https://jaedsonpys.github.io/cookiedb) to
-understand the methods available for creating, reading, updating and deleting
-data in the database. ## Getting started First, let's start by performing a
-quick installation of CookieDB using the PIP package manager: ``` pip install
-cookiedb ``` Take a look at this **simple example of using** the database,
+encrypted using AES-256, take advantage of *performance and security* to create
+your projects that need **fast storage** and simple to use, where you have full
+control over the data. Read the [full CookieDB documentation](https://
+jaedsonpys.github.io/cookiedb) to understand the methods available to create,
+read, update, and delete data in the database. ## Getting started First, let's
+start by performing a quick installation of CookieDB using the PIP package
+manager: ``` pip install cookiedb ``` If you prefer, you can perform the
+installation manually using Git. See below how to do this: ``` git clone https:
+//github.com/jaedsonpys/cookiedb.git cd cookiedb/ python3 setup.py install ```
+### Usage example Take a look at this **simple example of using** the database,
 where we create and get some data (the complete example can be found in
 [examples/example.py](https://github.com/jaedsonpys/cookiedb/blob/master/
 examples/example.py)) ```python from cookiedb import CookieDB database =
 CookieDB('MyDatabase', key='secret') database.add('languages/python', {'name':
 'Python', 'ext': '.py'}) python_ext = database.get('languages/python/ext')
 print(f'Python extension: {python_ext}') ``` You can find more usage examples
 in the [examples/ directory](https://github.com/jaedsonpys/cookiedb/tree/
```

### Comparing `cookiedb-8.1.0/setup.py` & `cookiedb-9.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = reader.read()
 
 setup(
     author='Jaedson Silva',
     author_email='jaedson.dev@proton.me',
     name='cookiedb',
     description='CookieDB is a noSQL document database.',
-    version='8.1.0',
+    version='9.0.0',
     long_description_content_type='text/markdown',
     long_description=readme,
     license='Apache License',
     install_requires=['pycryptodome==3.17'],
     packages=['cookiedb'],
     url='https://github.com/jaedsonpys/cookiedb',
     project_urls={
@@ -26,9 +26,9 @@
         'Intended Audience :: System Administrators',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Topic :: Database :: Database Engines/Servers'
     ],
-    keywords=['database', 'noSQL', 'document', 'JSON']
+    keywords=['database', 'noSQL', 'document', 'db', 'engine']
 )
```

### Comparing `cookiedb-8.1.0/tests/test_encrypt.py` & `cookiedb-9.0.0/tests/test_encrypt.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,10 @@
         try:
             self._fake_enc.decrypt(self.encrypted)
         except cookiedb.exceptions.InvalidTokenError:
             self.assert_true(True)
         else:
             self.assert_true(False, message='Expected a InvalidTokenError exception')
 
-    def test_get_data_size(self):
-        data_size = self._enc.get_data_size(self.encrypted)
-        self.assert_expected(data_size, len(self._data))
-
 
 if __name__ == '__main__':
     bupytest.this()
```

