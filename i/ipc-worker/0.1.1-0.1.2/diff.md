# Comparing `tmp/ipc_worker-0.1.1-py3-none-any.whl.zip` & `tmp/ipc_worker-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17553 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat       83 b- defN 23-Aug-05 15:13 ipc_worker/__init__.py
--rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 15:32 ipc_worker/ipc_shm_loader.py
--rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 12:22 ipc_worker/ipc_zmq_loader.py
--rw-rw-rw-  2.0 fat      839 b- defN 23-Aug-05 15:11 ipc_worker/utils.py
--rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 12:22 ipc_worker/shm_module/__init__.py
--rw-rw-rw-  2.0 fat     5087 b- defN 23-Aug-05 17:51 ipc_worker/shm_module/ipc_shm.py
--rw-rw-rw-  2.0 fat     8445 b- defN 23-Aug-05 15:16 ipc_worker/shm_module/ipc_shm_utils.py
--rw-rw-rw-  2.0 fat     2194 b- defN 23-Aug-05 15:15 ipc_worker/shm_module/ipc_utils_func.py
--rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 12:22 ipc_worker/zmq_module/__init__.py
--rw-rw-rw-  2.0 fat      878 b- defN 23-Aug-05 15:32 ipc_worker/zmq_module/ipc_utils_func.py
--rw-rw-rw-  2.0 fat     3409 b- defN 23-Aug-05 18:15 ipc_worker/zmq_module/ipc_zmq.py
--rw-rw-rw-  2.0 fat     9009 b- defN 23-Aug-05 17:49 ipc_worker/zmq_module/ipc_zmq_utils.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6757 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1459 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/RECORD
-17 files, 50124 bytes uncompressed, 15129 bytes compressed:  69.8%
+Zip file size: 18289 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat       83 b- defN 23-Aug-06 08:20 ipc_worker/__init__.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-06 08:20 ipc_worker/ipc_shm_loader.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-06 08:20 ipc_worker/ipc_zmq_loader.py
+-rw-rw-rw-  2.0 fat     2842 b- defN 23-Aug-06 09:00 ipc_worker/utils.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-06 08:20 ipc_worker/shm_module/__init__.py
+-rw-rw-rw-  2.0 fat     5336 b- defN 23-Aug-06 09:55 ipc_worker/shm_module/ipc_shm.py
+-rw-rw-rw-  2.0 fat     8445 b- defN 23-Aug-06 08:20 ipc_worker/shm_module/ipc_shm_utils.py
+-rw-rw-rw-  2.0 fat     2194 b- defN 23-Aug-06 08:20 ipc_worker/shm_module/ipc_utils_func.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-06 08:20 ipc_worker/zmq_module/__init__.py
+-rw-rw-rw-  2.0 fat      878 b- defN 23-Aug-06 08:20 ipc_worker/zmq_module/ipc_utils_func.py
+-rw-rw-rw-  2.0 fat     5442 b- defN 23-Aug-06 09:55 ipc_worker/zmq_module/ipc_zmq.py
+-rw-rw-rw-  2.0 fat     7487 b- defN 23-Aug-06 09:12 ipc_worker/zmq_module/ipc_zmq_utils.py
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Aug-06 09:58 ipc_worker-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6538 b- defN 23-Aug-06 09:58 ipc_worker-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-06 09:58 ipc_worker-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-06 09:58 ipc_worker-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1460 b- defN 23-Aug-06 09:58 ipc_worker-0.1.2.dist-info/RECORD
+17 files, 52669 bytes uncompressed, 15865 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: ipc_worker/zmq_module/ipc_zmq.py
 Comment: 
 
 Filename: ipc_worker/zmq_module/ipc_zmq_utils.py
 Comment: 
 
-Filename: ipc_worker-0.1.1.dist-info/LICENSE
+Filename: ipc_worker-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: ipc_worker-0.1.1.dist-info/METADATA
+Filename: ipc_worker-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: ipc_worker-0.1.1.dist-info/WHEEL
+Filename: ipc_worker-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: ipc_worker-0.1.1.dist-info/top_level.txt
+Filename: ipc_worker-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ipc_worker-0.1.1.dist-info/RECORD
+Filename: ipc_worker-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipc_worker/utils.py

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/30 10:22
 # @Author  : tk
 
 import logging
