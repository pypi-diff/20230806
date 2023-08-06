# Comparing `tmp/chainlib-eth-0.4.9.tar.gz` & `tmp/chainlib-eth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlib-eth-0.4.9.tar", last modified: Fri Feb  3 09:18:24 2023, max compression
+gzip compressed data, was "chainlib-eth-0.5.0.tar", last modified: Sun Aug  6 12:55:52 2023, max compression
```

## Comparing `chainlib-eth-0.4.9.tar` & `chainlib-eth-0.5.0.tar`

### file list

```diff
@@ -1,74 +1,96 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/
--rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-16 08:29:08.000000 chainlib-eth-0.4.9/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:13:49.000000 chainlib-eth-0.4.9/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       89 2022-11-14 07:21:26.000000 chainlib-eth-0.4.9/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      731 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      146 2022-11-14 18:46:19.000000 chainlib-eth-0.4.9/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      872 2022-11-14 07:16:48.000000 chainlib-eth-0.4.9/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:16:57.000000 chainlib-eth-0.4.9/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.659991 chainlib-eth-0.4.9/chainlib/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)     1029 2022-02-27 09:47:47.000000 chainlib-eth-0.4.9/chainlib/eth/address.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4296 2022-12-16 08:27:32.000000 chainlib-eth-0.4.9/chainlib/eth/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      420 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       94 2021-10-18 11:32:11.000000 chainlib-eth-0.4.9/chainlib/eth/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      474 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1135 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      515 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/cli/decode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2479 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/cli/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)       41 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2362 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/cli/rpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      629 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/cli/wallet.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7796 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/connection.py
--rw-r--r--   0 lash      (1000) lash      (1000)      248 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/constant.py
--rw-r--r--   0 lash      (1000) lash      (1000)    15644 2022-12-19 08:03:44.000000 chainlib-eth-0.4.9/chainlib/eth/contract.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.659991 chainlib-eth-0.4.9/chainlib/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)      275 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/dialect/
--rw-r--r--   0 lash      (1000) lash      (1000)      597 2022-12-16 09:15:51.000000 chainlib-eth-0.4.9/chainlib/eth/dialect/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      486 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/dialect/openethereum.py
--rw-r--r--   0 lash      (1000) lash      (1000)      578 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9041 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-10 10:08:49.000000 chainlib-eth-0.4.9/chainlib/eth/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      726 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3659 2022-10-13 13:18:24.000000 chainlib-eth-0.4.9/chainlib/eth/nonce.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/pytest/
--rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      296 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_chain.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2535 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_ethtester.py
--rw-r--r--   0 lash      (1000) lash      (1000)      310 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.663324 chainlib-eth-0.4.9/chainlib/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2815 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/balance.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4512 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      694 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/checksum.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2364 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/count.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2212 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/decode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7400 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)      996 2022-11-12 13:31:10.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/flags.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6114 2023-02-03 09:18:20.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4628 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/get.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5205 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/info.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5572 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/raw.py
--rw-r--r--   0 lash      (1000) lash      (1000)      303 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/subscribe.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4102 2022-11-06 10:28:58.000000 chainlib-eth-0.4.9/chainlib/eth/runnable/wait.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5726 2023-02-03 09:18:20.000000 chainlib-eth-0.4.9/chainlib/eth/settings.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1833 2021-10-10 10:18:45.000000 chainlib-eth-0.4.9/chainlib/eth/sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1209 2022-11-04 07:29:23.000000 chainlib-eth-0.4.9/chainlib/eth/src.py
--rw-r--r--   0 lash      (1000) lash      (1000)    25819 2023-02-03 09:18:20.000000 chainlib-eth-0.4.9/chainlib/eth/tx.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/chainlib/eth/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)     6361 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2551 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/chainlib/eth/unittest/ethtester.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/chainlib_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      731 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1642 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      104 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-02-03 09:18:24.000000 chainlib-eth-0.4.9/chainlib_eth.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      104 2022-11-04 07:31:55.000000 chainlib-eth-0.4.9/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1468 2023-02-03 09:18:24.666658 chainlib-eth-0.4.9/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      474 2022-11-08 10:59:04.000000 chainlib-eth-0.4.9/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2021-12-21 14:52:18.000000 chainlib-eth-0.4.9/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.267273 chainlib-eth-0.5.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3477 2023-06-27 19:32:06.000000 chainlib-eth-0.5.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:13:49.000000 chainlib-eth-0.5.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      111 2023-06-03 11:38:52.000000 chainlib-eth-0.5.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     2735 2023-08-06 12:55:52.267273 chainlib-eth-0.5.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1961 2023-06-03 11:38:17.000000 chainlib-eth-0.5.0/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      872 2022-11-14 07:16:48.000000 chainlib-eth-0.5.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:16:57.000000 chainlib-eth-0.5.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.257273 chainlib-eth-0.5.0/chainlib/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.260606 chainlib-eth-0.5.0/chainlib/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1029 2022-02-27 09:47:47.000000 chainlib-eth-0.5.0/chainlib/eth/address.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4297 2023-02-12 08:11:49.000000 chainlib-eth-0.5.0/chainlib/eth/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      420 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       94 2021-10-18 11:32:11.000000 chainlib-eth-0.5.0/chainlib/eth/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      601 2023-02-07 06:18:34.000000 chainlib-eth-0.5.0/chainlib/eth/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1144 2023-02-12 08:11:49.000000 chainlib-eth-0.5.0/chainlib/eth/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      515 2022-11-06 10:28:58.000000 chainlib-eth-0.5.0/chainlib/eth/cli/decode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2801 2023-06-27 19:27:45.000000 chainlib-eth-0.5.0/chainlib/eth/cli/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       41 2022-10-13 13:18:24.000000 chainlib-eth-0.5.0/chainlib/eth/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2512 2023-02-13 06:36:33.000000 chainlib-eth-0.5.0/chainlib/eth/cli/rpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      629 2022-10-13 13:18:24.000000 chainlib-eth-0.5.0/chainlib/eth/cli/wallet.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7796 2021-12-21 14:52:18.000000 chainlib-eth-0.5.0/chainlib/eth/connection.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      248 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/constant.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    17638 2023-05-08 05:03:13.000000 chainlib-eth-0.5.0/chainlib/eth/contract.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.257273 chainlib-eth-0.5.0/chainlib/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)      291 2023-08-06 12:05:44.000000 chainlib-eth-0.5.0/chainlib/eth/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib/eth/dialect/
+-rw-r--r--   0 lash      (1000) lash      (1000)      597 2023-02-03 09:18:31.000000 chainlib-eth-0.5.0/chainlib/eth/dialect/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      486 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/dialect/openethereum.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      578 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9041 2021-12-21 14:52:18.000000 chainlib-eth-0.5.0/chainlib/eth/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-10 10:08:49.000000 chainlib-eth-0.5.0/chainlib/eth/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      726 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3659 2022-10-13 13:18:24.000000 chainlib-eth-0.5.0/chainlib/eth/nonce.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib/eth/pytest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/pytest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      296 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/pytest/fixtures_chain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2535 2021-12-21 14:52:18.000000 chainlib-eth-0.5.0/chainlib/eth/pytest/fixtures_ethtester.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      310 2021-12-21 14:52:18.000000 chainlib-eth-0.5.0/chainlib/eth/pytest/fixtures_signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2815 2022-11-04 07:29:23.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/balance.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4562 2023-08-06 11:07:28.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      694 2022-11-04 07:29:23.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/checksum.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2364 2022-11-04 07:29:23.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/count.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2367 2023-02-10 16:44:27.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/decode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7307 2023-02-13 06:36:33.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      996 2022-11-12 13:31:10.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/flags.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6095 2023-02-10 16:44:27.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4679 2023-02-12 08:11:49.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/get.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5328 2023-03-01 22:45:39.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/info.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5572 2022-11-06 10:28:58.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/raw.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      303 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/subscribe.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4102 2022-11-06 10:28:58.000000 chainlib-eth-0.5.0/chainlib/eth/runnable/wait.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5717 2023-06-03 06:59:28.000000 chainlib-eth-0.5.0/chainlib/eth/settings.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1833 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/chainlib/eth/sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1209 2022-11-04 07:29:23.000000 chainlib-eth-0.5.0/chainlib/eth/src.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    25819 2023-02-03 09:18:31.000000 chainlib-eth-0.5.0/chainlib/eth/tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib/eth/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)     6361 2021-12-21 14:52:18.000000 chainlib-eth-0.5.0/chainlib/eth/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2705 2023-05-13 09:04:30.000000 chainlib-eth-0.5.0/chainlib/eth/unittest/ethtester.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.263939 chainlib-eth-0.5.0/chainlib_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2735 2023-08-06 12:55:52.000000 chainlib-eth-0.5.0/chainlib_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     2029 2023-08-06 12:55:52.000000 chainlib-eth-0.5.0/chainlib_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 12:55:52.000000 chainlib-eth-0.5.0/chainlib_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-08-06 12:55:52.000000 chainlib-eth-0.5.0/chainlib_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      109 2023-08-06 12:55:52.000000 chainlib-eth-0.5.0/chainlib_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2023-08-06 12:55:52.000000 chainlib-eth-0.5.0/chainlib_eth.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.257273 chainlib-eth-0.5.0/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.267273 chainlib-eth-0.5.0/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3349 2023-05-08 06:23:52.000000 chainlib-eth-0.5.0/man/build/eth-balance.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4585 2023-05-08 06:23:50.000000 chainlib-eth-0.5.0/man/build/eth-count.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4012 2023-05-08 06:23:50.000000 chainlib-eth-0.5.0/man/build/eth-decode.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     9745 2023-05-08 06:23:50.000000 chainlib-eth-0.5.0/man/build/eth-encode.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    11012 2023-05-08 06:23:49.000000 chainlib-eth-0.5.0/man/build/eth-gas.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4333 2023-05-08 06:23:49.000000 chainlib-eth-0.5.0/man/build/eth-get.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4230 2023-05-08 06:23:49.000000 chainlib-eth-0.5.0/man/build/eth-info.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     7965 2023-05-08 06:23:51.000000 chainlib-eth-0.5.0/man/build/eth-raw.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     5024 2023-05-08 06:23:51.000000 chainlib-eth-0.5.0/man/build/eth-wait.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      109 2023-08-06 12:53:57.000000 chainlib-eth-0.5.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1469 2023-08-06 12:55:52.267273 chainlib-eth-0.5.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      974 2023-06-03 12:08:30.000000 chainlib-eth-0.5.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2023-06-10 09:02:56.000000 chainlib-eth-0.5.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 12:55:52.267273 chainlib-eth-0.5.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     7080 2023-03-29 08:49:49.000000 chainlib-eth-0.5.0/tests/test_abi.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      978 2022-05-04 18:10:33.000000 chainlib-eth-0.5.0/tests/test_address.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2244 2023-02-03 09:18:31.000000 chainlib-eth-0.5.0/tests/test_block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     8184 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/tests/test_bloom.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1196 2022-10-13 13:18:24.000000 chainlib-eth-0.5.0/tests/test_cli.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      896 2023-03-29 09:08:32.000000 chainlib-eth-0.5.0/tests/test_event.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      620 2021-10-10 10:18:45.000000 chainlib-eth-0.5.0/tests/test_nonce.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3466 2021-12-21 14:52:18.000000 chainlib-eth-0.5.0/tests/test_sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1607 2022-10-13 13:18:24.000000 chainlib-eth-0.5.0/tests/test_stat.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6621 2022-10-13 13:18:24.000000 chainlib-eth-0.5.0/tests/test_tx.py
```

### Comparing `chainlib-eth-0.4.9/CHANGELOG` & `chainlib-eth-0.5.0/CHANGELOG`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,49 @@
+- 0.4.27
+	* Fix break in encoding string values for eth-encode CLI tool
+- 0.4.26
+	* Upgrade funga-eth to ensure safe-pysha3
+	* Limit python runtime environment to <3.11 (eth-tester environment not currently compatible)
+- 0.4.25
+	* Replace pysha3 with safe-pysha3
+- 0.4.24
+	* Update texinfo documentation
+	* Generate readme from texinfo documentation
+- 0.4.23
+	* Fix encode hex translation bug 
+- 0.4.22
+	* Add roles and contracts index in unittest fixture
+- 0.4.21
+	* Add man pages to installer
+- 0.4.20
+	* Enable short 0 value in eth-encode for address and bytes
+- 0.4.19
+	* Proper hex comparison in contract topic decoder
+- 0.4.18
+	* Set a dirty bit on abi encoder when type added before contents generation
+	* Support for tuple abi encoding (decoding not implemented)
+	* Rename log decoder signature method to get_signature
+- 0.4.17
+	* Add dialect filter to info and block cli tools
+- 0.4.16
+	* Add dynamic bytes encoding in contracts module
+- 0.4.15
+	* Enable setting of unsigned sender address for contract calls
+- 0.4.14
+	* Enable wait on eth-encode
+- 0.4.13
+	* Enable send from eth-encode
+- 0.4.12
+	* Fix remaining flag bugs in cli tools
+- 0.4.11
+	* Add literal type definition support for contract argument building	
+- 0.4.10
+	* Remove rpc lookup when using arg-mode in eth-encode regardless of fee arguments
+- 0.4.9
+	* Enable contract creation with eth-gas tool when recipient is omitted
 - 0.4.8
 	* Add support for dialect differences in tx and block processing
 - 0.4.7
 	* Add support for all power of two uint sizes
 - 0.4.6
 	* Correct license classifier for python package
 - 0.4.5
```

