# Comparing `tmp/ashcrypt-3.1.9.tar.gz` & `tmp/ashcrypt-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.9.tar", last modified: Fri Aug  4 13:04:05 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.2.0.tar", last modified: Sun Aug  6 11:28:23 2023, max compression
```

## Comparing `ashcrypt-3.1.9.tar` & `ashcrypt-3.2.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39593 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/sandbox/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/utils/consts/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/consts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/exceptions/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/exceptions/fixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt/utils/safepack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/safepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/safepack/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/safepack/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/ashcrypt/utils/safepack/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 13:04:05.000000 ashcrypt-3.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-04 13:03:52.000000 ashcrypt-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/sandbox/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/unittests/test_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/consts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/exceptions/fixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:28:23.000000 ashcrypt-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-06 11:28:12.000000 ashcrypt-3.2.0/setup.py
```

### Comparing `ashcrypt-3.1.9/PKG-INFO` & `ashcrypt-3.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.9
+Version: 3.2.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.9/README.md` & `ashcrypt-3.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 **App :** 
 <br>Full-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
 <br>check [GUI](https://github.com/AshGw/AES-256#gui) header for more info.
 
 **Library :** 
 <br>A simple, secure, and developer-oriented library for performing encryption and decryption operations on data using the AES-256 (CBC) encryption algorithm.
 <br>The core of the library is the module `crypt`
-It offers cryptographic capabilities and top security measures to safeguard
+It offers cryptographic capabilities and security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 
 
 ### For Developers ###
 The project uses `crypt` module to ensure secure data encryption and decryption for files and text while keeping it very easy and simple to use .
 View the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
-It also incorporates a database module that serve the same purpose which is allowing for key management & storage of classified content in a secure, 
+It also incorporates a database module which is there to allow key management & storage of classified content in a secure, 
 safe and simple manner.
 
-<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries with built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
 
 ## Installation ##
 ### If you want to use it as a library ###
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
 pip install --upgrade pip 
@@ -61,49 +61,44 @@
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
 python -m ashcrypt.gui
 ```
 
 ## `crypt` Module ##
-The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring security and 
+The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate the performance and reliability for data encryption and decryption operations  while ensuring security and 
 confidentiality.
 
-<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+<br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
-<br>You can check the [unittesting file](ashcrypt/unittests/unittest_crypt.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
-<br>This will output a string type key (hex), you can choose to render your preferred key length:
+<br>This will output a string type key (hex), you can choose to render your preferred key length too:
 ```python
 mainkey = Enc.genkey(desired_bytes=64) # 512-bit long key
 ```
 ```python
 mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
 ```
-The message can be of type string or bytes.
-<br>Normal string message :  
+The message can be of type str or bytes.
 ```python 
-message = 'Hello There'
+message = 'Hello There'  # str
+message = b'Hello There' # bytes
 ```
-or a normal bytes message 
-```python
-message = b'Hello There'
-```
-or string URL safe encrypted message ( to decrypt ): 
+an encrypted message ( to decrypt ): 
 ```python
 message = 'ZEfikRiNQ4EE1y5E-Qn4gQbo8goVpWLPstqTlgWtoRq1CK_oeMz4oelCYNpM-NZyzSIKk7DazkAUO9HcZJzWWMXR6zqRjNTN-c1Q6vRWSkj1g20oL6JbzUvEJL3xvY2-Fye1simoOAr7YP5YHAnSYAAAADIA0juak_JYQnzXQ-apJ8azahvngigFrHRg142g7OqvfA=='
 ```
-or bytes type encrypted message ( to decrypt ):
+or bytes encrypted message ( to decrypt ):
 ```python
 message = b'dG\xe2\x91\x18\x8dC\x81\x04\xd7.D\xf9\t\xf8\x81\x06\xe8\xf2\n\x15\xa5b\xcf\xb2\xda\x93\x96\x05\xad\xa1\x1a\xb5\x08\xaf\xe8x\xcc\xf8\xa1\xe9B`\xdaL\xf8\xd6r\xcd"\n\x93\xb0\xda\xce@\x14;\xd1\xdcd\x9c\xd6X\xc5\xd1\xeb:\x91\x8c\xd4\xcd\xf9\xcdP\xea\xf4VJH\xf5\x83m(/\xa2[\xcdK\xc4$\xbd\xf1\xbd\x8d\xbe\x17\'\xb5\xb2)\xa88\n\xfb`\xfeX\x1c\t\xd2`\x00\x00\x002\x00\xd2;\x9a\x93\xf2XB|\xd7C\xe6\xa9\'\xc6\xb3j\x1b\xe7\x82(\x05\xact`\xd7\x8d\xa0\xec\xea\xaf|'
 ```
 3) Now pass the arguments accordingly. If you have a normal message and you try to decrypt it, an Exception will be raised so pass the arguments to the right classes. 
 <br><br>So first create an instance of either the `Enc` or `Dec` class. 
 <br>Here I chose to encrypt a message 
 ```python
@@ -116,19 +111,15 @@
 output = a.encrypt(get_bytes=True)
 ```
 you can also encrypt to a URL safe string
 ```python
 output = a.encrypt()
 ```
 <br> 
-The same logic applies to the decryption process simply switch `Enc` with `Dec` and `encrypt()` to `decrypt()`
-That simple, that's it.
-
-
-
+The same logic applies to the decryption process.
 
 ## Features ## 
 - AES 256 CBC mode 
 - Generates a randomly secure 256-bit main key 
 - Derives the HMAC and the AES key from the mainkey using bcrypt's KDFs with a configurable number of iterations with :
     - Salt : Random 128 bit value is generated  each time and passed to the KDF to generate the AES key
     - Pepper : Random 128 bit value is generated  each time and passed to the KDF to generate the HMAC
@@ -136,16 +127,15 @@
 - HMAC : 256 bit hashed using SHA256
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In `crypt` module the key is flexible it must be **at least** 256-bit , so can go higher if you want ( although for `textcrypt` and `filecrypt` you have to use a 256 bit long key )
-- Encrypting to a string has URL-safe string representation 
+- For the `crypt` module the key is flexible it must **at least** be 256-bit , so can go higher if you want ( although for `textcrypt` and `filecrypt` you have to use a 256 bit long key )
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50 ( which is secure enough ), the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
@@ -166,15 +156,15 @@
 b.encrypt()
 print(time.perf_counter() - t2)
 ```
 
 ## `filecrypt` ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
-2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
+2) Create an instance of the class CryptFile and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 my_instance = CryptFile('target.txt', key)
 ```
 ```python
 my_instance = CryptFile('test.db', key)
 ```
 The file can be of anything : image`.png`, movie `.mp4`,`.sqlite`  etc..
@@ -212,21 +202,21 @@
 ```
 ```python
 my_instance.encrypt()[1]
 ```
 ```python
 my_instance.decrypt()[1]
 ```
