# Comparing `tmp/chainsyncer-0.7.2.tar.gz` & `tmp/chainsyncer-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainsyncer-0.7.2.tar", last modified: Mon Nov 14 08:11:48 2022, max compression
+gzip compressed data, was "chainsyncer-0.8.0.tar", last modified: Sun Aug  6 13:04:36 2023, max compression
```

## Comparing `chainsyncer-0.7.2.tar` & `chainsyncer-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.156628 chainsyncer-0.7.2/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:23:41.000000 chainsyncer-0.7.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2022-11-14 07:23:41.000000 chainsyncer-0.7.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      763 2022-11-14 08:11:48.156628 chainsyncer-0.7.2/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:19:26.000000 chainsyncer-0.7.2/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:23:01.000000 chainsyncer-0.7.2/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/
--rw-r--r--   0 lash      (1000) lash      (1000)       31 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      697 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)       90 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/cli/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      618 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/cli/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/data/
--rw-r--r--   0 lash      (1000) lash      (1000)      132 2022-05-13 06:47:02.000000 chainsyncer-0.7.2/chainsyncer/data/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/data/config/syncer.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/driver/
--rw-r--r--   0 lash      (1000) lash      (1000)       29 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/driver/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4274 2022-11-11 05:58:04.000000 chainsyncer-0.7.2/chainsyncer/driver/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2062 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/driver/chain_interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1145 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3582 2022-11-11 05:58:04.000000 chainsyncer-0.7.2/chainsyncer/filter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3308 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/runnable/unlock.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1163 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1424 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer/store/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13085 2022-11-14 07:23:41.000000 chainsyncer-0.7.2/chainsyncer/store/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3010 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/store/fs.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1001 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/store/mem.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2070 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/store/rocksdb.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.156628 chainsyncer-0.7.2/chainsyncer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/chainsyncer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6936 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7544 2022-10-13 07:54:43.000000 chainsyncer-0.7.2/chainsyncer/unittest/store.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-14 08:11:48.153294 chainsyncer-0.7.2/chainsyncer.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      763 2022-11-14 08:11:48.000000 chainsyncer-0.7.2/chainsyncer.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      932 2022-11-14 08:11:48.000000 chainsyncer-0.7.2/chainsyncer.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-11-14 08:11:48.000000 chainsyncer-0.7.2/chainsyncer.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2022-11-14 08:11:48.000000 chainsyncer-0.7.2/chainsyncer.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      176 2022-11-14 08:11:48.000000 chainsyncer-0.7.2/chainsyncer.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2022-11-14 08:11:48.000000 chainsyncer-0.7.2/chainsyncer.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       74 2022-11-14 07:23:41.000000 chainsyncer-0.7.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      957 2022-11-14 08:11:48.156628 chainsyncer-0.7.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      592 2022-08-13 18:16:03.000000 chainsyncer-0.7.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-14 03:38:11.000000 chainsyncer-0.7.2/sql_requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      135 2022-01-30 09:51:34.000000 chainsyncer-0.7.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      695 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       31 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      697 2023-08-06 11:56:37.000000 chainsyncer-0.8.0/chainsyncer/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       90 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/cli/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      618 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/cli/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)      132 2022-05-13 06:47:02.000000 chainsyncer-0.8.0/chainsyncer/data/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/data/config/syncer.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/driver/
+-rw-r--r--   0 lash      (1000) lash      (1000)       29 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/driver/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4274 2023-04-22 20:26:06.000000 chainsyncer-0.8.0/chainsyncer/driver/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3071 2023-08-06 13:01:13.000000 chainsyncer-0.8.0/chainsyncer/driver/chain_interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2848 2023-08-06 12:22:53.000000 chainsyncer-0.8.0/chainsyncer/driver/chain_interface_new.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1814 2023-02-26 19:42:52.000000 chainsyncer-0.8.0/chainsyncer/driver/chain_interface_race.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1145 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3582 2023-04-22 20:26:06.000000 chainsyncer-0.8.0/chainsyncer/filter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3308 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/runnable/unlock.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1163 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1424 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13085 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/chainsyncer/store/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3010 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/store/fs.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1001 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/store/mem.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2070 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/store/rocksdb.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7016 2023-08-06 12:44:01.000000 chainsyncer-0.8.0/chainsyncer/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7544 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/unittest/store.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      695 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1079 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      176 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       74 2023-08-06 12:57:18.000000 chainsyncer-0.8.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      889 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      592 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-14 03:38:11.000000 chainsyncer-0.8.0/sql_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1670 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1426 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/tests/test_driver.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    10649 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/tests/test_filter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4622 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/tests/test_session.py
```

### Comparing `chainsyncer-0.7.2/LICENSE` & `chainsyncer-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/PKG-INFO` & `chainsyncer-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: chainsyncer
-Version: 0.7.2
+Version: 0.8.0
 Summary: Generic blockchain syncer driver