### Comparing `chainlib-eth-0.4.9/LICENSE` & `chainlib-eth-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/WAIVER` & `chainlib-eth-0.5.0/WAIVER`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/WAIVER.asc` & `chainlib-eth-0.5.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/address.py` & `chainlib-eth-0.5.0/chainlib/eth/address.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/block.py` & `chainlib-eth-0.5.0/chainlib/eth/block.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,17 @@
     tx_generator = Tx
 
     def __init__(self, src=None, dialect_filter=None):
         super(Block, self).__init__(src=src, dialect_filter=dialect_filter)
 
 
     def load_src(self, dialect_filter=None):
+        if dialect_filter != None:
+            dialect_filter.apply_block(self)
+
         self.set_hash(self.src['hash'])
         try:
             self.number = int(strip_0x(self.src['number']), 16)
         except TypeError:
             self.number = int(self.src['number'])
         self.txs = self.src['transactions']
         self.block_src = self.src
@@ -115,16 +118,14 @@
         except KeyError:
             self.author = self.src['miner']
 
         self.fee_limit = self.src['gas_limit']
         self.fee_cost = self.src['gas_used']
         self.parent_hash = self.src['parent_hash']
 
-        if dialect_filter != None:
-            dialect_filter.apply_block(self)
 
 
     def tx_index_by_hash(self, tx_hash):
         i = 0
         idx = -1
         tx_hash = add_0x(tx_hash)
         for tx in self.txs:
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/cli/config.py` & `chainlib-eth-0.5.0/chainlib/eth/cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,21 @@
     """
     default_base_config_dir = os.path.join(data_dir, 'data', 'config')
     default_fee_limit = 21000
 
 
 def process_config(config, arg, args, flags, positional_name=None):
     config = base_process_config(config, arg, args, flags, positional_name=positional_name)
-    if arg.match('provider', flags):
+#    if arg.match('provider', flags):
+#        if not bool(config.get('RPC_DIALECT')):
+#            config.add('default', 'RPC_DIALECT', exists_ok=True)
+#        elif config.get('RPC_DIALECT') not in [
+#                'openethereum',
+#                'default',
+#                ]:
+#            raise ValueError('unknown rpc dialect {}'.format(config.get('RPC_DIALECT'))) 
 
-        if not bool(config.get('RPC_DIALECT')):
-            config.add('default', 'RPC_DIALECT', exists_ok=True)
-        elif config.get('RPC_DIALECT') not in [
-                'openethereum',
-                'default',
-                ]:
-            raise ValueError('unknown rpc dialect {}'.format(config.get('RPC_DIALECT'))) 
-
-    if arg.match('create', flags):
-        config.add(getattr(args, 'null'), '_NULL')
+    #if arg.match('create', flags):
+    #    config.add(getattr(args, 'null'), '_NULL')
 
 
     return config
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/cli/decode.py` & `chainlib-eth-0.5.0/chainlib/eth/cli/decode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/cli/encode.py` & `chainlib-eth-0.5.0/chainlib/eth/cli/encode.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import logging
 
 # external imports
 from chainlib.eth.contract import (
         ABIContractType,
         ABIContractEncoder,
         )
+from chainlib.eth.constant import ZERO_ADDRESS
+from chainlib.eth.constant import ZERO_CONTENT
 
 logg = logging.getLogger(__name__)
 
 
 class CLIEncoder(ABIContractEncoder):
 
     __re_uint = r'^([uU])[int]*([0-9]+)?$'
@@ -77,27 +79,33 @@
         if m == None:
             return None
         s = 'STRING'
         a = getattr(ABIContractType, s)
         return (s, a)
 
 
-    def translate_type(self, typ):
+    def translate(self, typ, val):
         r = None
         for tr in self.__translations:
             r = getattr(self, tr)(typ)
             if r != None:
                 break
         if r == None:
             raise ValueError('no translation for type {}'.format(typ))
         logg.debug('type {} translated to {}'.format(typ, r[0]))
-        return r[1]
+        if r[0] != 'STRING':
+            if int(val, 16) == 0:
+                if r[0][0] == 'B':
+                    val = ZERO_CONTENT
+                elif r[0][0] == 'A':
+                    val = ZERO_ADDRESS
+        return (r[1], val,)
 
 
     def add_from(self, arg):
         logg.debug('arg {}'.format(arg))
         (typ, val) = arg.split(':', maxsplit=1)
-        real_typ = self.translate_type(typ)
+        (real_typ, val) = self.translate(typ, val)
         if self.signature != None:
             self.typ(real_typ)
         fn = getattr(self, real_typ.value)
         fn(val)
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/cli/rpc.py` & `chainlib-eth-0.5.0/chainlib/eth/cli/rpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # external imports
 from chainlib.cli import Rpc as BaseRpc
 from chainlib.eth.connection import EthHTTPConnection
+from chainlib.eth.constant import ZERO_ADDRESS
 
 # local imports
 from chainlib.eth.gas import (
         OverrideGasOracle,
         RPCGasOracle,
         )
 from chainlib.eth.nonce import (
@@ -15,14 +16,17 @@
 
 # TODO: how is the keystore implemented in rpc here?
 class Rpc(BaseRpc):
     """Convenience constructor to set Ethereum defaults for chainlib cli Rpc object
 
 
     """
+
+    default_sender_address = ZERO_ADDRESS
+
     def __init__(self, wallet=None):
         super(Rpc, self).__init__(EthHTTPConnection, wallet=wallet)
 
     
     def connect_by_config(self, config, nonce_confirmed=True):
         """
 