+import time
+from multiprocessing import Queue
+from threading import Lock
+
 from termcolor import colored
 
 
 def set_logger(context, verbose=False):
     # if os.name == 'nt':  # for Windows
     #     return NTLogger(context, verbose)
 
@@ -19,8 +23,59 @@
     console_handler.setLevel(logging.DEBUG if verbose else logging.INFO)
     console_handler.setFormatter(formatter)
     logger.handlers = []
     logger.addHandler(console_handler)
     return logger
 
 
-logger = set_logger(colored('VENTILATOR', 'magenta'))
+logger = set_logger(colored('VENTILATOR', 'magenta'))
+
+
+
+# class RequestInfo:
+#     def __int__(self,queue : Queue):
+#         self.__last_t = time.time()
+#         self.pending_request = {}
+#         self.pending_response = {}
+#         self.locker = Lock()
+#         self.queue = queue
+#
+#     def add_request_id(self, request_id):
+#         self.locker.acquire()
+#         self.pending_request[request_id] = time.time()
+#         self.locker.release()
+#
+#     def __clean__private__(self):
+#         c_t = time.time()
+#         if (c_t - self.__last_t) / 600 > 0:
+#             self.__last_t = c_t
+#             invalid = set({rid for rid, t in self.pending_request.items() if (c_t - t) / 3600 > 0})
+#             logger.debug('remove {}'.format(str(list(invalid))))
+#             for rid in invalid:
+#                 self.pending_request.pop(rid)
+#
+#     def get(self, request_id):
+#         response = None
+#         while True:
+#             is_end = False
+#             self.locker.acquire(timeout=0.005)
+#             if self.locker.locked():
+#                 self.__clean__private__()
+#             if request_id in self.pending_request:
+#                 self.pending_request[request_id] = time.time()
+#                 if request_id in self.pending_response:
+#                     response = self.pending_response.pop(request_id)
+#                     is_end = True
+#                 else:
+#                     r_id, w_id, seq_id, response = self.queue.get()
+#                     if r_id != request_id:
+#                         self.pending_response[r_id] = response
+#                     else:
+#                         is_end = True
+#             else:
+#                 logger.error('bad request_id {}'.format(request_id))
+#                 is_end = True
+#             if self.locker.locked():
+#                 self.locker.release()
+#             if is_end:
+#                 break
+#         return response
```

## ipc_worker/shm_module/ipc_shm.py

```diff
@@ -1,13 +1,15 @@
 #coding: utf-8
+import math
 import multiprocessing
 import time
 from threading import Lock
 from .ipc_shm_utils import SHM_manager,SHM_woker
 import pickle
+from ..utils import logger
 # import numpy as np
 class SHM_process_worker(SHM_woker):
     def __init__(self,*args,**kwargs):
         super(SHM_process_worker,self).__init__(*args,**kwargs)
 
     #Process begin trigger this func
     def run_begin(self):
@@ -96,26 +98,31 @@
         self.request_id += 1
         request_id = self.request_id
         self.pending_request[request_id] = time.time()
         self.__input_queue.put((request_id,pickle.dumps(data)))
         self.locker.release()
         return request_id
 
-    def get(self,request_id):
+    def __clean__private__(self):
         c_t = time.time()
-        if (c_t - self.__last_t) / 600 > 0:
+        if math.floor((c_t - self.__last_t) / 600) > 0:
             self.__last_t = c_t
-            invalid = set({rid for rid, t in self.pending_request.items() if (c_t - t) / 3600 > 0})
+            invalid = set({rid for rid, t in self.pending_request.items() if math.floor((c_t - t) / 3600) > 0})
+            logger.debug('remove {}'.format(str(list(invalid))))
             for rid in invalid:
                 self.pending_request.pop(rid)
 
+    def get(self,request_id):
         response = None
         while True:
             is_end = False
             self.locker.acquire(blocking=False)
+            if self.locker.locked():
+                self.__clean__private__()
+
             if request_id in self.pending_request:
                 self.pending_request[request_id] = time.time()
                 if request_id in self.pending_response:
                     response = self.pending_response.pop(request_id)
                     is_end = True
                 else:
                     r_id,_,seq_id, response = self.__output_queue.get()
```

## ipc_worker/zmq_module/ipc_zmq.py

```diff
@@ -1,15 +1,20 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/29 13:45
 # @Author  : tk
+import math
 import multiprocessing
+import os
 import random
+import threading
 import time
+from threading import Lock
 from .ipc_zmq_utils import ZMQ_manager,ZMQ_sink,ZMQ_worker
 import pickle