-The result simply returns a tuple so index `[0]` is going to be the confirmation if it's `1` then it worked, else some Error has occurred.
+The result simply returns a tuple so index `[0]` is going to be the confirmation if it's `1` then it worked, else an exception will be raised.
 <br>Index `[1]` contains the encrypted/decrypted content.
 
 ## `database` ##
-To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using sqlite3 type database
+To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using sqlite.
 
-Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
+Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep secured.
 
 **Note** that in `database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 Run:
 ```python
 pip install dataclasses
 ```
 
@@ -271,14 +261,15 @@
 You can check the current size of the database using the size property method 
 ```python
 print(conn.size) # Size of the Database in MB 
 ```
 
 6) Check the module itself so you can run through all the available methods.
 <br>The available methods can perform usual operations like insertion, deletion , updating the database and more..
+<br>Use your editor and hover over the target function and it will fetch the docstrings for it.
 
 
 7) to run more complex queries I've dedicated a query function that takes in `*queries` and returns the result fetched 
 ```python
 query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
 print(conn.query(query))
 ```
@@ -311,25 +302,26 @@
 - Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` button to encrypt the given file , if the encryption turns out to be successful , you'll see a success message along with a `added .crypt extention to the file` message. If the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
 - The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
 #### Database
 - Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by :
 1) Specifying the actual path where you want your database to be 
 2) Give it a name, it must be a valid file name that ends with `.db` .<br>
 If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
