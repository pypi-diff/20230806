# Comparing `tmp/libnacl-2.0.0.tar.gz` & `tmp/libnacl-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libnacl-2.0.0.tar", max compression
+gzip compressed data, was "libnacl-2.1.0.tar", max compression
```

## Comparing `libnacl-2.0.0.tar` & `libnacl-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,84 @@
--rw-r--r--   0        0        0    11313 2023-08-04 21:07:41.149581 libnacl-2.0.0/LICENSE
--rw-r--r--   0        0        0     1729 2023-08-04 21:07:41.149581 libnacl-2.0.0/README.rst
--rw-r--r--   0        0        0    45854 2023-08-04 23:53:52.025381 libnacl-2.0.0/libnacl/__init__.py
--rw-r--r--   0        0        0     3955 2023-08-05 00:48:48.443540 libnacl-2.0.0/libnacl/aead.py
--rw-r--r--   0        0        0     2021 2023-08-04 21:56:41.178688 libnacl-2.0.0/libnacl/base.py
--rw-r--r--   0        0        0      950 2023-08-04 21:07:41.149581 libnacl-2.0.0/libnacl/blake.py
--rw-r--r--   0        0        0      889 2023-08-04 21:57:18.509004 libnacl-2.0.0/libnacl/dual.py
--rw-r--r--   0        0        0      933 2023-08-04 21:07:41.149581 libnacl-2.0.0/libnacl/encode.py
--rw-r--r--   0        0        0     3363 2023-08-04 21:57:09.148925 libnacl-2.0.0/libnacl/public.py
--rw-r--r--   0        0        0      916 2023-08-04 21:07:41.149581 libnacl-2.0.0/libnacl/sealed.py
--rw-r--r--   0        0        0     1540 2023-08-04 21:07:41.152914 libnacl-2.0.0/libnacl/secret.py
--rw-r--r--   0        0        0     1586 2023-08-04 22:01:56.531348 libnacl-2.0.0/libnacl/secret_easy.py
--rw-r--r--   0        0        0     1571 2023-08-04 22:01:13.470985 libnacl-2.0.0/libnacl/sign.py
--rw-r--r--   0        0        0     3327 2023-08-04 23:59:03.280546 libnacl-2.0.0/libnacl/utils.py
--rw-r--r--   0        0        0     1339 2023-08-05 04:18:26.525579 libnacl-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 libnacl-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11313 2023-08-06 21:16:41.578067 libnacl-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1729 2023-08-04 21:07:41.149581 libnacl-2.1.0/README.rst
+-rw-r--r--   0        0        0     6782 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/Makefile
+-rw-r--r--   0        0        0    10265 2023-08-06 21:22:44.769822 libnacl-2.1.0/doc/conf.py
+-rw-r--r--   0        0        0      465 2023-08-05 04:24:44.711489 libnacl-2.1.0/doc/index.rst
+-rw-r--r--   0        0        0     1046 2023-08-05 04:18:01.472025 libnacl-2.1.0/doc/topics/aead.rst
+-rw-r--r--   0        0        0     2822 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/dual.rst
+-rw-r--r--   0        0        0     1847 2023-08-06 21:16:41.578067 libnacl-2.1.0/doc/topics/kx.rst
+-rw-r--r--   0        0        0     3099 2023-08-04 21:32:25.685573 libnacl-2.1.0/doc/topics/public.rst
+-rw-r--r--   0        0        0      806 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/raw_generichash.rst
+-rw-r--r--   0        0        0      621 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/raw_hash.rst
+-rw-r--r--   0        0        0     2519 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/raw_public.rst
+-rw-r--r--   0        0        0     1147 2023-08-04 21:40:20.666825 libnacl-2.1.0/doc/topics/raw_sealed.rst
+-rw-r--r--   0        0        0     1860 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/raw_secret.rst
+-rw-r--r--   0        0        0     1826 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/raw_sign.rst
+-rw-r--r--   0        0        0      421 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.0.0.rst
+-rw-r--r--   0        0        0      615 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.1.0.rst
+-rw-r--r--   0        0        0      838 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.2.0.rst
+-rw-r--r--   0        0        0      176 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.3.0.rst
+-rw-r--r--   0        0        0      124 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.3.1.rst
+-rw-r--r--   0        0        0      151 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.3.2.rst
+-rw-r--r--   0        0        0      191 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.3.3.rst
+-rw-r--r--   0        0        0      259 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.3.4.rst
+-rw-r--r--   0        0        0      331 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.4.0.rst
+-rw-r--r--   0        0        0      192 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.4.1.rst
+-rw-r--r--   0        0        0      188 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.4.2.rst
+-rw-r--r--   0        0        0      507 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.4.3.rst
+-rw-r--r--   0        0        0      824 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.4.4.rst
+-rw-r--r--   0        0        0      327 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.4.5.rst
+-rw-r--r--   0        0        0      534 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.5.0.rst
+-rw-r--r--   0        0        0      576 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.5.1.rst
+-rw-r--r--   0        0        0      424 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.5.2.rst
+-rw-r--r--   0        0        0     1043 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.6.0.rst
+-rw-r--r--   0        0        0      225 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.6.1.rst
+-rw-r--r--   0        0        0      544 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.7.1.rst
+-rw-r--r--   0        0        0      328 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/1.7.rst
+-rw-r--r--   0        0        0      291 2023-08-04 22:42:31.495624 libnacl-2.1.0/doc/topics/releases/1.9.0.rst
+-rw-r--r--   0        0        0      292 2023-08-05 04:23:10.381011 libnacl-2.1.0/doc/topics/releases/2.0.0.rst
+-rw-r--r--   0        0        0      737 2023-08-06 21:18:39.859062 libnacl-2.1.0/doc/topics/releases/2.1.0.rst
+-rw-r--r--   0        0        0       96 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/releases/index.rst
+-rw-r--r--   0        0        0     1080 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/sealed.rst
+-rw-r--r--   0        0        0     1367 2023-08-05 04:15:34.274048 libnacl-2.1.0/doc/topics/secret.rst
+-rw-r--r--   0        0        0     1530 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/sign.rst
+-rw-r--r--   0        0        0     1562 2023-08-04 21:07:41.149581 libnacl-2.1.0/doc/topics/utils.rst
+-rw-r--r--   0        0        0    45854 2023-08-04 23:53:52.025381 libnacl-2.1.0/libnacl/__init__.py
+-rw-r--r--   0        0        0     3955 2023-08-05 00:48:48.443540 libnacl-2.1.0/libnacl/aead.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:16:41.578067 libnacl-2.1.0/libnacl/base.py
+-rw-r--r--   0        0        0      950 2023-08-04 21:07:41.149581 libnacl-2.1.0/libnacl/blake.py
+-rw-r--r--   0        0        0      889 2023-08-04 21:57:18.509004 libnacl-2.1.0/libnacl/dual.py
+-rw-r--r--   0        0        0      933 2023-08-04 21:07:41.149581 libnacl-2.1.0/libnacl/encode.py
+-rw-r--r--   0        0        0     2617 2023-08-06 21:16:41.578067 libnacl-2.1.0/libnacl/kx.py
+-rw-r--r--   0        0        0     3363 2023-08-04 21:57:09.148925 libnacl-2.1.0/libnacl/public.py
+-rw-r--r--   0        0        0      916 2023-08-04 21:07:41.149581 libnacl-2.1.0/libnacl/sealed.py
+-rw-r--r--   0        0        0     1540 2023-08-04 21:07:41.152914 libnacl-2.1.0/libnacl/secret.py
+-rw-r--r--   0        0        0     1586 2023-08-04 22:01:56.531348 libnacl-2.1.0/libnacl/secret_easy.py
+-rw-r--r--   0        0        0     1571 2023-08-04 22:01:13.470985 libnacl-2.1.0/libnacl/sign.py
+-rw-r--r--   0        0        0     3487 2023-08-06 21:16:41.578067 libnacl-2.1.0/libnacl/utils.py
+-rw-r--r--   0        0        0     1380 2023-08-06 21:22:03.166387 libnacl-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      549 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/runtests.py
+-rw-r--r--   0        0        0       24 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4374 2023-08-05 00:52:05.401774 libnacl-2.1.0/tests/unit/test_aead.py
+-rw-r--r--   0        0        0     4689 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_auth_verify.py
+-rw-r--r--   0        0        0     1476 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_blake.py
+-rw-r--r--   0        0        0     2311 2023-08-04 22:00:09.217111 libnacl-2.1.0/tests/unit/test_dual.py
+-rw-r--r--   0        0        0     1322 2023-08-06 21:16:41.578067 libnacl-2.1.0/tests/unit/test_kx.py
+-rw-r--r--   0        0        0     1587 2023-08-04 21:59:00.286530 libnacl-2.1.0/tests/unit/test_public.py
+-rw-r--r--   0        0        0      560 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_auth_sym.py
+-rw-r--r--   0        0        0      575 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_auth_sym_easy.py
+-rw-r--r--   0        0        0     1468 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_generichash.py
+-rw-r--r--   0        0        0      904 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_hash.py
+-rw-r--r--   0        0        0     3678 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_public.py
+-rw-r--r--   0        0        0     3629 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_random.py
+-rw-r--r--   0        0        0      924 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_secret.py
+-rw-r--r--   0        0        0      959 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_secret_easy.py
+-rw-r--r--   0        0        0     1379 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_raw_sign.py
+-rw-r--r--   0        0        0     3102 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_save.py
+-rw-r--r--   0        0        0     1046 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_seal.py
+-rw-r--r--   0        0        0      653 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_secret.py
+-rw-r--r--   0        0        0      680 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_secret_easy.py
+-rw-r--r--   0        0        0     4532 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_sign.py
+-rw-r--r--   0        0        0     1974 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_stream.py
+-rw-r--r--   0        0        0     2520 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_verify.py
+-rw-r--r--   0        0        0      734 2023-08-04 21:07:41.152914 libnacl-2.1.0/tests/unit/test_version.py
+-rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 libnacl-2.1.0/PKG-INFO
```

### Comparing `libnacl-2.0.0/LICENSE` & `libnacl-2.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {2014} Thomas S Hatch
+   Copyright {2023} Thomas S Hatch
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `libnacl-2.0.0/README.rst` & `libnacl-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/__init__.py` & `libnacl-2.1.0/libnacl/__init__.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/aead.py` & `libnacl-2.1.0/libnacl/aead.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/base.py` & `libnacl-2.1.0/libnacl/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,26 +12,34 @@
 class BaseKey(object):
     '''
     Include methods for key management convenience
     '''
     def __init__(self):
         self.sk_hex = self.hex_sk()
         self.pk_hex = self.hex_pk()
+        self.kx_sk_hex = self.hex_kx_sk()
+        self.kx_pk_hex = self.hex_kx_pk()
         self.vk_hex = self.hex_vk()
 
     def hex_sk(self):
         if hasattr(self, 'sk'):
             return libnacl.encode.hex_encode(self.sk)
-        else:
-            return ''
 
     def hex_pk(self):
         if hasattr(self, 'pk'):
             return libnacl.encode.hex_encode(self.pk)
 
+    def hex_kx_pk(self):
+        if hasattr(self, 'kx_pk'):
+            return libnacl.encode.hex_encode(self.kx_pk)
+
+    def hex_kx_sk(self):
+        if hasattr(self, 'kx_sk'):
+            return libnacl.encode.hex_encode(self.kx_sk)
+
     def hex_vk(self):
         if hasattr(self, 'vk'):
             return libnacl.encode.hex_encode(self.vk)
 
     def hex_seed(self):
         if hasattr(self, 'seed'):
             return libnacl.encode.hex_encode(self.seed)
@@ -39,20 +47,26 @@
     def for_json(self):
         '''
         Return a dictionary of the secret values we need to store.
         '''
         pre = {}
         sk = self.hex_sk()
         pk = self.hex_pk()
+        kx_sk = self.hex_kx_sk()
+        kx_pk = self.hex_kx_pk()
         vk = self.hex_vk()
         seed = self.hex_seed()
         if sk:
             pre['priv'] = sk.decode('utf-8')
         if pk:
             pre['pub'] = pk.decode('utf-8')
+        if kx_sk:
+            pre['kx_priv'] = kx_sk.decode('utf-8')
+        if kx_pk:
+            pre['kx_pub'] = kx_pk.decode('utf-8')
         if vk:
             pre['verify'] = vk.decode('utf-8')
         if seed:
             pre['sign'] = seed.decode('utf-8')
 
         return pre
```