+from ..utils import logger
 
 
 
 class ZMQ_process_worker(ZMQ_worker):
     def __init__(self,*args,**kwargs):
         super(ZMQ_process_worker,self).__init__(*args,**kwargs)
 
@@ -59,14 +64,18 @@
                 is_log_time=is_log_time,
                 idx=i,
                 daemon=daemon
             )
             self.__group_idenity.append(identity)
             self.__woker_lst.append(worker)
         self.__last_worker_id = len(self.__group_idenity) - 1
+        self.pending_request = {}
+        self.pending_response = {}
+        self.locker = Lock()
+        self.__last_t = time.time()
     def start(self):
         for w in self.__manager_lst:
             w.start()
 
         for w in self.__manager_lst:
             w.wait_init()
 
@@ -81,21 +90,70 @@
             del w.signal
 
 
     def put(self,data):
         self.__last_worker_id = (self.__last_worker_id + 1 ) % len(self.__group_idenity)
         idenity = self.__group_idenity[self.__last_worker_id]
         request_id = self.__manager_lst[0].put(idenity,pickle.dumps(data))
-        self.__manager_lst[1].add_request_id(request_id)
+        self.locker.acquire()
+        self.pending_request[request_id] = time.time() # (os.getpid(), threading.get_native_id(),time.time())
+        self.locker.release()
         return request_id
 
     def get(self,request_id):
-        d = self.__manager_lst[1].get(request_id)
+        d = self.__get_private__(request_id)
         return d if d is None else pickle.loads(d)
 
+
+    def __clean__private__(self):
+        c_t = time.time()
+        if math.floor((c_t - self.__last_t) / 600) > 0:
+            self.__last_t = c_t
+            invalid = set({rid for rid, t in self.pending_request.items() if math.floor((c_t - t) / 3600) > 0})
+            logger.debug('remove {}'.format(str(list(invalid))))
+            for rid in invalid:
+                self.pending_request.pop(rid)
+
+    def __get_private__(self, request_id):
+        sink = self.__manager_lst[1]
+        response = None
+        is_end = False
+        timeout = 0.005
+        while not is_end:
+            sink.get_signal().wait(timeout)
+            self.locker.acquire(timeout=timeout)
+            if not self.locker.locked():
+                continue
+            if request_id in self.pending_request:
+                self.pending_request[request_id] = time.time()
+                if request_id in self.pending_response:
+                    response = self.pending_response.pop(request_id)
+                    is_end = True
+                else:
+                    r_id, w_id, seq_id, response = sink.get_queue().get()
+                    if r_id != request_id:
+                        self.pending_response[r_id] = response
+                    else:
+                        is_end = True
+            else:
+                logger.error('bad request_id {}'.format(request_id))
+                is_end = True
+            if self.locker.locked():
+                self.locker.release()
+            if is_end:
+                break
+
+        self.locker.acquire()
+        self.__clean__private__()
+        self.locker.release()
+        return response
+
+
+
+
     def join(self):
         for p in self.__manager_lst:
             p.join()
         time.sleep(1)
         for p in self.__woker_lst:
             p.join()
```

## ipc_worker/zmq_module/ipc_zmq_utils.py

```diff
@@ -108,50 +108,30 @@
 class ZMQ_sink(Process):
     def __init__(self,queue_size,group_name,evt_quit,daemon=False):
         super(ZMQ_sink,self).__init__(daemon=daemon)
 
         self.group_name = group_name
         self.__is_closed = False
         self.evt_quit = evt_quit
-        self.pending_request = {}
-        self.pending_response = {}
+
         self.queue = Queue(maxsize=queue_size)
         #
-        self.locker = Lock()
+
         self.signal = Event()
         self.addr = None
+
+
     def wait_init(self):
         self.addr = self.queue.get()
 