@@ -55,17 +59,18 @@
             pass
 
         if fee_price != None or fee_limit != None:
             self.fee_oracle = OverrideGasOracle(price=fee_price, limit=fee_limit, conn=self.conn, id_generator=self.id_generator)
         else:
             self.fee_oracle = RPCGasOracle(self.conn, id_generator=self.id_generator)
 
-        error_parser = None
-        if config.get('RPC_DIALECT') == 'openethereum':
-            from chainlib.eth.dialect.openethereum import DialectErrorParser
-            self.error_parser = DialectErrorParser()
+        # todo move to separate repo for dialect apply
+        #error_parser = None
+        #if config.get('RPC_DIALECT') == 'openethereum':
+        #    from chainlib.eth.dialect.openethereum import DialectErrorParser
+        #    self.error_parser = DialectErrorParser()
 
         return self.conn
 
 
     def get_gas_oracle(self):
         return self.get_fee_oracle()
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/cli/wallet.py` & `chainlib-eth-0.5.0/chainlib/eth/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/connection.py` & `chainlib-eth-0.5.0/chainlib/eth/connection.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/contract.py` & `chainlib-eth-0.5.0/chainlib/eth/contract.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 
 # external imports
 from hexathon import (
         strip_0x,
         add_0x,
         pad,
+        same as same_hex,
         )
 
 # local imports
 from chainlib.hash import keccak256_string_to_hex
 from chainlib.block import BlockSpec
 from chainlib.jsonrpc import JSONRPCRequest
 from .address import to_checksum_address