-Home-page: https://git.defalsify.org/chainsyncer.git
+Home-page: https://git.defalsify.org/chainsyncer
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
-License: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+License: AGPLv3+
 Keywords: cryptocurrency
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `chainsyncer-0.7.2/WAIVER` & `chainsyncer-0.8.0/WAIVER`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/WAIVER.asc` & `chainsyncer-0.8.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/cli/arg.py` & `chainsyncer-0.8.0/chainsyncer/cli/arg.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/cli/config.py` & `chainsyncer-0.8.0/chainsyncer/cli/config.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/driver/base.py` & `chainsyncer-0.8.0/chainsyncer/driver/base.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/driver/chain_interface.py` & `chainsyncer-0.8.0/chainsyncer/driver/chain_interface_new.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+# standard imports
+import logging
+
 # external imports
 from chainlib.error import RPCException
 
 # local imports
 from chainsyncer.error import NoBlockForYou
 from chainsyncer.driver import SyncDriver
 
+logg = logging.getLogger(__name__)
+
 
 class ChainInterfaceDriver(SyncDriver):
 
     def __init__(self, store, chain_interface, offset=0, target=-1, pre_callback=None, post_callback=None, block_callback=None, idle_callback=None):
         super(ChainInterfaceDriver, self).__init__(store, offset=offset, target=target, pre_callback=pre_callback, post_callback=post_callback, block_callback=block_callback, idle_callback=idle_callback)
         self.chain_interface = chain_interface
 
@@ -30,28 +35,60 @@
         if r == None:
             raise NoBlockForYou()
         b = self.chain_interface.block_from_src(r)
         b.txs = b.txs[item.tx_cursor:]
 
         return b
 
+    def merge_rcpts_single(self, conn, txs):
+        i = 0
+        for j in range(len(txs)):
+            o = self.chain_interface.tx_receipt(tx.hash)
+            r = conn.do(o)
+            tx[j].apply_receipt(r)
+            i += 1
+        return i
+
+
+    def merge_rcpts(self, conn, txs):
+        if self.chain_interface.batch_limit == 1:
+            return merge_rcpts_single(self, conn, txs)
+
+        rcpts = []
+        for tx in txs:
+            rcpts.append(self.chain_interface.tx_receipt(tx.hash))
+
+        rcpts_r = conn.do(rcpts)
+        i = 0
+        for j in range(len(txs)):
+            rcpt = rcpts_r[j]
+            if rcpt != None:
+                txs[j].apply_receipt(self.chain_interface.src_normalize(rcpt))
+            i += 1
+
+        return i
+
 
     def process(self, conn, item, block):
-        tx_src = None
+        txs = []
         i = item.tx_cursor
         while True:
             # handle block objects regardless of whether the tx data is embedded or not
             try:
                 tx = block.tx(i)
             except AttributeError:
                 tx_hash = block.txs[i]
                 o = self.chain_interface.tx_by_hash(tx_hash, block=block)
                 r = conn.do(o)
-                #tx = self.chain_interface.tx_from_src(tx_src, block=block)
-
-            rcpt = conn.do(self.chain_interface.tx_receipt(tx.hash))
-            if rcpt != None:
-                tx.apply_receipt(self.chain_interface.src_normalize(rcpt))
+            except IndexError:
+                break
+            txs.append(tx)
+            i += 1
+  
+        j = len(txs)
+        i = 0
+        while i < j:
+            i += self.merge_rcpts(conn, txs)
 
+        for tx in txs:
             self.process_single(conn, block, tx)
