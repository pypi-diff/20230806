# Comparing `tmp/pylimit-0.1.7.tar.gz` & `tmp/pylimit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylimit-0.1.7.tar", last modified: Wed Mar 29 04:27:39 2017, max compression
+gzip compressed data, was "/Users/biplap.sarkar/dev/pylimit/dist/.tmp-2_6k2s27/pylimit-1.0.0.tar", last modified: Sun Aug  6 04:54:35 2023, max compression
```

## Comparing `pylimit-0.1.7.tar` & `pylimit-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxr-xr-x   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)        0 2017-03-29 04:27:39.000000 pylimit-0.1.7/
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)      430 2017-03-29 04:27:39.000000 pylimit-0.1.7/PKG-INFO
-drwxr-xr-x   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)        0 2017-03-29 04:27:39.000000 pylimit-0.1.7/pylimit/
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)      152 2016-05-29 18:43:34.000000 pylimit-0.1.7/pylimit/__init__.py
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)     4083 2016-08-17 19:47:11.000000 pylimit-0.1.7/pylimit/pyratelimit.py
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)       48 2016-05-29 18:43:34.000000 pylimit-0.1.7/pylimit/pyratelimit_exception.py
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)     1945 2017-03-29 04:04:51.000000 pylimit-0.1.7/pylimit/redis_helper.py
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)     1491 2016-05-29 18:43:34.000000 pylimit-0.1.7/README
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)       39 2016-05-29 18:43:34.000000 pylimit-0.1.7/setup.cfg
--rw-r--r--   0 biplap.sarkar (598264411) WEPAY\Domain Users (1477001427)      482 2017-03-29 04:05:20.000000 pylimit-0.1.7/setup.py
+drwxr-xr-x   0 biplap.sarkar   (501) staff       (20)        0 2023-08-06 04:54:35.000000 pylimit-1.0.0/
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)    11366 2019-11-23 04:24:06.000000 pylimit-1.0.0/LICENSE.txt
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)      400 2023-08-06 04:54:35.000000 pylimit-1.0.0/PKG-INFO
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)     1491 2019-11-23 04:24:06.000000 pylimit-1.0.0/README
+drwxr-xr-x   0 biplap.sarkar   (501) staff       (20)        0 2023-08-06 04:54:35.000000 pylimit-1.0.0/pylimit/
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)      152 2019-11-23 04:24:06.000000 pylimit-1.0.0/pylimit/__init__.py
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)     4566 2023-08-05 19:21:40.000000 pylimit-1.0.0/pylimit/pyratelimit.py
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)       48 2019-11-23 04:24:06.000000 pylimit-1.0.0/pylimit/pyratelimit_exception.py
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)     2105 2023-08-05 19:21:40.000000 pylimit-1.0.0/pylimit/redis_helper.py
+drwxr-xr-x   0 biplap.sarkar   (501) staff       (20)        0 2023-08-06 04:54:35.000000 pylimit-1.0.0/pylimit.egg-info/
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)      400 2023-08-06 04:54:35.000000 pylimit-1.0.0/pylimit.egg-info/PKG-INFO
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)      261 2023-08-06 04:54:35.000000 pylimit-1.0.0/pylimit.egg-info/SOURCES.txt
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)        1 2023-08-06 04:54:35.000000 pylimit-1.0.0/pylimit.egg-info/dependency_links.txt
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)        8 2023-08-06 04:54:35.000000 pylimit-1.0.0/pylimit.egg-info/top_level.txt
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)       79 2023-08-06 04:54:35.000000 pylimit-1.0.0/setup.cfg
+-rw-r--r--   0 biplap.sarkar   (501) staff       (20)      482 2023-08-06 04:26:57.000000 pylimit-1.0.0/setup.py
```

### Comparing `pylimit-0.1.7/pylimit/pyratelimit.py` & `pylimit-1.0.0/pylimit/pyratelimit.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,103 +3,136 @@
 from pylimit.redis_helper import RedisHelper
 from pylimit.pyratelimit_exception import PyRateLimitException
 
 
 class PyRateLimit(object):
     redis_helper = None     # type: RedisHelper
 