### Comparing `libnacl-2.0.0/libnacl/blake.py` & `libnacl-2.1.0/libnacl/blake.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/dual.py` & `libnacl-2.1.0/libnacl/dual.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/encode.py` & `libnacl-2.1.0/libnacl/encode.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/public.py` & `libnacl-2.1.0/libnacl/public.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/sealed.py` & `libnacl-2.1.0/libnacl/sealed.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/secret.py` & `libnacl-2.1.0/libnacl/secret.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/secret_easy.py` & `libnacl-2.1.0/libnacl/secret_easy.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/sign.py` & `libnacl-2.1.0/libnacl/sign.py`

 * *Files identical despite different names*

### Comparing `libnacl-2.0.0/libnacl/utils.py` & `libnacl-2.1.0/libnacl/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     if 'priv' in key_data and 'sign' in key_data and 'pub' in key_data:
         return libnacl.dual.DualSecret(
                 libnacl.encode.hex_decode(key_data['priv']),
                 libnacl.encode.hex_decode(key_data['sign']))
     elif 'priv' in key_data and 'pub' in key_data:
         return libnacl.public.SecretKey(
                 libnacl.encode.hex_decode(key_data['priv']))
+    elif 'kx_priv' in key_data and 'kx_pub' in key_data:
+        return libnacl.kx.ExchangeKey(
+                libnacl.encode.hex_decode(key_data['kx_priv']))
     elif 'sign' in key_data:
         return libnacl.sign.Signer(
                 libnacl.encode.hex_decode(key_data['sign']))
     elif 'pub' in key_data:
         return libnacl.public.PublicKey(
                 libnacl.encode.hex_decode(key_data['pub']))
     elif 'verify' in key_data:
```

### Comparing `libnacl-2.0.0/pyproject.toml` & `libnacl-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libnacl"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python bindings for libsodium based on ctypes"
 authors = ["Thomas S Hatch <thatch45@gmail.com>"]
 license = "Apache-2.0"
 homepage="https://libnacl.readthedocs.org"
 repository="https://github.com/saltstack/libnacl"
 documentation="https://libnacl.readthedocs.org"
 readme = "README.rst"
@@ -23,15 +23,16 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Security :: Cryptography",
     ]
 include = [
-    { path = "test", format = "sdist" },
+    { path = "doc", format = "sdist" },
+    { path = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.4"
 
 
 [build-system]
```

### Comparing `libnacl-2.0.0/PKG-INFO` & `libnacl-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libnacl
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python bindings for libsodium based on ctypes
 Home-page: https://libnacl.readthedocs.org
 License: Apache-2.0
 Author: Thomas S Hatch
 Author-email: thatch45@gmail.com
 Requires-Python: >=3.4,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

