# Comparing `tmp/pih-1.48044.tar.gz` & `tmp/pih-1.48045.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48044.tar", last modified: Sat Aug  5 15:13:46 2023, max compression
+gzip compressed data, was "pih-1.48045.tar", last modified: Sat Aug  5 15:16:24 2023, max compression
```

## Comparing `pih-1.48044.tar` & `pih-1.48045.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 15:13:46.601608 pih-1.48044/
--rw-rw-rw-   0        0        0      261 2023-08-05 15:13:46.585986 pih-1.48044/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 15:13:46.335986 pih-1.48044/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48044/pih/__init__.py
--rw-rw-rw-   0        0        0    20623 2023-08-04 07:31:27.000000 pih-1.48044/pih/collection.py
--rw-rw-rw-   0        0        0    60496 2023-08-05 14:50:54.000000 pih-1.48044/pih/console_api.py
--rw-rw-rw-   0        0        0   109843 2023-08-05 14:58:20.000000 pih-1.48044/pih/const.py
--rw-rw-rw-   0        0        0   321323 2023-08-05 15:13:08.000000 pih-1.48044/pih/pih.py
--rw-rw-rw-   0        0        0    25353 2023-08-05 12:39:59.000000 pih-1.48044/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48044/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48044/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2528 2023-08-05 13:46:18.000000 pih-1.48044/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48044/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48044/pih/service_example.py
--rw-rw-rw-   0        0        0    38354 2023-08-05 14:56:00.000000 pih-1.48044/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48044/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-05 15:13:46.554776 pih-1.48044/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-05 15:13:44.000000 pih-1.48044/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-05 15:13:45.000000 pih-1.48044/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 15:13:44.000000 pih-1.48044/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-05 15:13:45.000000 pih-1.48044/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-05 15:13:45.000000 pih-1.48044/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48044/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-05 15:13:46.601608 pih-1.48044/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 15:16:25.072084 pih-1.48045/
+-rw-rw-rw-   0        0        0      261 2023-08-05 15:16:25.072084 pih-1.48045/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 15:16:24.290878 pih-1.48045/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48045/pih/__init__.py
+-rw-rw-rw-   0        0        0    20623 2023-08-04 07:31:27.000000 pih-1.48045/pih/collection.py
+-rw-rw-rw-   0        0        0    60496 2023-08-05 14:50:54.000000 pih-1.48045/pih/console_api.py
+-rw-rw-rw-   0        0        0   109843 2023-08-05 14:58:20.000000 pih-1.48045/pih/const.py
+-rw-rw-rw-   0        0        0   321319 2023-08-05 15:16:12.000000 pih-1.48045/pih/pih.py
+-rw-rw-rw-   0        0        0    25353 2023-08-05 12:39:59.000000 pih-1.48045/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48045/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48045/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2528 2023-08-05 13:46:18.000000 pih-1.48045/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48045/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48045/pih/service_example.py
+-rw-rw-rw-   0        0        0    38354 2023-08-05 14:56:00.000000 pih-1.48045/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48045/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:16:25.040838 pih-1.48045/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-05 15:16:23.000000 pih-1.48045/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-05 15:16:24.000000 pih-1.48045/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 15:16:23.000000 pih-1.48045/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-05 15:16:23.000000 pih-1.48045/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-05 15:16:23.000000 pih-1.48045/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48045/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 15:16:25.087709 pih-1.48045/setup.cfg
```

### Comparing `pih-1.48044/pih/collection.py` & `pih-1.48045/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/console_api.py` & `pih-1.48045/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/const.py` & `pih-1.48045/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/pih.py` & `pih-1.48045/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1648,15 +1648,15 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
-        value: str = "1.48044"
+        value: str = "1.48045"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2879,15 +2879,15 @@
         @staticmethod
         def get_creation_time(path: str) -> str:
             return os.path.getctime(PIH.PATH.adapt_if_linux(path))
 
         @staticmethod
         def adapt_if_linux(path: str) -> str:
             path = PIH.PATH.standarted(path)
-            if not PIH.OS.is_linux():
+            if PIH.OS.is_linux():
                 alias: str = PATH_FACADE.VALUE
                 if path.find(alias) == 0:
                     path = path[len(alias):]
                     path = PATHS.FACADE.LINUX_MOUNT_POINT_PATH + path
             return path
 
         @staticmethod
```

### Comparing `pih-1.48044/pih/rpc.py` & `pih-1.48045/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/rpcCommandCall_pb2.py` & `pih-1.48045/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48045/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/rpc_collection.py` & `pih-1.48045/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/rpc_const.py` & `pih-1.48045/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/service_example.py` & `pih-1.48045/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/tools.py` & `pih-1.48045/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih/widgets.py` & `pih-1.48045/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48044/pih_setup.py` & `pih-1.48045/pih_setup.py`

 * *Files identical despite different names*