@@ -30,27 +31,40 @@
     UINT128 = 'uint128'
     UINT64 = 'uint64'
     UINT32 = 'uint32'
     UINT16 = 'uint16'
     UINT8 = 'uint8'
     ADDRESS = 'address'
     STRING = 'string'
+    BYTES = 'bytes'
     BOOLEAN = 'bool'
+    TUPLE = 'tuple'
 
 dynamic_contract_types = [
     ABIContractType.STRING,
+    ABIContractType.BYTES,
     ]
 
+pointer_contract_types = [
+    ABIContractType.TUPLE,
+        ] + dynamic_contract_types
+
 
 class ABIContract:
     """Base class for Ethereum smart contract encoder
     """
     def __init__(self):
         self.types = []
         self.contents = []
+        self.dirty = False
+
+
+    def add_type(self, v):
+        self.types.append(v)
+        self.dirty = True
 
 
 class ABIMethodEncoder(ABIContract):
     """Generate ABI method signatures from method signature string.
     """
     def __init__(self):
         super(ABIMethodEncoder, self).__init__()
@@ -73,56 +87,93 @@
 
     def get_method(self):
         """Return currently set method signature string.
 
         :rtype: str
         :returns: Method signature
         """
+        contents = '(' + ','.join(self.method_contents) + ')'
         if self.method_name == None:
-            return ''
-        return '{}({})'.format(self.method_name, ','.join(self.method_contents))
+            return contents
+        return self.method_name + contents
 
 
     def typ(self, v):
         """Add argument type to argument vector.
 
         Method name must be set before this is called.
 
         :param v: Type to add
         :type v: chainlib.eth.contract.ABIContractType
         :raises AttributeError: Type set before method name
         :raises TypeError: Invalid type
         """
-        if self.method_name == None:
-            raise AttributeError('method name must be set before adding types')
+        if isinstance(v, ABIContractEncoder):
+            return self.typ_tuple(v)
         if not isinstance(v, ABIContractType):
             raise TypeError('method type not valid; expected {}, got {}'.format(type(ABIContractType).__name__, type(v).__name__))
         self.method_contents.append(v.value)
         self.__log_method()
 
 
