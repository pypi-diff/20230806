# Comparing `tmp/eciespy-0.3.9.tar.gz` & `tmp/eciespy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eciespy-0.3.9.tar", last modified: Sun Dec 13 14:02:20 2020, max compression
+gzip compressed data, was "eciespy-0.4.0.tar", max compression
```

## Comparing `eciespy-0.3.9.tar` & `eciespy-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1073 2020-12-13 14:02:09.412662 eciespy-0.3.9/LICENSE
--rw-r--r--   0        0        0    12554 2020-12-13 14:02:09.412662 eciespy-0.3.9/README.md
--rw-r--r--   0        0        0     1807 2020-12-13 14:02:09.416662 eciespy-0.3.9/ecies/__init__.py
--rw-r--r--   0        0        0     3075 2020-12-13 14:02:09.416662 eciespy-0.3.9/ecies/__main__.py
--rw-r--r--   0        0        0     5282 2020-12-13 14:02:09.416662 eciespy-0.3.9/ecies/utils.py
--rw-r--r--   0        0        0     1193 2020-12-13 14:02:09.416662 eciespy-0.3.9/pyproject.toml
--rw-r--r--   0        0        0    13831 2020-12-13 14:02:20.791982 eciespy-0.3.9/setup.py
--rw-r--r--   0        0        0    13785 2020-12-13 14:02:20.792923 eciespy-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-06 16:31:06.708458 eciespy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5382 2023-08-06 16:31:06.708458 eciespy-0.4.0/README.md
+-rw-r--r--   0        0        0     1865 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/__init__.py
+-rw-r--r--   0        0        0     3083 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/__main__.py
+-rw-r--r--   0        0        0      725 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/config.py
+-rw-r--r--   0        0        0       27 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/py.typed
+-rw-r--r--   0        0        0      403 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/utils/__init__.py
+-rw-r--r--   0        0        0     2902 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/utils/elliptic.py
+-rw-r--r--   0        0        0      826 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/utils/hex.py
+-rw-r--r--   0        0        0     3583 2023-08-06 16:31:06.708458 eciespy-0.4.0/ecies/utils/symmetric.py
+-rw-r--r--   0        0        0     1430 2023-08-06 16:31:06.708458 eciespy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6612 1970-01-01 00:00:00.000000 eciespy-0.4.0/PKG-INFO
```

### Comparing `eciespy-0.3.9/LICENSE` & `eciespy-0.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2020 Weiliang Li
+Copyright (c) 2018-2023 Weiliang Li
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `eciespy-0.3.9/ecies/__init__.py` & `eciespy-0.4.0/ecies/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 from typing import Union
 
 from coincurve import PrivateKey, PublicKey
-from ecies.utils import generate_key, hex2prv, hex2pub, encapsulate, decapsulate, aes_encrypt, aes_decrypt
 
-__all__ = ["encrypt", "decrypt"]
+from .config import ECIES_CONFIG
+from .utils import (
+    decapsulate,
+    encapsulate,
+    generate_key,
+    hex2pk,
+    hex2sk,
+    sym_decrypt,
+    sym_encrypt,
+)
+
+__all__ = ["encrypt", "decrypt", "ECIES_CONFIG"]
 
 
 def encrypt(receiver_pk: Union[str, bytes], msg: bytes) -> bytes:
     """
     Encrypt with receiver's secp256k1 public key
 
     Parameters
@@ -18,25 +28,29 @@
         Data to encrypt
 
     Returns
     -------
     bytes
         Encrypted data
     """
-    ephemeral_key = generate_key()
     if isinstance(receiver_pk, str):
-        receiver_pubkey = hex2pub(receiver_pk)
+        pk = hex2pk(receiver_pk)
     elif isinstance(receiver_pk, bytes):
-        receiver_pubkey = PublicKey(receiver_pk)
+        pk = PublicKey(receiver_pk)
     else:
         raise TypeError("Invalid public key type")
 
-    aes_key = encapsulate(ephemeral_key, receiver_pubkey)
-    cipher_text = aes_encrypt(aes_key, msg)
-    return ephemeral_key.public_key.format(False) + cipher_text
+    ephemeral_sk = generate_key()
+    ephemeral_pk = ephemeral_sk.public_key.format(
+        ECIES_CONFIG.is_ephemeral_key_compressed
+    )
+
+    sym_key = encapsulate(ephemeral_sk, pk)
+    encrypted = sym_encrypt(sym_key, msg)
+    return ephemeral_pk + encrypted
 
 
 def decrypt(receiver_sk: Union[str, bytes], msg: bytes) -> bytes:
     """
     Decrypt with receiver's secp256k1 private key
 
     Parameters
@@ -48,19 +62,18 @@
 
     Returns
     -------
     bytes
         Plain text
     """
     if isinstance(receiver_sk, str):
-        private_key = hex2prv(receiver_sk)
+        sk = hex2sk(receiver_sk)
     elif isinstance(receiver_sk, bytes):
-        private_key = PrivateKey(receiver_sk)
+        sk = PrivateKey(receiver_sk)
     else:
         raise TypeError("Invalid secret key type")
 
-    pubkey = msg[0:65]  # uncompressed pubkey's length is 65 bytes
-    encrypted = msg[65:]
-    ephemeral_public_key = PublicKey(pubkey)
+    key_size = ECIES_CONFIG.ephemeral_key_size
+    ephemeral_pk, encrypted = PublicKey(msg[0:key_size]), msg[key_size:]
 
-    aes_key = decapsulate(ephemeral_public_key, private_key)
-    return aes_decrypt(aes_key, encrypted)
+    sym_key = decapsulate(ephemeral_pk, sk)
+    return sym_decrypt(sym_key, encrypted)
```