-    def get(self,request_id):
-        response = None
-        while True:
-            is_end = False
-            self.signal.wait(0.005)
-            self.locker.acquire(timeout=0.005)
-            if request_id in self.pending_request:
-                self.pending_request[request_id] = time.time()
-                if request_id in self.pending_response:
-                    response = self.pending_response.pop(request_id)
-                    self.signal.clear()
-                    is_end = True
-                else:
-                    r_id,w_id,seq_id,response = self.queue.get()
-                    if r_id != request_id:
-                        self.pending_response[r_id] = response
-                    else:
-                        is_end = True
-            else:
-                logger.error('bad request_id {}'.format(request_id))
-                is_end = True
-            if self.locker.locked():
-                self.locker.release()
-            if is_end:
-                break
-        return response
+    def get_queue(self) -> Queue:
+        return self.queue
+
+    def get_signal(self) -> Event:
+        return self.signal
 
     def __processinit__(self):
         self.context = zmq.Context()
         self.receiver = self.context.socket(zmq.PULL)
         self.receiver.setsockopt(zmq.LINGER, 0)
         # self.receiver.bind('tcp://*:{}'.format(self.port_out))
         self.addr = auto_bind(self.receiver)
@@ -170,41 +150,29 @@
             ...
 
 
 
     def run(self):
         self.__processinit__()
         try:
-            last_t = time.time()
             while not self.evt_quit.is_set():
                 request_id,w_id,seq_id,response = self.receiver.recv_multipart()
                 if self.__is_closed:
                     break
-
-                c_t = time.time()
-                if (c_t - last_t) / 600 > 0:
-                    last_t = c_t
-                    invalid = set({rid for rid, t in self.pending_request.items() if (c_t - t) / 3600 > 0})
-                    for rid in invalid:
-                        self.pending_request.pop(rid)
-
                 r_id = int.from_bytes(request_id, byteorder='little', signed=False)
                 w_id = int.from_bytes(w_id, byteorder='little', signed=False)
                 seq_id = int.from_bytes(seq_id, byteorder='little', signed=False)
                 self.queue.put((r_id,w_id,seq_id,response))
                 self.signal.set()
         except Exception as e:
             print(e)
         self.release()
 
 
-    def add_request_id(self,request_id):
-        self.locker.acquire()
-        self.pending_request[request_id] = time.time()
-        self.locker.release()
+
 
 
 
 class ZMQ_manager(Process):
     def __init__(self,idx,queue_size,group_name,evt_quit,daemon=False):
         super(ZMQ_manager, self).__init__(daemon=daemon)
         self.group_name = group_name