+    def typ_literal(self, v):
+        if type(v).__name__ != 'str':
+            raise ValueError('literal type must be string')
+        self.method_contents.append(v)
+        self.__log_method()
+
+
+    def typ_tuple(self, v):
+        if not isinstance(v, ABIContractEncoder):
+            raise TypeError('tuple type not valid; expected {}, got {}'.format(type(ABIContractEncoder).__name__, type(v).__name__))
+        r = v.get_method()
+        self.method_contents.append(r)
+        self.__log_method()
+
+
     def __log_method(self):
         logg.debug('method set to {}'.format(self.get_method()))
 
 
+    def get_signature(self):
+        """Generate topic signature from set topic.
+
+        :rtype: str
+        :returns: Topic signature, in hex
+        """
+        if self.method_name == None:
+            return ''
+        s = self.get_method()
+        return keccak256_string_to_hex(s)
+
+
+    def get_method_signature(self):
+        s = self.get_signature()
+        if s == '':
+            return s
+        return s[:8]
+
+
 
 class ABIContractDecoder(ABIContract):
     """Decode serialized ABI contract input data to corresponding python primitives.
     """
     
     def typ(self, v):
         """Add type to argument array to parse input against.
 
         :param v: Type
         :type v: chainlib.eth.contract.ABIContractType
         :raises TypeError: Invalid type
         """
         if not isinstance(v, ABIContractType):
             raise TypeError('method type not valid; expected {}, got {}'.format(type(ABIContractType).__name__, type(v).__name__))
-        self.types.append(v.value)
+        if v == ABIContractType.TUPLE:
+            raise NotImplementedError('sorry, tuple decoding not yet implemented')
+        self.add_type(v.value)
         self.__log_typ()
 
 
     def val(self, v):
         """Add value to value array.
 
         :param v: Value, in hex
@@ -273,52 +324,48 @@
         """Set topic to match.
 
         :param event: Topic name
         :type event: str
         """
         self.method(event)
 
-
-    def get_method_signature(self):
-        """Generate topic signature from set topic.
-
-        :rtype: str
-        :returns: Topic signature, in hex
-        """
-        s = self.get_method()
-        return keccak256_string_to_hex(s)
-
-
     def typ(self, v):
         """Add type to event argument array.
 
         :param v: Type
         :type v: chainlib.eth.contract.ABIContractType
         """
         super(ABIContractLogDecoder, self).typ(v)
-        self.types.append(v.value)
+        self.add_type(v.value)
+
 
 
     def apply(self, topics, data):
         """Set log entry data to parse.
 
         After set, self.decode can be used to render the output.
 
         :param topics: The topics array of the receipt, list of hex
         :type topics: list
         :param data: Non-indexed data, in hex
         :type data: str
         :raises ValueError: Topic of input does not match topic set in parser
         """
-        t = self.get_method_signature()
-        if topics[0] != t:
+        t = self.get_signature()
+        if not same_hex(topics[0], t):
             raise ValueError('topic mismatch')
         for i in range(len(topics) - 1):
             self.contents.append(topics[i+1])
         self.contents += data
+
+
+    # Backwards compatibility
+    def get_method_signature(self):
+        logg.warning('ABIContractLogDecoder.get_method_signature() is deprecated. Use ABIContractLogDecoder.get_signature() instead')
+        return self.get_signature()
               
 
 class ABIContractEncoder(ABIMethodEncoder):
 
     def __log_latest(self, v):
         l = len(self.types) - 1 
         logg.debug('Encoder added {} -> {} ({})'.format(v, self.contents[l], self.types[l].value))
@@ -329,15 +376,15 @@
 
         :param v: Integer value
         :type v: int
         """
         v = int(v)
         b = v.to_bytes(32, 'big')
         self.contents.append(b.hex())