-3) Did I mention the keys' database ? well if you give a database a file name it will also create the keys database with the same name as the database you chose plus `Keys` added to the name. This database holds the actual keys and the reference to these keys.
+3) Did I mention the keys' database ? if you give your database a name it will also create the keys database with the same name as the database you chose plus `Keys` added to the name. This database holds the actual keys and the reference to these keys.
 <br>The only piece of data that these two separate databases have in common is the key reference values.  
 
    
 **Info**: 
 <br>Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
-`Name` that holds the filename in both databases , although for the keys database if you haven't specified any file to operate on while selecting different keys, then all these inserted keys will be tagged `STANDALONE` 
+`Name` that holds the filename in both db's , although for the keys database if you haven't specified any file to operate on while selecting different keys, then all these inserted keys will be tagged with: `STANDALONE` 
 <br>`Content` for the main db, this holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
 <br>`Key` for  both db's, this holds the `KeyRef` A.K.A key reference value
 #### Usage 
-The buttons are self-explanatory so do what you see fit. The result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+The buttons are self-explanatory so do what you see fit. The result of any task related to the databases is displayed on `DATABASE OUTPUT CONSOLE` 
+<br>You can run a query anytime by writing a query ( raw sqlite query ) and clicking on `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
 <br>Just click buttons and check the result in the output console, it will guide you through the process.
 
 <br>To run the GUI anywhere
 ```shell
 python -m ashcrypt.gui
 ```
```

### Comparing `ashcrypt-3.1.9/ashcrypt/crypt.py` & `ashcrypt-3.2.0/ashcrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.9/ashcrypt/database.py` & `ashcrypt-3.2.0/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.9/ashcrypt/filecrypt.py` & `ashcrypt-3.2.0/ashcrypt/filecrypt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """This module is used to encrypt and decrypt files of either type str or bytes"""
 
-
+from dataclasses import dataclass, field
 from ashcrypt import crypt
 from ashcrypt.utils import exceptions
 import os
 
 
+@dataclass
 class CryptFile:
-    """Class to encrypt/decrypt a given file. Pass in the filename
-                as well as a 256-bit key """
+    """Class to encrypt/decrypt a given file. Pass in the filename as well as a 256-bit key """
+    filename: str = field()
+    key: str = field()
 
-    def __init__(self, filename: str, key: str):
-        self.filename = filename
-        self.bad_key = 0
-        if self.keyverify(key) == 1:
-            self.key = key
-        else:
+    def __post_init__(self):
+        if self.keyverify(self.key) != 1:
             raise exceptions.dynamic.KeyLengthError()
 
     @staticmethod
     def genkey() -> str:
         return crypt.Enc.genkey()
 
     @staticmethod
@@ -30,79 +28,65 @@
                 return 1
         except ValueError:
             return 0
 
     def encrypt(self) -> int:
         if os.path.isdir(self.filename):
             raise exceptions.fixed.GivenDirectoryError()
-        if self.bad_key == 1:
-            raise exceptions.dynamic.KeyLengthError()
+        if not os.path.exists(self.filename):
+            raise exceptions.fixed.FileDoesNotExistError()
+        if os.path.splitext(self.filename)[1] == '.crypt':
+            raise exceptions.fixed.AlreadyEncryptedError()
+        with open(self.filename, 'rb') as f:
+            filecontent = f.read()
         try:
-            if not os.path.exists(self.filename):
-                raise exceptions.fixed.FileDoesNotExistError()
-            else:
-                if os.path.splitext(self.filename)[1] == '.crypt':
-                    raise exceptions.fixed.AlreadyEncryptedError()
-                else:
-                    with open(self.filename, 'rb') as f:
-                        filecontent = f.read()
-                    with open(self.filename, 'wb') as f:
-                        if filecontent:
-                            try:
-                                ins = crypt.Enc(
-                                    message=filecontent, mainkey=self.key)
-                                new_content = ins.encrypt(get_bytes=True)
-                                f.write(new_content)
-                                go_ahead_rename_crypt = 1
-                            except BaseException:
-                                f.write(filecontent)
-                                raise exceptions.fixed.FileCryptError()
-                        else:
-                            f.write(filecontent)
-                            raise exceptions.fixed.EmptyContentError()
-                    if go_ahead_rename_crypt == 1:
-                        os.rename(self.filename, self.filename + '.crypt')
-                        return 1
-        except Exception:
+            with open(self.filename, 'wb') as f:
+                if filecontent:
+                    try:
+                        ins = crypt.Enc(
+                            message=filecontent, mainkey=self.key)
+                        new_content = ins.encrypt(get_bytes=True)
+                        f.write(new_content)
+                        go_ahead_rename_crypt = 1
+                    except BaseException:
+                        f.write(filecontent)
+                        raise exceptions.fixed.FileCryptError()
+                elif not filecontent:
+                    f.write(filecontent)
+                    raise exceptions.fixed.EmptyContentError()
+            if go_ahead_rename_crypt == 1:
+                os.rename(self.filename, self.filename + '.crypt')
+                return 1
+        except IOError:
             raise exceptions.fixed.SysError()
 
     def decrypt(self) -> int:
         if os.path.isdir(self.filename):
             raise exceptions.fixed.GivenDirectoryError()
-        if self.bad_key == 1:
-            raise exceptions.dynamic.KeyLengthError()
+        if not os.path.exists(self.filename):
+            raise exceptions.fixed.FileDoesNotExistError()
+        if os.path.splitext(self.filename)[1] != '.crypt':
+            raise exceptions.fixed.AlreadyDecryptedError()
+        with open(self.filename, 'rb') as f:
+            enc_content = f.read()
         try:
-            if not os.path.exists(self.filename):
-                raise exceptions.fixed.FileDoesNotExistError()
-            else:
-                if os.path.splitext(self.filename)[1] != '.crypt':
-                    raise exceptions.fixed.AlreadyDecryptedError()
-                else:
-                    with open(self.filename, 'rb') as f:
-                        enc_content = f.read()
-                    with open(self.filename, 'wb') as f:
-                        if enc_content:
-                            try:
-                                ins = crypt.Dec(
-                                    message=enc_content, mainkey=self.key)
-                                a = ins.decrypt(get_bytes=True)
-                                f.write(a)
-                                go_ahead_remove_crypt = 1
-                            except Exception:
-                                f.write(enc_content)
-                                raise exceptions.fixed.FileCryptError()
-                        else:
-                            f.write(enc_content)
-                            raise exceptions.fixed.EmptyContentError()
-                    if go_ahead_remove_crypt == 1:
-                        os.rename(
-                            self.filename, os.path.splitext(
-                                self.filename)[0])
-                        return 1
-        except Exception:
+            with open(self.filename, 'wb') as f:
+                if enc_content:
+                    try:
+                        ins = crypt.Dec(
+                            message=enc_content, mainkey=self.key)
+                        a = ins.decrypt(get_bytes=True)
+                        f.write(a)
+                        go_ahead_remove_crypt = 1
+                    except Exception:
+                        f.write(enc_content)
+                        raise exceptions.fixed.FileCryptError()
+                elif not enc_content:
+                    f.write(enc_content)
+                    raise exceptions.fixed.EmptyContentError()
+                if go_ahead_remove_crypt == 1:
+                    os.rename(
+                        self.filename, os.path.splitext(
+                            self.filename)[0])
+                    return 1
+        except IOError:
             raise exceptions.fixed.SysError()
-
-    def __str__(self):
-        return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
-
-    def __repr__(self):
-        return f'{self.__class__.__name__}({self.filename},{self.key})'
```

### Comparing `ashcrypt-3.1.9/ashcrypt/gui.py` & `ashcrypt-3.2.0/ashcrypt/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,19 +324,19 @@
 
 main_db_name_blocker = 0
 db_already_exists_blocker = 0
 maindbname = ''
 
 
 def main_db_name():
-    global main_db_name_blocker,\
-        db_already_exists_blocker,\
-        usable_real_path, db_path_blocker,\
-        success_maindb_connection_blocker,\
-        main_db_conn,\
+    global main_db_name_blocker, \
+        db_already_exists_blocker, \
+        usable_real_path, db_path_blocker, \
+        success_maindb_connection_blocker, \
+        main_db_conn, \
         maindbname
 
     dbname = main_db_name_var.get().strip()
     if re.match(r'((^[\w(-.)?]+\.db$)|(^[\w?(-.)]\.db$))', dbname):
         try:
             maindbname = dbname
             main_db_name_blocker = 1
