# Comparing `tmp/eniris-0.7.6.tar.gz` & `tmp/eniris-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.7.6.tar", last modified: Sun Aug  6 20:49:20 2023, max compression
+gzip compressed data, was "eniris-0.7.7.tar", last modified: Sun Aug  6 20:56:29 2023, max compression
```

## Comparing `eniris-0.7.6.tar` & `eniris-0.7.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 20:49:11.000000 eniris-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 20:49:20.852753 eniris-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 20:49:11.000000 eniris-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.848753 eniris-0.7.6/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/point/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/point/writer/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/telemessage/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/telemessage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/telemessage/writer/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/pooled.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.848753 eniris-0.7.6/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:49:20.852753 eniris-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-06 20:49:11.000000 eniris-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.499479 eniris-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 20:56:20.000000 eniris-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 20:56:29.499479 eniris-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 20:56:20.000000 eniris-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.495479 eniris-0.7.7/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.495479 eniris-0.7.7/eniris/point/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.499479 eniris-0.7.7/eniris/point/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/writer/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/writer/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/writer/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/point/writer/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.499479 eniris-0.7.7/eniris/telemessage/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/telemessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/telemessage/telemessage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.499479 eniris-0.7.7/eniris/telemessage/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/telemessage/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/telemessage/writer/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/telemessage/writer/pooled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-06 20:56:20.000000 eniris-0.7.7/eniris/telemessage/writer/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:56:29.495479 eniris-0.7.7/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 20:56:29.000000 eniris-0.7.7/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 20:56:29.000000 eniris-0.7.7/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:56:29.000000 eniris-0.7.7/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 20:56:29.000000 eniris-0.7.7/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 20:56:29.000000 eniris-0.7.7/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:56:29.499479 eniris-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-06 20:56:20.000000 eniris-0.7.7/setup.py
```

### Comparing `eniris-0.7.6/LICENSE` & `eniris-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/PKG-INFO` & `eniris-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.6
+Version: 0.7.7
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.6.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.7.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `eniris-0.7.6/README.md` & `eniris-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/driver.py` & `eniris-0.7.7/eniris/driver.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/point/namespace.py` & `eniris-0.7.7/eniris/point/namespace.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/point/point.py` & `eniris-0.7.7/eniris/point/point.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/point/writer/buffered.py` & `eniris-0.7.7/eniris/point/writer/buffered.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/point/writer/direct.py` & `eniris-0.7.7/eniris/point/writer/direct.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/point/writer/filter.py` & `eniris-0.7.7/eniris/point/writer/filter.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/point/writer/writer.py` & `eniris-0.7.7/eniris/point/writer/writer.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/telemessage/telemessage.py` & `eniris-0.7.7/eniris/telemessage/telemessage.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/telemessage/writer/direct.py` & `eniris-0.7.7/eniris/telemessage/writer/direct.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris/telemessage/writer/pooled.py` & `eniris-0.7.7/eniris/telemessage/writer/pooled.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,19 +151,18 @@
         return self._scheduledDt < other._scheduledDt
   
   # Note, we assume that no other threads are trying to modify the scheduledDt when comparing elements
   def __eq__(self, other):
         return self._scheduledDt == other._scheduledDt
 
 class TelemessageWrapperQueue:
-  def __init__(self, waitingMessages: list[TelemessageWrapper]=[], maximumRetries:int=4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60, retryStatusCodes:set[int]=set([HTTPStatus.TOO_MANY_REQUESTS,HTTPStatus.INTERNAL_SERVER_ERROR,HTTPStatus.SERVICE_UNAVAILABLE])):
+  def __init__(self, waitingMessages: list[TelemessageWrapper]=[], maximumRetries:int=4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60):
     self.maximumRetries = maximumRetries
     self.initialRetryDelayS = initialRetryDelayS
     self.maximumRetryDelayS = maximumRetryDelayS
-    self.retryStatusCodes = retryStatusCodes
     self._lock = RLock()
     self._activeMessages: dict[str, TelemessageWrapper] = dict()
     self._waitingMessages = list(waitingMessages)
     self._moreMessagesOrStoppingCondition: Condition = Condition(self._lock)
     self._newMessageOrStoppingCondition: Condition = Condition(self._lock)
     self._isStopping = False
 
@@ -221,22 +220,24 @@
       self._isStopping = True
       self._moreMessagesOrStoppingCondition.notifyAll()
       self._newMessageOrStoppingCondition.notify_all()
 
 class PooledTelemessageWriterDaemon(Thread):
   def __init__(self, queue: TelemessageWrapperQueue,
                url:str="https://neodata-ingress.eniris.be/v1/telemetry", params:dict[str, str]={}, authorizationHeaderFunction:'Callable|None'=None, timeoutS:float=60,
+               retryStatusCodes:set[int]=set([HTTPStatus.TOO_MANY_REQUESTS,HTTPStatus.INTERNAL_SERVER_ERROR,HTTPStatus.SERVICE_UNAVAILABLE]),
                session:requests.Session=None):
     super().__init__()
     self.daemon = True
     self.queue = queue
     self.url = url
     self.params = params
     self.authorizationHeaderFunction = authorizationHeaderFunction
     self.timeoutS = timeoutS
+    self.retryStatusCodes = retryStatusCodes
     self.session = requests.Session() if session is None else session
 
   def run(self):
     logging.debug("Started PooledTelemessageWriterDaemon")
     while True:
       tmw = self.queue.onWaitingToActive()
       if tmw is None:
@@ -329,18 +330,19 @@
         session (requests.Session, optional): A session object to use for all calls. If None, a requests.Session without extra options is created. Defaults to None
         maximumRetries (int, optional): How many times to try again in case of a failure. Defaults to 4
         initialRetryDelayS (int, optional): The initial delay between successive retries in seconds. Defaults to 1
         maximumRetryDelayS (int, optional): The maximum delay between successive retries in seconds. Defaults to 60
         retryStatusCodes (set[str], optional): A set of all response code for which a retry attempt must be made. Defaults to {429, 500, 503}
     """
     waitingMessages: list[TelemessageWrapper] = [] if snapshotFolder is None else TelemessageWrapper.loadSnapshotsFromDirectory(snapshotFolder)
-    self.queue = TelemessageWrapperQueue(waitingMessages, maximumRetries=maximumRetries, initialRetryDelayS=initialRetryDelayS, maximumRetryDelayS=maximumRetryDelayS, retryStatusCodes=retryStatusCodes)
+    self.queue = TelemessageWrapperQueue(waitingMessages, maximumRetries=maximumRetries, initialRetryDelayS=initialRetryDelayS, maximumRetryDelayS=maximumRetryDelayS)
     session = requests.Session() if session is None else session
     self.pool = [PooledTelemessageWriterDaemon(self.queue,
       url=url, params=params, authorizationHeaderFunction=authorizationHeaderFunction, timeoutS=timeoutS,
+      retryStatusCodes=retryStatusCodes,
       session=session) for i in range(poolSize)]
     for d in self.pool:
       d.start()
     if snapshotFolder is not None:
       self.snapshotDaemon = PooledTelemessageSnapshotDaemon(self.queue, snapshotFolder, minimumSnaphotAgeS, maximumSnapshotStorageBytes)
       self.snapshotDaemon.start()
     else:
```

### Comparing `eniris-0.7.6/eniris/telemessage/writer/writer.py` & `eniris-0.7.7/eniris/telemessage/writer/writer.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/eniris.egg-info/PKG-INFO` & `eniris-0.7.7/eniris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.6
+Version: 0.7.7
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.6.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.7.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `eniris-0.7.6/eniris.egg-info/SOURCES.txt` & `eniris-0.7.7/eniris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eniris-0.7.6/setup.py` & `eniris-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,23 @@
   packages = [
     'eniris',
     'eniris.point',
     'eniris.point.writer',
     'eniris.telemessage',
     'eniris.telemessage.writer'
   ],
-  version = '0.7.6',
+  version = '0.7.7',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.6.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.7.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