-        self.types.append(ABIContractType.UINT256)
+        self.add_type(ABIContractType.UINT256)
         self.__log_latest(v)
 
 
     def uintn(self, v, bitsize):
         """Encode value to uint256 and add to input value vector.
 
         :param v: Integer value
@@ -351,15 +398,15 @@
         # encodings of all uint types are padded to word boundary
         return self.uint256(v)
 
         v = int(v)
         b = v.to_bytes(int(bitsize / 8), 'big')
         self.contents.append(b.hex())
         typ = getattr(ABIContractType, 'UINT' + str(bitsize))
-        self.types.append(typ)
+        self.add_type(typ)
         self.__log_latest(v)
 
 
     def bool(self, v):
         """Alias of chainlib.eth.contract.ABIContractEncoder.boolean.
         """
         return self.boolean(v)
@@ -380,125 +427,143 @@
 
     def address(self, v):
         """Encode value to address and add to input value vector.
 
         :param v: Ethereum address, in hex
         :type v: str
         """
-        self.bytes_fixed(32, v, 20)
-        self.types.append(ABIContractType.ADDRESS)
+        self.bytes_fixed(32, v, exact=20)
+        self.add_type(ABIContractType.ADDRESS)
         self.__log_latest(v)
 
 
     def bytes32(self, v):
         """Encode value to bytes32 and add to input value vector.
 
         :param v: Bytes, in hex
         :type v: str
         """
         self.bytes_fixed(32, v)
-        self.types.append(ABIContractType.BYTES32)
+        self.add_type(ABIContractType.BYTES32)
         self.__log_latest(v)
 
 
     def bytes4(self, v):
         """Encode value to bytes4 and add to input value vector.
 
         :param v: Bytes, in hex
         :type v: str
         """
         self.bytes_fixed(4, v)
-        self.types.append(ABIContractType.BYTES4)
+        self.add_type(ABIContractType.BYTES4)
         self.__log_latest(v)
 
 
+    def tuple(self, v):
+        if type(v).__name__ != 'ABIContractEncoder':
+            raise ValueError('Type for tuple must be ABIContractEncoder')
+        r = v.get_contents()
+        self.bytes_fixed(int(len(r) / 2), r)
+        self.add_type(ABIContractType.TUPLE)
+        self.__log_latest(v)
+
 
     def string(self, v):
         """Encode value to string and add to input value vector.
 
         :param v: String input
         :type v: str
         """
         b = v.encode('utf-8')
-        l = len(b)
+        return self._bytes(b, pad=True)
+
+
+    def bytes(self, v):
+        b = bytes.fromhex(v)
+        return self._bytes(b, pad=True)
+        
+
+    def _bytes(self, v, pad=False):
+        l = len(v)
         contents = l.to_bytes(32, 'big')
-        contents += b
+        contents += v
         padlen = 32 - (l % 32)
-        contents += padlen * b'\x00'
+        if pad:
+            contents += padlen * b'\x00'
         self.bytes_fixed(len(contents), contents)
-        self.types.append(ABIContractType.STRING)
+        self.add_type(ABIContractType.STRING)
         self.__log_latest(v)
         return contents
 
 
-    def bytes_fixed(self, mx, v, exact=0):
+    def bytes_fixed(self, mx, v, exact=0, enforce_word=False):
         """Add arbirary length byte data to value vector.
 
         :param mx: Max length of input data.
         :type mx: int
         :param v: Byte input, hex or bytes
         :type v: str | bytes
         :param exact: Fail parsing if input does not translate to given byte length.
         :type exact: int
         :raises ValueError: Input length or input format mismatch.
         """
         typ = type(v).__name__
         if typ == 'str':
             v = strip_0x(v)
             l = len(v)
+            if mx == 0:
+                mx = l
             if exact > 0 and l != exact * 2:
                 raise ValueError('value wrong size; expected {}, got {})'.format(mx, l))
+            if enforce_word and mx % 32 > 0:
+                raise ValueError('value size {} does not match word boundary'.format(mx))
             if l > mx * 2:
                 raise ValueError('value too long ({})'.format(l))
             v = pad(v, mx)
         elif typ == 'bytes':
             l = len(v)
+            if mx == 0:
+                mx = l
             if exact > 0 and l != exact:
                 raise ValueError('value wrong size; expected {}, got {})'.format(mx, l))
+            if enforce_word and mx % 32 > 0:
+                raise ValueError('value size {} does not match word boundary'.format(mx))
             b = bytearray(mx)
             b[mx-l:] = v
             v = pad(b.hex(), mx)
         else:
             raise ValueError('invalid input {}'.format(typ))
         self.contents.append(v.ljust(64, '0'))
 
-    
-    def get_method_signature(self):
-        """Return abi encoded signature of currently set method.
-        """
-        s = self.get_method()
-        if s == '':
-            return s
-        return keccak256_string_to_hex(s)[:8]
-
 
     def get_contents(self):
         """Encode value array.
 
         :rtype: str
         :returns: ABI encoded values, in hex
         """
         direct_contents = ''
         pointer_contents = ''
         l = len(self.types)
         pointer_cursor = 32 * l
         for i in range(l):
-            if self.types[i] in dynamic_contract_types:
+            if self.types[i] in pointer_contract_types:
                 content_length = len(self.contents[i])
                 pointer_contents += self.contents[i]
                 direct_contents += pointer_cursor.to_bytes(32, 'big').hex()
                 pointer_cursor += int(content_length / 2)
             else:
                 direct_contents += self.contents[i]
         s = ''.join(direct_contents + pointer_contents)
         for i in range(0, len(s), 64):
             l = len(s) - i
             if l > 64:
                 l = 64
             logg.debug('code word {} {}'.format(int(i / 64), s[i:i+64]))
+        self.dirty = False
         return s
 
 
     def get(self):
         """Alias of chainlib.eth.contract.ABIContractEncoder.encode
         """
         return self.encode()
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/dialect/__init__.py` & `chainlib-eth-0.5.0/chainlib/eth/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/error.py` & `chainlib-eth-0.5.0/chainlib/eth/error.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/gas.py` & `chainlib-eth-0.5.0/chainlib/eth/gas.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/jsonrpc.py` & `chainlib-eth-0.5.0/chainlib/eth/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/log.py` & `chainlib-eth-0.5.0/chainlib/eth/log.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/nonce.py` & `chainlib-eth-0.5.0/chainlib/eth/nonce.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/pytest/fixtures_ethtester.py` & `chainlib-eth-0.5.0/chainlib/eth/pytest/fixtures_ethtester.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/balance.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/balance.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/block.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 logg.debug('config loaded:\n{}'.format(config))
 
 settings = ChainSettings()
 settings = process_settings_local(settings, config)
 logg.debug('settings loaded:\n{}'.format(settings))
 
 
-
 def get_block(settings):
     hsh = None
     try:
         hsh = settings.get('HASH')[0]
     except TypeError:
         pass
     r = None
@@ -163,15 +162,15 @@
     if block_src == None:
         logg.error('Block hash {} not found'.format(block_hash))
         sys.exit(1)
     return block_src
 
 
 def block_process(block_src):
-    return Block(block_src)
+    return Block(block_src, dialect_filter=settings.get('RPC_DIALECT_FILTER'))
 
 
 def main():
     r = get_block(settings)
 
     if not config.true('_RAW'):
         r = r.to_human()
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/checksum.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/checksum.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/count.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/count.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/decode.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/decode.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,15 +47,18 @@
     try:
         data = strip_0x(data)
     except TypeError:
         data = stdin_arg()
         data = strip_0x(data)
 
     config.add(data, '_TX_DATA', False)
-
+    
+    # workaround to avoid rpc lookup of fee parameters when using arg mode
+    config.add(0, '_FEE_PRICE', True)
+    config.add(0, '_FEE_LIMIT', True)
     return config
 
 
 arg_flags = ArgFlag()
 arg = Arg(arg_flags)
 flags = arg_flags.VERBOSE | arg_flags.CHAIN_SPEC | arg_flags.RAW | arg_flags.ENV | arg_flags.SEQ | arg_flags.TAB
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/encode.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/encode.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,20 +57,23 @@
 script_dir = os.path.dirname(os.path.realpath(__file__)) 
 config_dir = os.path.join(script_dir, '..', 'data', 'config')
 
 
 def process_config_local(config, arg, args, flags):
     config.add(args.signature, '_SIGNATURE', False)
     config.add(args.contract_args, '_CONTRACT_ARGS', False)
+    # workaround to avoid rpc lookup of fee parameters when using arg mode
+    if args.mode == 'arg':
+        config.add(0, '_FEE_PRICE', True)
+        config.add(0, '_FEE_LIMIT', True)
     return config
 
 arg_flags = ArgFlag()
 arg = Arg(arg_flags)
 flags = arg_flags.STD_WRITE | arg_flags.EXEC | arg_flags.FEE | arg_flags.FMT_HUMAN | arg_flags.FMT_WIRE | arg_flags.FMT_RPC
-flags |= arg_flags.CREATE
 
 argparser = chainlib.eth.cli.ArgumentParser()
 argparser = process_args(argparser, arg, flags)
 argparser.add_argument('--mode', type=str, choices=['tx', 'call', 'arg'], help='Mode of operation')
 argparser.add_argument('--signature', type=str, help='Method signature to encode')
 argparser.add_argument('contract_args', type=str, nargs='*', help='arguments to encode')
 args = argparser.parse_args()
@@ -83,38 +86,18 @@
 logg.debug('config loaded:\n{}'.format(config))
 
 settings = ChainSettings()
 settings = process_settings(settings, config)
 logg.debug('settings loaded:\n{}'.format(settings))
 
 
-#wallet = chainlib.eth.cli.Wallet(EIP155Signer)
-#wallet.from_config(config)
-#
-#rpc = chainlib.eth.cli.Rpc(wallet=wallet)
-#conn = rpc.connect_by_config(config)
-#
-#send = config.true('_RPC_SEND')
-
-#chain_spec = None
-#try:
-#    chain_spec = ChainSpec.from_chain_str(config.get('CHAIN_SPEC'))
-#except AttributeError:
-#    pass
-
-
 def main():
 
     signer_address = ZERO_ADDRESS
     signer = None
-    #try:
-        #signer = rpc.get_signer()
-    #    signer_address = rpc.get_signer_address()
-    #except SignerMissingException:
-    #    pass
     conn = settings.get('CONN')
     signer_address = settings.get('SENDER_ADDRESS')
 
     code = '0x'
     cli_encoder = CLIEncoder(signature=config.get('_SIGNATURE'))
 
     for arg in config.get('_CONTRACT_ARGS'):
@@ -222,17 +205,22 @@
             use_nonce=True,
             )
     tx = c.set_code(tx, code)
     tx_format = TxFormat.JSONRPC
     if config.get('_RAW'):
         tx_format = TxFormat.RLP_SIGNED
     (tx_hash_hex, o) = c.finalize(tx, tx_format=tx_format)
-    if settings.get('SEND'):
+    if settings.get('RPC_SEND'):
         r = conn.do(o)
-        print(r)
+        if settings.get('WAIT'):
+            r = conn.wait(tx_hash_hex)
+            if r['status'] == 0:
+                logg.critical('VM revert. Wish I could tell you more')
+                sys.exit(1)
+        print(tx_hash_hex)
     else:
         if config.get('_RAW'):
             o = strip_0x(o)
         print(o)
 
 if __name__ == '__main__':
     main()
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/flags.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/flags.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/gas.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/gas.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     config.add(data, '_DATA', False)
     config.add(args.amount[0], '_VALUE', False)
     return config
 
 
 arg_flags = ArgFlag()
 arg = Arg(arg_flags)
-flags = arg_flags.STD_WRITE | arg_flags.WALLET | arg_flags.CREATE | arg_flags.VALUE | arg_flags.TAB
+flags = arg_flags.STD_WRITE | arg_flags.WALLET | arg_flags.VALUE | arg_flags.TAB
 
 argparser = chainlib.eth.cli.ArgumentParser()
 argparser = process_args(argparser, arg, flags)
 argparser.add_argument('--data', type=str, action='append', help='Transaction data')
 argparser.add_argument('amount', type=str, help='Token amount to send')
 args = argparser.parse_args()
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/get.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     if tx == None:
         tx = Tx(tx_src)
     if rcpt != None:
         tx.apply_receipt(rcpt)
         rcpt = snake_and_camel(rcpt)
         o = block_by_hash(rcpt['block_hash'])
         r = conn.do(o)
-        block = Block(r)
+        block = Block(r, dialect_filter=settings.get('RPC_DIALECT_FILTER'))
         tx.apply_block(block)
     tx.generate_wire(chain_spec)
     return tx
     
 
 
 def get_address(conn, address, id_generator, height):
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/info.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if config.get('_ENTRY') not in results_translation.keys():
             raise ValueError('Unknown entry {}'.format(config.get('_ENTRY')))
     return config
 
 
 arg_flags = ArgFlag()
 arg = Arg(arg_flags)
-flags = arg_flags.STD_READ | arg_flags.ENV
+flags = arg_flags.STD_READ_NOEX | arg_flags.ENV | arg_flags.TAB
 
 argparser = chainlib.eth.cli.ArgumentParser()
 argparser = process_args(argparser, arg, flags)
 argparser.add_argument('--long', action='store_true', help='Calculate averages through sampling of blocks and txs')
 argparser.add_argument('--local', action='store_true', help='Include local info')
 argparser.add_argument('entry', nargs='?', help='Output single item')
 args = argparser.parse_args()
@@ -128,24 +128,24 @@
     if human:
         n = format(n, ',')
     if set_result(results, 'block', n):
         return
 
     o = block_by_number(first_block_number, False, id_generator=settings.get('RPC_ID_GENERATOR'))
     r = settings.get('CONN').do(o)
-    last_block = Block(r)
+    last_block = Block(r, dialect_filter=settings.get('RPC_DIALECT_FILTER'))
     last_timestamp = last_block.timestamp
 
     if config.true('_LONG'):
         aggr_time = 0.0
         aggr_gas = 0
         for i in range(BLOCK_SAMPLES): 
             o = block_by_number(first_block_number-i, False, id_generator=settings.get('RPC_ID_GENERATOR'))
             r = settings.get('CONN').do(o)
-            block = Block(r)
+            block = Block(r, dialect_filter=settings.get('RPC_DIALECT_FILTER'))
             aggr_time += last_block.timestamp - block.timestamp
         
             gas_limit = int(r['gasLimit'], 16)
             aggr_gas += gas_limit
 
             last_block = block
             last_timestamp = block.timestamp
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/raw.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/raw.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/runnable/wait.py` & `chainlib-eth-0.5.0/chainlib/eth/runnable/wait.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/settings.py` & `chainlib-eth-0.5.0/chainlib/eth/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,24 @@
     settings.set('RPC_SEND', config.true('_RPC_SEND'))
     settings.set('WAIT', config.true('_WAIT'))
 
     gas_oracle = rpc.get_gas_oracle()
     settings.set('GAS_ORACLE', gas_oracle)
     settings.set('FEE_ORACLE', gas_oracle)
 
+    sender_address = rpc.get_sender_address()
     try:
         settings.set('SIGNER', rpc.get_signer())
-        sender_address = rpc.get_sender_address()
-        settings.set('SENDER_ADDRESS', add_0x(sender_address))
     except AttributeError:
         pass
     except SignerMissingException:
         pass
 
+    settings.set('SENDER_ADDRESS', add_0x(sender_address))
+
     nonce_oracle = rpc.get_nonce_oracle()
     settings.set('NONCE_ORACLE', nonce_oracle)
 
     return settings
 
 
 def process_settings_blockspec(settings, config):
@@ -156,15 +157,14 @@
         raise ValueError('invalid checksum address: {}'.format(exec_address_in))
     exec_address = add_0x(exec_address)
 
     settings.set('EXEC', exec_address)
     return settings
 
 
-
 def process_settings_data(settings, config):
     data = None
     try:
         data = config.get('_DATA')
     except KeyError:
         settings.set('DATA', None)
         return settings
@@ -177,15 +177,14 @@
     return settings
 
 
 def process_settings_value(settings, config):
     updated_value = __calculate_net_amount(settings, config)
     settings.set('VALUE', updated_value)
 
-
     return settings
 
 
 def process_settings_hash(settings, config):
     hshs = None
     try:
         hshs = config.get('_HASH')
```

### Comparing `chainlib-eth-0.4.9/chainlib/eth/sign.py` & `chainlib-eth-0.5.0/chainlib/eth/sign.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/src.py` & `chainlib-eth-0.5.0/chainlib/eth/src.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/tx.py` & `chainlib-eth-0.5.0/chainlib/eth/tx.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/unittest/base.py` & `chainlib-eth-0.5.0/chainlib/eth/unittest/base.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/chainlib/eth/unittest/ethtester.py` & `chainlib-eth-0.5.0/chainlib/eth/unittest/ethtester.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,18 +64,25 @@
         self.helper = eth_tester_instance
         self.backend = self.helper.backend
         self.rpc = TestRPCConnection(None, eth_tester_instance, self.signer)
 
         for a in self.keystore.list():
             self.accounts.append(add_0x(to_checksum_address(a)))
 
+        self.publisher = self.accounts[0]
+
         def rpc_with_tester(chain_spec=self.chain_spec, url=None):
             return self.rpc
 
         RPCConnection.register_constructor(ConnType.CUSTOM, rpc_with_tester, tag='default')
         RPCConnection.register_constructor(ConnType.CUSTOM, rpc_with_tester, tag='signer')
         RPCConnection.register_location('custom', self.chain_spec, tag='default', exist_ok=True)
         RPCConnection.register_location('custom', self.chain_spec, tag='signer', exist_ok=True)
+
+        self.contracts = {}
+        self.roles = {
+            'publisher': self.publisher,
+                }
         
 
     def tearDown(self):
         pass
```

### Comparing `chainlib-eth-0.4.9/chainlib_eth.egg-info/entry_points.txt` & `chainlib-eth-0.5.0/chainlib_eth.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.4.9/setup.cfg` & `chainlib-eth-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = chainlib-eth
-version = 0.4.9
+version = 0.5.0
 description = Ethereum implementation of the chainlib interface
 author = Louis Holbrook
 author_email = dev@holbrook.no
-url = https://git.defalslfy.org/chainlib-eth,git
+url = https://git.defalslfy.org/chainlib-eth
 keywords = 
 	dlt
 	blockchain
 	cryptocurrency
 	ethereum
 classifiers = 
 	Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 	Topic :: Internet
 license = AGPLv3+
 licence_files = 
 	LICENSE
 
 [options]
 include_package_data = True
-python_requires = >= 3.7
+python_requires = >=3.8,<3.11
 packages = 
 	chainlib.eth
 	chainlib.eth.dialect
 	chainlib.eth.runnable
 	chainlib.eth.pytest
 	chainlib.eth.unittest
 	chainlib.eth.cli
```