@@ -380,16 +380,16 @@
             db_display_text.insert(tk.END, f"The database might be distorted")
     else:
         main_db_name_result_var.set('NOT SET')
         main_db_name_blocker = 0
 
 
 def keyd_db_setup():
-    global usable_real_path,\
-        success_keysdb_connection_blocker,\
+    global usable_real_path, \
+        success_keysdb_connection_blocker, \
         keys_db_conn
     if db_path_blocker == 1 and main_db_name_blocker == 1:
         try:
             dbname = main_db_name_var.get().strip()
             keys_db = dbname[:-3] + 'Keys.db'
             dbname_keys_win = '\\' + keys_db
             dbname_keys_unix = '/' + keys_db
@@ -766,15 +766,14 @@
 )
 progressbar2.place(relx=0.05, rely=0.42)
 
 
 '''---------FILE ENCRYPTION/DECRYPTION STARTED-------------'''
 
 
-
 if platform.system() == 'Windows':
     filepathlabel = tk.Label(master=frameFile1,
                              text='FILE PATH',
                              font='Calibre 20',
                              )
     filepathlabel.place(relx=0.335, rely=0.10)
 
@@ -1021,14 +1020,15 @@
         except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Faulty Database\n")
     else:
         keySelectionFlag.set(0)
         keyselectionvar.set('     NOT SELECTED')
 
+
 if platform.system() == 'Windows':
     mainkeyLabel = tk.Label(master=frameFile2,
                             text='MAIN KEY',
                             font='Calibre 20',
                             bootstyle='info',
                             )
     mainkeyLabel.place(relx=0.3, rely=0.075)
@@ -1037,15 +1037,14 @@
                             text='MAIN KEY',
                             font='Calibre 20 bold',
                             bootstyle='info',
                             )
     mainkeyLabel.place(relx=0.3, rely=0.075)
 
 
-
 mainkeyvar = tk.StringVar()
 mainkeyEntry = tk.Entry(master=frameFile2,
                         font='Calibre 14 bold',
                         textvariable=mainkeyvar,
                         width=29
                         )
 mainkeyEntry.place(relx=0.09, rely=0.29)
@@ -1108,32 +1107,19 @@
 keyButton = tk.Button(master=frameFile2,
                       text='GENERATE',
                       command=genkey,
                       bootstyle='success outline')
 keyButton.place(relx=0.671, rely=0.7)
 
 
-'''----------------------------STAMP STARTED ------------------------------'''
-
-
-latest_ID_key_label = tk.Label(
-    master=lowerFrame,
-    text='GitHub.com/AshGw/AES-256',
-    font='Calibre 6')
-latest_ID_key_label.place(relx=0.84, rely=0.92)
-
-'''------------------------------STAMP ENDED------------------------------'''
-
-
 def rm_json():
     global usable_real_path
     file = os.path.join(usable_real_path, 'output.json')
     if os.path.exists(file):
         os.remove(file)
 
 
-
 atexit.register(rm_json)
 
 
 if __name__ == '__main__':
     main_object.mainloop()
```

### Comparing `ashcrypt-3.1.9/ashcrypt/sandbox/clicrypt.py` & `ashcrypt-3.2.0/ashcrypt/sandbox/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.9/ashcrypt/textcrypt.py` & `ashcrypt-3.2.0/ashcrypt/textcrypt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """This module is used to encrypt and decrypt text data"""
 
+from dataclasses import dataclass, field
 from ashcrypt.utils import exceptions
 from ashcrypt import crypt as ac
 from typing import Union
 
 
+@dataclass()
 class Crypt:
-    def __init__(self, text: Union[str, bytes], key: str):
-        self.text = text
-        if self.keyverify(key) == 1:
-            self.key = key
-        else:
+    text: Union[str, bytes] = field()
+    key: str = field()
+
+    def __post_init__(self):
+        if self.keyverify(self.key) != 1:
             raise exceptions.dynamic.KeyLengthError()
 
     @staticmethod
     def genkey() -> str:
         return ac.Enc.genkey()
 
     @staticmethod