-                        
-            i += 1
+        raise IndexError()
```

### Comparing `chainsyncer-0.7.2/chainsyncer/error.py` & `chainsyncer-0.8.0/chainsyncer/error.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/filter.py` & `chainsyncer-0.8.0/chainsyncer/filter.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/runnable/unlock.py` & `chainsyncer-0.8.0/chainsyncer/runnable/unlock.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/session.py` & `chainsyncer-0.8.0/chainsyncer/session.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/settings.py` & `chainsyncer-0.8.0/chainsyncer/settings.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/store/base.py` & `chainsyncer-0.8.0/chainsyncer/store/base.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/store/fs.py` & `chainsyncer-0.8.0/chainsyncer/store/fs.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/store/mem.py` & `chainsyncer-0.8.0/chainsyncer/store/mem.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/store/rocksdb.py` & `chainsyncer-0.8.0/chainsyncer/store/rocksdb.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer/unittest/base.py` & `chainsyncer-0.8.0/chainsyncer/unittest/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,14 +217,18 @@
             self.process_single(conn, block, tx)
             item.next()
             i += 1
 
 
 class MockChainInterface:
 
+    def __init__(self, batch_limit=1):
+        self.batch_limit = batch_limit
+
+
     def block_by_number(self, number):
         return ('block_by_number', number,)
 
 
     def tx_by_hash(self, hsh):
         return ('tx_by_hash', hsh,)
```

### Comparing `chainsyncer-0.7.2/chainsyncer/unittest/store.py` & `chainsyncer-0.8.0/chainsyncer/unittest/store.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.7.2/chainsyncer.egg-info/PKG-INFO` & `chainsyncer-0.8.0/chainsyncer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: chainsyncer
-Version: 0.7.2
+Version: 0.8.0
 Summary: Generic blockchain syncer driver
-Home-page: https://git.defalsify.org/chainsyncer.git
+Home-page: https://git.defalsify.org/chainsyncer
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
-License: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+License: AGPLv3+
 Keywords: cryptocurrency
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `chainsyncer-0.7.2/chainsyncer.egg-info/SOURCES.txt` & `chainsyncer-0.8.0/chainsyncer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 WAIVER
 WAIVER.asc
 requirements.txt
 setup.cfg
 setup.py
 sql_requirements.txt
-test_requirements.txt
 chainsyncer/__init__.py
 chainsyncer/error.py
 chainsyncer/filter.py
 chainsyncer/session.py
 chainsyncer/settings.py
 chainsyncer.egg-info/PKG-INFO
 chainsyncer.egg-info/SOURCES.txt
@@ -22,16 +21,22 @@
 chainsyncer/cli/base.py
 chainsyncer/cli/config.py
 chainsyncer/data/__init__.py
 chainsyncer/data/config/syncer.ini
 chainsyncer/driver/__init__.py
 chainsyncer/driver/base.py
 chainsyncer/driver/chain_interface.py
+chainsyncer/driver/chain_interface_new.py
+chainsyncer/driver/chain_interface_race.py
 chainsyncer/runnable/unlock.py
 chainsyncer/store/__init__.py
 chainsyncer/store/base.py
 chainsyncer/store/fs.py
 chainsyncer/store/mem.py
 chainsyncer/store/rocksdb.py
 chainsyncer/unittest/__init__.py
 chainsyncer/unittest/base.py
-chainsyncer/unittest/store.py
+chainsyncer/unittest/store.py
+tests/test_basic.py
+tests/test_driver.py
+tests/test_filter.py
+tests/test_session.py
```

### Comparing `chainsyncer-0.7.2/setup.cfg` & `chainsyncer-0.8.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = chainsyncer
-version = 0.7.2
+version = 0.8.0
 description = Generic blockchain syncer driver
 author = Louis Holbrook
 author_email = dev@holbrook.no
-url = https://git.defalsify.org/chainsyncer.git
+url = https://git.defalsify.org/chainsyncer
 keywords = 
 	cryptocurrency
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 	Topic :: Internet
-license = OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+license = AGPLv3+
 licence_files = 
 	LICENSE
 
 [options]
 include_package_data = True
 python_requires = >= 3.7
 packages =
```

### Comparing `chainsyncer-0.7.2/setup.py` & `chainsyncer-0.8.0/setup.py`

 * *Files identical despite different names*