```

## Comparing `ipc_worker-0.1.1.dist-info/LICENSE` & `ipc_worker-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ipc_worker-0.1.1.dist-info/METADATA` & `ipc_worker-0.1.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-Metadata-Version: 2.1
-Name: ipc-worker
-Version: 0.1.1
-Summary: ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
-Home-page: https://github.com/ssbuild/ipc_worker
-Author: ssbuild
-Author-email: 9727464@qq.com
-License: Apache 2.0
-Keywords: ipc-worker,ipc_worker,ipc,process worker,ipc,ipc mq,fast-ipc,process ipc
-Platform: win32_AMD64
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: termcolor
-
-ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
-
-```py
-support share memory (py>=3.8 and linux) and mq process worker (py >=3.6)
-
-```
-```py
-# -*- coding: utf-8 -*-
-# @Time    : 2021/11/23 9:35
-
-'''
-demo share memrory
-recommended system linux and python >= 3.8
-    recommended linux
-    python 3.8
-
-Do not recommended run in windows , it will report an error as follow
-    RuntimeError:
-            An attempt has been made to start a new process before the
-            current process has finished its bootstrapping phase.
-
-'''
-import multiprocessing
-import os
-from ipc_worker import logger
-from ipc_worker.ipc_shm_loader import IPC_shm,SHM_process_worker
-
-class My_worker(SHM_process_worker):
-    def __init__(self,config,*args,**kwargs):
-        super(My_worker,self).__init__(*args,**kwargs)
-        #config info , use by yourself
-
-        logger.info('Process id {}, group name {} ,shm name {}'.format(self._idx,self._group_name,self._shm_name))
-        logger.info(config)
-        self.config = config
-
-
-    #Process begin trigger this func
-    def run_begin(self):
-        logger.info('worker pid {}...'.format(os.getpid()))
-        self.handle = None
-        pass
-
-    # Process end trigger this func
-    def run_end(self):
-        if self.handle is not None:
-            pass
-
-    #any data put will trigger this func
-    def run_once(self,request_data):
-        #process request_data
-        if isinstance(request_data,dict):
-            request_data['b']  = 200
-        if self.handle is not None:
-            #do some thing
-            pass
-        return request_data
-
-
-if __name__ == '__main__':
-    config = {
-        "anything" : "anything",
-        "aa": 100
-    }
-
-    evt_quit = multiprocessing.Manager().Event()
-
-    # group_name 为共享内存组名,需唯一
-    # manager is an agent  and act as a load balancing
-    # worker is real doing your work
-    instance = IPC_shm(
-        CLS_worker=My_worker,
-        worker_args=(config,),  # must be tuple
-        worker_num=10,  # number of worker Process
-        manager_num=2,  # number of agent Process
-        group_name='serving_shm',  # share memory name
-        shm_size=1 * 1024 * 1024,  # share memory size
-        queue_size=20,  # recv queue size
-        is_log_time=True,  # whether log compute time
-        daemon=False,
-    )
-
-    instance.start()
-
-    #demo produce and consume message , you can process by http
-    for i in range(10):
-        print('produce message')
-        data = {"a" : 100}
-        request_id = instance.put(data)
-        data = instance.get(request_id)
-        print('get process result',data)
-    try:
-        instance.join()
-    except Exception as e:
-        evt_quit.set()
-        instance.terminate()
-
-    del evt_quit
-```
-```py
-# -*- coding: utf-8 -*-
-# @Time    : 2021/11/29 15:06
-# @Author  : tk
-import multiprocessing
-import os
-from ipc_worker import logger
-from ipc_worker.ipc_zmq_loader import IPC_zmq,ZMQ_process_worker
-'''
-    demo ZMQ depend zmq
-    pip install pyzmq
-    
-    test pass >= python3.6
-'''
-
-tmp_dir = './tmp'
-if not os.path.exists(tmp_dir):
-    os.mkdir(tmp_dir)
-
-os.environ['ZEROMQ_SOCK_TMP_DIR'] = tmp_dir
-
-class My_worker(ZMQ_process_worker):
-    def __init__(self,config,*args,**kwargs):
-        super(My_worker,self).__init__(*args,**kwargs)
-        #config info , use by yourself
-        logger.info('Process id {}, group name {} , identity {}'.format(self._idx,self._group_name,self._identity))
-        logger.info(config)
-        self.config = config
-
-    #Process begin trigger this func
-    def run_begin(self):
-        logger.info('worker pid {}...'.format(os.getpid()))
-        self.handle = None
-        pass
-
-    # Process end trigger this func
-    def run_end(self):
-        if self.handle is not None:
-            pass
-
-    #any data put will trigger this func
-    def run_once(self,request_data):
-        #process request_data
-        if isinstance(request_data,dict):
-            request_data['b'] = 200
-        if self.handle is not None:
-            #do some thing
-            pass
-        return request_data
-
-
-if __name__ == '__main__':
-    config = {
-        "anything" : "anything",
-        "aa": 100
-    }
-
-    evt_quit = multiprocessing.Manager().Event()
-
-    # group_name 为共享内存组名,需唯一
-    # manager is an agent  and act as a load balancing
-    # worker is real doing your work
-    instance = IPC_zmq(
-        CLS_worker=My_worker,
-        worker_args=(config,),  # must be tuple
-        worker_num=10,  # number of worker Process
-        group_name='serving_zmq',  # share memory name
-        evt_quit=evt_quit,
-        queue_size=20,  # recv queue size
-        is_log_time=True,  # whether log compute time
-        daemon=False,
-    )
-    instance.start()
-
-    #demo produce and consume message , you can process by http
-    for i in range(10):
-        data = {"a" : 100}
-        request_id = instance.put(data)
-
-        data = instance.get(request_id)
-        print('get process result',request_id,data)
-    try:
-        instance.join()
-    except Exception as e:
-        evt_quit.set()
-        instance.terminate()
-    del evt_quit
-```
+Metadata-Version: 2.1
+Name: ipc-worker
+Version: 0.1.2
+Summary: ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
+Home-page: https://github.com/ssbuild/ipc_worker
+Author: ssbuild
+Author-email: 9727464@qq.com
+License: Apache 2.0
+Keywords: ipc-worker,ipc_worker,ipc,process worker,ipc,ipc mq,fast-ipc,process ipc
+Platform: win32_AMD64
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: termcolor
+
+ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
+
+```py
+support share memory (py>=3.8 and linux) and mq process worker (py >=3.6)
+
+```
+```py
+# -*- coding: utf-8 -*-
+# @Time    : 2021/11/23 9:35
+
+'''
+demo share memrory
+recommended system linux and python >= 3.8
+    recommended linux
+    python 3.8
+
+Do not recommended run in windows , it will report an error as follow
+    RuntimeError:
+            An attempt has been made to start a new process before the
+            current process has finished its bootstrapping phase.
+
+'''
+import multiprocessing
+import os
+from ipc_worker import logger
+from ipc_worker.ipc_shm_loader import IPC_shm,SHM_process_worker
+
+class My_worker(SHM_process_worker):
+    def __init__(self,config,*args,**kwargs):
+        super(My_worker,self).__init__(*args,**kwargs)
+        #config info , use by yourself
+
+        logger.info('Process id {}, group name {} ,shm name {}'.format(self._idx,self._group_name,self._shm_name))
+        logger.info(config)
+        self.config = config
+
+
+    #Process begin trigger this func
+    def run_begin(self):
+        logger.info('worker pid {}...'.format(os.getpid()))
+        self.handle = None
+        pass
+
+    # Process end trigger this func
+    def run_end(self):
+        if self.handle is not None:
+            pass
+
+    #any data put will trigger this func
+    def run_once(self,request_data):
+        #process request_data
+        if isinstance(request_data,dict):
+            request_data['b']  = 200
+        if self.handle is not None:
+            #do some thing
+            pass
+        return request_data
+
+
+if __name__ == '__main__':
+    config = {
+        "anything" : "anything",
+        "aa": 100
+    }
+
+    evt_quit = multiprocessing.Manager().Event()
+
+    # group_name 为共享内存组名,需唯一
+    # manager is an agent  and act as a load balancing
+    # worker is real doing your work
+    instance = IPC_shm(
+        CLS_worker=My_worker,
+        worker_args=(config,),  # must be tuple
+        worker_num=10,  # number of worker Process
+        manager_num=2,  # number of agent Process
+        group_name='serving_shm',  # share memory name
+        shm_size=1 * 1024 * 1024,  # share memory size
+        queue_size=20,  # recv queue size
+        is_log_time=True,  # whether log compute time
+        daemon=False,
+    )
+
+    instance.start()
+
+    #demo produce and consume message , you can process by http
+    for i in range(10):
+        print('produce message')
+        data = {"a" : 100}
+        request_id = instance.put(data)
+        data = instance.get(request_id)
+        print('get process result',data)
+    try:
+        instance.join()
+    except Exception as e:
+        evt_quit.set()
+        instance.terminate()
+
+    del evt_quit
+```
+```py
+# -*- coding: utf-8 -*-
+# @Time    : 2021/11/29 15:06
+# @Author  : tk
+import multiprocessing
+import os
+from ipc_worker import logger
+from ipc_worker.ipc_zmq_loader import IPC_zmq,ZMQ_process_worker
+'''
+    demo ZMQ depend zmq
+    pip install pyzmq
+    
+    test pass >= python3.6
+'''
+
+tmp_dir = './tmp'
+if not os.path.exists(tmp_dir):
+    os.mkdir(tmp_dir)
+
+os.environ['ZEROMQ_SOCK_TMP_DIR'] = tmp_dir
+
+class My_worker(ZMQ_process_worker):
+    def __init__(self,config,*args,**kwargs):
+        super(My_worker,self).__init__(*args,**kwargs)
+        #config info , use by yourself
+        logger.info('Process id {}, group name {} , identity {}'.format(self._idx,self._group_name,self._identity))
+        logger.info(config)
+        self.config = config
+
+    #Process begin trigger this func
+    def run_begin(self):
+        logger.info('worker pid {}...'.format(os.getpid()))
+        self.handle = None
+        pass
+
+    # Process end trigger this func
+    def run_end(self):
+        if self.handle is not None:
+            pass
+
+    #any data put will trigger this func
+    def run_once(self,request_data):
+        #process request_data
+        if isinstance(request_data,dict):
+            request_data['b'] = 200
+        if self.handle is not None:
+            #do some thing
+            pass
+        return request_data
+
+
+if __name__ == '__main__':
+    config = {
+        "anything" : "anything",
+        "aa": 100
+    }
+
+    evt_quit = multiprocessing.Manager().Event()
+
+    # group_name 为共享内存组名,需唯一
+    # manager is an agent  and act as a load balancing
+    # worker is real doing your work
+    instance = IPC_zmq(
+        CLS_worker=My_worker,
+        worker_args=(config,),  # must be tuple
+        worker_num=10,  # number of worker Process
+        group_name='serving_zmq',  # share memory name
+        evt_quit=evt_quit,
+        queue_size=20,  # recv queue size
+        is_log_time=True,  # whether log compute time
+        daemon=False,
+    )
+    instance.start()
+
+    #demo produce and consume message , you can process by http
+    for i in range(10):
+        data = {"a" : 100}
+        request_id = instance.put(data)
+
+        data = instance.get(request_id)
+        print('get process result',request_id,data)
+    try:
+        instance.join()
+    except Exception as e:
+        evt_quit.set()
+        instance.terminate()
+    del evt_quit
+```
```

## Comparing `ipc_worker-0.1.1.dist-info/RECORD` & `ipc_worker-0.1.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ipc_worker/__init__.py,sha256=fK3ASYKB5vx3P71YnrPzgFtrrpc0nuv7NrbDXjh0KmA,83
 ipc_worker/ipc_shm_loader.py,sha256=xKqpZQPfNtcUgVVt5iOlEqVWCt7ws5uvU6GsuqT8eeE,126
 ipc_worker/ipc_zmq_loader.py,sha256=eGAAxWe19H51mWZsW675sGY2YrMXI1m6e4L1VjjRqPY,126