@@ -44,13 +46,7 @@
                 a = dec_instance.decrypt()
                 output = a
                 return 1, output
             except BaseException:
                 raise exceptions.fixed.CryptError()
         else:
             raise exceptions.fixed.EmptyContentError()
-
-    def __str__(self):
-        return f'Encrypting/Decrypting Text {self.text[:8]}.. With {self.key} Key '
-
-    def __repr__(self):
-        return f'{self.__class__.__name__}({self.text[:8]},{self.key})'
```

### Comparing `ashcrypt-3.1.9/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.2.0/ashcrypt/unittests/test_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.9/ashcrypt/utils/exceptions/fixed.py` & `ashcrypt-3.2.0/ashcrypt/utils/exceptions/fixed.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 class MessageTamperingError(Exception):
 
     def __init__(self) -> None:
         self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n' \
                        ' or Possible key difference'
         super().__init__(self.display)
 
+
 class EmptyContentError(Exception):
     def __init__(self):
         self.display = 'Empty content !'
         super().__init__(self.display)
 
 
-
 class GivenDirectoryError(Exception):
     def __init__(self):
         self.display = 'Given directory instead of file'
         super().__init__(self.display)
 
 
 class FileDoesNotExistError(Exception):
```

### Comparing `ashcrypt-3.1.9/ashcrypt/utils/safepack/file.py` & `ashcrypt-3.2.0/ashcrypt/utils/safepack/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """This module is used to encrypt and decrypt files of either type str or bytes"""
 
 
 from ashcrypt import crypt
 import os
 
+
 class CryptFile:
     '''Class to encrypt/decrypt a given file. Pass in the filename
                 as well as a 256-bit key '''
-    def __init__(self, filename : str, key : str):
+
+    def __init__(self, filename: str, key: str):
         self.filename = filename
         self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
             self.not_256_bit_key = 1
 
@@ -101,8 +103,8 @@
         except Exception:
             return 4
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({self.filename},{self.key})'
+        return f'{self.__class__.__name__}({self.filename},{self.key})'
```

### Comparing `ashcrypt-3.1.9/ashcrypt/utils/safepack/text.py` & `ashcrypt-3.2.0/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.9/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.2.0/ashcrypt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.9
+Version: 3.2.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.9/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.2.0/ashcrypt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 README.md
 setup.py
-ashcrypt/README.md
 ashcrypt/__init__.py
 ashcrypt/crypt.py
 ashcrypt/database.py
 ashcrypt/filecrypt.py
 ashcrypt/gui.py
 ashcrypt/textcrypt.py
 ashcrypt.egg-info/PKG-INFO
 ashcrypt.egg-info/SOURCES.txt
 ashcrypt.egg-info/dependency_links.txt
 ashcrypt.egg-info/requires.txt
 ashcrypt.egg-info/top_level.txt
 ashcrypt/sandbox/__init__.py
 ashcrypt/sandbox/clicrypt.py
 ashcrypt/unittests/__init__.py
-ashcrypt/unittests/unittest_crypt.py
+ashcrypt/unittests/test_crypt.py
 ashcrypt/utils/__init__.py
 ashcrypt/utils/consts/__init__.py
 ashcrypt/utils/consts/main.py
 ashcrypt/utils/exceptions/__init__.py
 ashcrypt/utils/exceptions/dynamic.py
 ashcrypt/utils/exceptions/fixed.py
 ashcrypt/utils/safepack/__init__.py
```

### Comparing `ashcrypt-3.1.9/setup.py` & `ashcrypt-3.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.9',
+    version='3.2.0',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/AshGw/AES-256.git',
     packages=find_packages(exclude=['important', 'Docker-build', '.github']),
     package_data={
         'ashcrypt': ['**'],
     },
     exclude_package_data={
-        '': ['.gitignore', 'LICENSE', 'README'],
+        '': ['.gitignore', 'LICENSE', 'README.md'],
     },
     install_requires=[
         'bcrypt==4.0.1',
         'cryptography==40.0.2',
         'qrcode==7.4.2',
         'ttkbootstrap==1.10.1',
     ],
```

