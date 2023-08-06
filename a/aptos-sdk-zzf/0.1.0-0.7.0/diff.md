# Comparing `tmp/aptos_sdk_zzf-0.1.0.tar.gz` & `tmp/aptos_sdk_zzf-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptos_sdk_zzf-0.1.0.tar", max compression
+gzip compressed data, was "aptos_sdk_zzf-0.7.0.tar", max compression
```

## Comparing `aptos_sdk_zzf-0.1.0.tar` & `aptos_sdk_zzf-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2746 2023-08-05 14:05:18.540609 aptos_sdk_zzf-0.1.0/README.md
--rw-r--r--   0        0        0       70 2023-08-06 01:28:30.126091 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/__init__.py
--rw-r--r--   0        0        0     5646 2023-08-06 01:28:30.126332 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/account.py
--rw-r--r--   0        0        0    10623 2023-08-06 01:28:30.126629 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/account_address.py
--rw-r--r--   0        0        0     8460 2023-08-06 01:28:30.127017 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/account_sequence_number.py
--rw-r--r--   0        0        0    20758 2023-08-06 01:28:30.127308 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/aptos_token_client.py
--rw-r--r--   0        0        0    27583 2023-08-06 01:28:30.127611 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/async_client.py
--rw-r--r--   0        0        0     5811 2023-08-06 01:28:30.127936 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/authenticator.py
--rw-r--r--   0        0        0    10443 2023-08-06 01:28:30.128119 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/bcs.py
--rw-r--r--   0        0        0    12056 2023-08-06 01:28:30.128294 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/ed25519.py
--rw-r--r--   0        0        0      277 2023-08-06 01:28:30.128431 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/metadata.py
--rw-r--r--   0        0        0     4757 2023-08-06 01:28:30.128574 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/package_publisher.py
--rw-r--r--   0        0        0     8516 2023-08-06 01:28:30.129676 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/transaction_worker.py
--rw-r--r--   0        0        0    26552 2023-08-06 01:28:30.129933 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/transactions.py
--rw-r--r--   0        0        0     8991 2023-08-06 01:28:30.131733 aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/type_tag.py
--rw-r--r--   0        0        0      758 2023-08-06 01:29:57.146229 aptos_sdk_zzf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 aptos_sdk_zzf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2746 2023-08-05 14:05:18.540609 aptos_sdk_zzf-0.7.0/README.md
+-rw-r--r--   0        0        0       70 2023-08-05 14:05:18.540915 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/__init__.py
+-rw-r--r--   0        0        0     5646 2023-08-05 14:05:18.541168 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/account.py
+-rw-r--r--   0        0        0    10623 2023-08-05 14:05:18.541517 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/account_address.py
+-rw-r--r--   0        0        0     8460 2023-08-05 14:05:18.541821 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/account_sequence_number.py
+-rw-r--r--   0        0        0    20758 2023-08-05 14:05:18.542089 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/aptos_token_client.py
+-rw-r--r--   0        0        0    27583 2023-08-05 14:05:18.542459 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/async_client.py
+-rw-r--r--   0        0        0     5811 2023-08-05 14:05:18.542869 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/authenticator.py
+-rw-r--r--   0        0        0    10443 2023-08-05 14:05:18.543129 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/bcs.py
+-rw-r--r--   0        0        0    12056 2023-08-05 14:05:18.543412 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/ed25519.py
+-rw-r--r--   0        0        0      277 2023-08-05 14:05:18.543615 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/metadata.py
+-rw-r--r--   0        0        0     4757 2023-08-05 14:05:18.543892 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/package_publisher.py
+-rw-r--r--   0        0        0     8516 2023-08-05 14:05:18.544183 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/transaction_worker.py
+-rw-r--r--   0        0        0    26552 2023-08-05 14:05:18.544450 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/transactions.py
+-rw-r--r--   0        0        0     8991 2023-08-05 14:05:18.544847 aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/type_tag.py
+-rw-r--r--   0        0        0      758 2023-08-06 01:22:22.964794 aptos_sdk_zzf-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 aptos_sdk_zzf-0.7.0/PKG-INFO
```

### Comparing `aptos_sdk_zzf-0.1.0/README.md` & `aptos_sdk_zzf-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/account.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/account.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/account_address.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/account_address.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/account_sequence_number.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/account_sequence_number.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/aptos_token_client.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/aptos_token_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/async_client.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/async_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/authenticator.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/authenticator.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/bcs.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/bcs.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/ed25519.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/ed25519.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/package_publisher.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/package_publisher.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/transaction_worker.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/transaction_worker.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/transactions.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/transactions.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/aptos_sdk_zzf/type_tag.py` & `aptos_sdk_zzf-0.7.0/aptos_sdk_zzf/type_tag.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk_zzf-0.1.0/pyproject.toml` & `aptos_sdk_zzf-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aptos-sdk-zzf"
-version = "0.1.0"
+version = "0.7.0"
 description = "Aptos SDK"
 authors = ["Aptos Labs <opensource@aptoslabs.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/aptos-labs/aptos-core"
 homepage = "https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk"
 keywords = ["web3", "sdk", "aptos", "blockchain"]
```

### Comparing `aptos_sdk_zzf-0.1.0/PKG-INFO` & `aptos_sdk_zzf-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-sdk-zzf
-Version: 0.1.0
+Version: 0.7.0
 Summary: Aptos SDK
 Home-page: https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk
 License: Apache-2.0
 Keywords: web3,sdk,aptos,blockchain
 Author: Aptos Labs
 Author-email: opensource@aptoslabs.com
 Requires-Python: >=3.8.1,<4.0
```