-    def __init__(self):
-        self.period = None      # type: int
-        self.limit = None       # type: int
+    def __init__(self, period: int, limit: int):
+        """
+        :param period: Rate limiting period in seconds
+        :type period: int
+
+        :param limit: Number of attempts permitted by rate limiting within a
+         given period
+        :type limit: int
+        """
+        self.period = period      # type: int
+        self.limit = limit       # type: int
 
     @classmethod
-    def init(cls, redis_host: str, redis_port: int, is_sentinel_redis=False, redis_sentinel_service="mymaster",
+    def init(cls, redis_host: str, redis_port: int, is_sentinel_redis=False,
+             redis_sentinel_service="mymaster",
              redis_password=None):
         """
         Initializes redis connection
+
         :param redis_host: Hostname of redis server
         :type redis_host: str
 
         :param redis_port: Port at which redis server is listening
         :type redis_port:int
 
-        :param is_sentinel_redis: Parameter indicating if redis server is a sentinel server. Default is false
+        :param is_sentinel_redis: Parameter indicating if redis server is a
+        sentinel server. Default is false
         :type is_sentinel_redis: bool
 
-        :param redis_sentinel_service: If redis server is a sentinel server, service name for redis sentinel
+        :param redis_sentinel_service: If redis server is a sentinel server,
+         service name for redis sentinel
         :type redis_sentinel_service: str
 
         :param redis_password: Password for redis connection
         :type redis_password: str
 
         """
         if not cls.redis_helper:
-            cls.redis_helper = RedisHelper(host=redis_host, port=redis_port, is_sentinel=is_sentinel_redis,
-                                           sentinel_service=redis_sentinel_service, password=redis_password)
+            cls.redis_helper = RedisHelper(
+                host=redis_host, port=redis_port,
+                is_sentinel=is_sentinel_redis,
+                sentinel_service=redis_sentinel_service,
+                password=redis_password)
 
-    def create(self, period: int, limit: int):
+    def __can_attempt(self, namespace: str, add_attempt=True,
+                      timestamp=None) -> bool:
         """
-        Creates a rate limiting rule with rate limiting period and attempt limit
-
-        :param period: Rate limiting period in seconds
-        :type period: int
-
-        :param limit: Number of attempts permitted by rate limiting within a given period
-        :type limit: int
-
-        """
-        self.period = period
-        self.limit = limit
-
-    def __can_attempt(self, namespace: str, add_attempt=True) -> bool:
-        """
-        Checks if a namespace is rate limited or not with including/excluding the current call
+        Checks if a namespace is rate limited or not with including/excluding
+         the current call
 
         :param namespace: Rate limiting namespace
         :type namespace: str
 
-        :param add_attempt: Boolean value indicating if the current call should be considered as an attempt or not
+        :param add_attempt: Boolean value indicating if the current call
+        should be considered as an attempt or not
         :type add_attempt: bool
 
-        :return: Returns true if attempt can go ahead under current rate limiting rules, false otherwise
+        :param timestamp: Fix timestamp when we want to check the same flow
+        many times and avoid to sum for these cases
+        :type timestamp: int
+
+        :return: Returns true if attempt can go ahead under current rate
+        limiting rules, false otherwise
         """
         can_attempt = False
+
         if not PyRateLimit.redis_helper:
-            raise PyRateLimitException("redis connection information not provided")
+            raise PyRateLimitException("Redis Connection information not provided")
+
         connection = PyRateLimit.redis_helper.get_atomic_connection()
+
         current_time = int(round(time.time() * 1000000))
         old_time_limit = current_time - (self.period * 1000000)
+
+        if timestamp:
+            current_time = timestamp
+
         connection.zremrangebyscore(namespace, 0, old_time_limit)
+
         connection.expire(namespace, self.period)
+
         if add_attempt:
             current_count = 0
-            connection.zadd(namespace, current_time, current_time)
+            mapping = {
+                current_time: current_time
+            }
+            connection.zadd(namespace, mapping)
         else:
             current_count = 1   # initialize at 1 to compensate the case that this attempt is not getting counted
+
         connection.zcard(namespace)
         redis_result = connection.execute()
+
         current_count += redis_result[-1]
+
         if current_count <= self.limit:
             can_attempt = True
+
         return can_attempt
 
-    def attempt(self, namespace: str):
+    def attempt(self, namespace: str, timestamp=None):
         """
-        Records an attempt and returns true of false depending on whether attempt can go through or not
+        Records an attempt and returns true of false depending on whether
+        attempt can go through or not
 
         :param namespace: Rate limiting namespace
         :type namespace: str
 
-        :return: Returns true if attempt can go ahead under current rate limiting rules, false otherwise
+        :param timestamp: Fix timestamp when we want to check the same flow
+        many times and avoid to sum for these cases
+        :type timestamp: int
+
+        :return: Returns true if attempt can go ahead under current rate
+        limiting rules, false otherwise
         """
-        return self.__can_attempt(namespace=namespace)
+        return self.__can_attempt(namespace=namespace, timestamp=timestamp)
 
     def is_rate_limited(self, namespace: str) -> bool:
         """
-        Checks if a namespace is already rate limited or not without making any additional attempts
+        Checks if a namespace is already rate limited or not without making
+        any additional attempts
 
         :param namespace:  Rate limiting namespace
         :type namespace: str
 
-        :return:    Returns true if attempt can go ahead under current rate limiting rules, false otherwise
+        :return:    Returns true if attempt can go ahead under current rate
+        limiting rules, false otherwise
         """
         return not self.__can_attempt(namespace=namespace, add_attempt=False)
```

### Comparing `pylimit-0.1.7/pylimit/redis_helper.py` & `pylimit-1.0.0/pylimit/redis_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 import redis
 from redis.sentinel import Sentinel
-from redis.client import StrictPipeline
+from redis.client import Pipeline
 import redis.client
 
 
 class RedisHelper(object):
-    def __init__(self, host: str, port: int, is_sentinel=False, sentinel_service=None, password=None):
+    def __init__(self, host: str, port: int, is_sentinel=False,
+                 sentinel_service=None, password=None):
         self.host = host
         self.port = port
         self.is_sentinel = is_sentinel
         self.sentinel_service = sentinel_service
         self.password = password
 
         self.connection = None
         self.get_connection()  # Ensure connection is established
 
     def get_connection(self, is_read_only=False) -> redis.StrictRedis:
         """
-        Gets a StrictRedis connection for normal redis or for redis sentinel based upon redis mode in configuration.
+        Gets a StrictRedis connection for normal redis or for redis sentinel
+         based upon redis mode in configuration.
 
         :type is_read_only: bool
-        :param is_read_only: In case of redis sentinel, it returns connection to slave
+        :param is_read_only: In case of redis sentinel, it returns connection
+         to slave
 
         :return: Returns a StrictRedis connection
         """
         if self.connection is not None:
             return self.connection
 
         if self.is_sentinel:
             kwargs = dict()
             if self.password:
                 kwargs["password"] = self.password
             sentinel = Sentinel([(self.host, self.port)], **kwargs)
             if is_read_only:
-                connection = sentinel.slave_for(self.sentinel_service, decode_responses=True)
+                connection = sentinel.slave_for(self.sentinel_service,
+                                                decode_responses=True)
             else:
-                connection = sentinel.master_for(self.sentinel_service, decode_responses=True)
+                connection = sentinel.master_for(self.sentinel_service,
+                                                 decode_responses=True)
         else:
-            connection = redis.StrictRedis(host=self.host, port=self.port, decode_responses=True,
+            connection = redis.StrictRedis(host=self.host, port=self.port,
+                                           decode_responses=True,
                                            password=self.password)
         self.connection = connection
         return connection
 
-    def get_atomic_connection(self) -> StrictPipeline:
+    def get_atomic_connection(self) -> Pipeline:
         """
-        Gets a StrictPipeline for normal redis or for redis sentinel based upon redis mode in configuration
+        Gets a Pipeline for normal redis or for redis sentinel based upon
+         redis mode in configuration
 
-        :return: Returns a StrictPipeline object
+        :return: Returns a Pipeline object
         """
         return self.get_connection().pipeline(True)
```

### Comparing `pylimit-0.1.7/README` & `pylimit-1.0.0/README`

 * *Files identical despite different names*