-ipc_worker/utils.py,sha256=UHkLeqz89qK6PCstESVUXHKjHt8isEMbE_ryDlBC2No,839
+ipc_worker/utils.py,sha256=ybO0G33mcfi5xWj-FvtkNkYv3zvheHnnZN7Ur6MHM4Y,2842
 ipc_worker/shm_module/__init__.py,sha256=xiptFd-Wn-CHHHrn76PjheyxuIQKmTfEbPKejYxb84Q,126
-ipc_worker/shm_module/ipc_shm.py,sha256=TRW89Lw37Z0IwlmU3JYbEzYFav3PN8qw4h70AsSRaOY,5087
+ipc_worker/shm_module/ipc_shm.py,sha256=cu43BNv0_bp3W3E0M-eAj4I7rsXRIdFW9-Y5kWaZdAo,5336
 ipc_worker/shm_module/ipc_shm_utils.py,sha256=UiCuddy0ebVAosR3u5yeVWpKhT1LAKWaPMFBius3VCI,8445
 ipc_worker/shm_module/ipc_utils_func.py,sha256=YNkqqMDFhMFgMSE1GEvBlxNR3g_HIVZGy0PySZU-lCY,2194
 ipc_worker/zmq_module/__init__.py,sha256=4HM8jgaXuGG3APy0jqsqcT-edJ09KBfTO64YKO0XMlg,126
 ipc_worker/zmq_module/ipc_utils_func.py,sha256=zvz9DZ99RMBvGHsFbAhNQ0LWn-5eIn2K8mh4cJJyCc0,878