### Comparing `eciespy-0.3.9/ecies/__main__.py` & `eciespy-0.4.0/ecies/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 | (____/\| (____/\___) (___| (____/\/\____) || )         | |
 (_______/(_______/\_______/(_______/\_______)|/          \_/
 
 """
 import argparse
 import sys
 
-from ecies import encrypt, decrypt
+from ecies import decrypt, encrypt
 from ecies.utils import generate_eth_key
 
 __description__ = "Elliptic Curve Integrated Encryption Scheme for secp256k1 in Python"
 
 
 def readablize(b: bytes) -> str:
     try:
@@ -64,44 +64,44 @@
         default=sys.stdout,
         help="encrypted or decrypted file, if not specified, it will write to stdout",
     )
 
     args = parser.parse_args()
     if args.generate:
         k = generate_eth_key()
-        prv, pub, addr = (
+        sk, pub, addr = (
             k.to_hex(),
             k.public_key.to_hex(),
             k.public_key.to_checksum_address(),
         )
-        print("Private: {}\nPublic: {}\nAddress: {}".format(prv, pub, addr))
+        print("Private: {}\nPublic: {}\nAddress: {}".format(sk, pub, addr))
         return
 
     if args.encrypt == args.decrypt:
         parser.print_help()
         return
 
     if not args.key:
         parser.print_help()
         return
 
     key = args.key.read().strip()
     if args.encrypt:
-        plaintext = args.data.read()
-        if isinstance(plaintext, str):
-            plaintext = plaintext.encode()
-        data = encrypt(key, plaintext)
+        plain_text = args.data.read()
+        if isinstance(plain_text, str):
+            plain_text = plain_text.encode()
+        data = encrypt(key, plain_text)
         if args.out == sys.stdout:
             data = data.hex()
     else:
-        ciphertext = args.data.read()
-        if isinstance(ciphertext, str):
+        cipher_text = args.data.read()
+        if isinstance(cipher_text, str):
             # if not bytes, suppose hex string
-            ciphertext = bytes.fromhex(ciphertext.strip())
-        data = decrypt(key, ciphertext)
+            cipher_text = bytes.fromhex(cipher_text.strip())
+        data = decrypt(key, cipher_text)
         if args.out == sys.stdout:
             # if binary data, print hex; if not, print utf8
             data = readablize(data)
 
     args.out.write(data)
```

### Comparing `eciespy-0.3.9/pyproject.toml` & `eciespy-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "eciespy"
 packages = [
   {include = "ecies"},
 ]
-version = "0.3.9"
+version = "0.4.0"
 # docs
 authors = ["Weiliang Li <to.be.impressive@gmail.com>"]
 description = "Elliptic Curve Integrated Encryption Scheme for secp256k1 in Python"
 license = "MIT"
 maintainers = ["Weiliang Li <to.be.impressive@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/ecies/py"
@@ -25,27 +25,39 @@
   "crypto",
   "elliptic curves",
   "ecies",
   "bitcoin",
   "ethereum",
   "cryptocurrency",
 ]
+# package data
+include = ["ecies/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
+
 # 3rd party
-coincurve = "^13.0"
-eth-keys = "^0.3.3"
-pycryptodome = "^3.9.9"
-
-[tool.poetry.dev-dependencies]
-black = {version = "^20.8b1", python = "^3.7"}
-flake8 = "^3.8"
-ipython = {version = "^7.19", python = "^3.7"}
-mypy = "^0.790"
+coincurve = ">=13,<19"
+eth-keys = "^0.4.0"
+pycryptodome = "^3.18.0"
+
+[tool.poetry.group.dev.dependencies]
+black = {version = "^23.7", python = "^3.9"}
+flake8 = {version = "^6.0.0", python = "^3.9"}
+ipython = {version = "^8.14.0", python = "^3.9"}
+mypy = "^1.4.1"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.scripts]
 eciespy = "ecies.__main__:main"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
+
+[tool.isort]
+multi_line_output = 3
+profile = "black"
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules"
```