-ipc_worker/zmq_module/ipc_zmq.py,sha256=aIQKub_EOgqEj1Zfke9djLliZqfZRw0E7C_fR2W72a0,3409
-ipc_worker/zmq_module/ipc_zmq_utils.py,sha256=LrLgXXx46H3xep1nmtyYg2_aXscYvkviAwCSG90uKDc,9009
-ipc_worker-0.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-ipc_worker-0.1.1.dist-info/METADATA,sha256=W591Fgq9RG90AujvN-zVZxbeCaHCtmSHbKSrfY7YAVo,6757
-ipc_worker-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ipc_worker-0.1.1.dist-info/top_level.txt,sha256=Nt7KccWqNby43j5fBuu3aSszZ17RHYqfHNdgT3LkfgQ,11
-ipc_worker-0.1.1.dist-info/RECORD,,
+ipc_worker/zmq_module/ipc_zmq.py,sha256=dlHHiqGcXLrNBLwyzx1gYJ2SBzanX_aVcDEpvfSvP0M,5442
+ipc_worker/zmq_module/ipc_zmq_utils.py,sha256=yf6rBHEs3pY73bfXDdu2Zs5f3CgLJK5CLrdWEQ5J5wc,7487
+ipc_worker-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ipc_worker-0.1.2.dist-info/METADATA,sha256=LYYu5Ql13a_wrLk_uHLs-qL2ytZg3fdHgYuM-kj7Who,6538
+ipc_worker-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+ipc_worker-0.1.2.dist-info/top_level.txt,sha256=Nt7KccWqNby43j5fBuu3aSszZ17RHYqfHNdgT3LkfgQ,11
+ipc_worker-0.1.2.dist-info/RECORD,,
```

