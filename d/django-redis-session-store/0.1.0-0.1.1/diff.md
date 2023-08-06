# Comparing `tmp/django-redis-session-store-0.1.0.tar.gz` & `tmp/django-redis-session-store-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-redis-session-store-0.1.0.tar", last modified: Sun Aug  6 13:03:52 2023, max compression
+gzip compressed data, was "django-redis-session-store-0.1.1.tar", last modified: Sun Aug  6 13:08:10 2023, max compression
```

## Comparing `django-redis-session-store-0.1.0.tar` & `django-redis-session-store-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 omer       (502) staff       (20)        0 2023-08-06 13:03:52.190678 django-redis-session-store-0.1.0/
--rw-r--r--   0 omer       (502) staff       (20)     1062 2023-08-05 16:53:27.000000 django-redis-session-store-0.1.0/LICENSE
--rw-r--r--   0 omer       (502) staff       (20)     3826 2023-08-06 13:03:52.190560 django-redis-session-store-0.1.0/PKG-INFO
--rw-r--r--   0 omer       (502) staff       (20)     1757 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.0/README.md
-drwxr-xr-x   0 omer       (502) staff       (20)        0 2023-08-06 13:03:52.189822 django-redis-session-store-0.1.0/django_redis_session_store/
--rw-r--r--   0 omer       (502) staff       (20)        0 2023-08-05 16:53:27.000000 django-redis-session-store-0.1.0/django_redis_session_store/__init__.py
--rw-r--r--   0 omer       (502) staff       (20)      866 2023-08-05 16:53:27.000000 django-redis-session-store-0.1.0/django_redis_session_store/redis_server.py
--rw-r--r--   0 omer       (502) staff       (20)     5101 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.0/django_redis_session_store/session_store.py
--rw-r--r--   0 omer       (502) staff       (20)     1748 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.0/django_redis_session_store/tests.py
-drwxr-xr-x   0 omer       (502) staff       (20)        0 2023-08-06 13:03:52.190392 django-redis-session-store-0.1.0/django_redis_session_store.egg-info/
--rw-r--r--   0 omer       (502) staff       (20)     3826 2023-08-06 13:03:52.000000 django-redis-session-store-0.1.0/django_redis_session_store.egg-info/PKG-INFO
--rw-r--r--   0 omer       (502) staff       (20)      394 2023-08-06 13:03:52.000000 django-redis-session-store-0.1.0/django_redis_session_store.egg-info/SOURCES.txt
--rw-r--r--   0 omer       (502) staff       (20)        1 2023-08-06 13:03:52.000000 django-redis-session-store-0.1.0/django_redis_session_store.egg-info/dependency_links.txt
--rw-r--r--   0 omer       (502) staff       (20)       27 2023-08-06 13:03:52.000000 django-redis-session-store-0.1.0/django_redis_session_store.egg-info/top_level.txt
--rw-r--r--   0 omer       (502) staff       (20)      877 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.0/pyproject.toml
--rw-r--r--   0 omer       (502) staff       (20)       38 2023-08-06 13:03:52.190713 django-redis-session-store-0.1.0/setup.cfg
+drwxr-xr-x   0 omer       (502) staff       (20)        0 2023-08-06 13:08:10.688747 django-redis-session-store-0.1.1/
+-rw-r--r--   0 omer       (502) staff       (20)     1062 2023-08-05 16:53:27.000000 django-redis-session-store-0.1.1/LICENSE
+-rw-r--r--   0 omer       (502) staff       (20)     3877 2023-08-06 13:08:10.688541 django-redis-session-store-0.1.1/PKG-INFO
+-rw-r--r--   0 omer       (502) staff       (20)     1757 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.1/README.md
+drwxr-xr-x   0 omer       (502) staff       (20)        0 2023-08-06 13:08:10.687600 django-redis-session-store-0.1.1/django_redis_session_store/
+-rw-r--r--   0 omer       (502) staff       (20)        0 2023-08-05 16:53:27.000000 django-redis-session-store-0.1.1/django_redis_session_store/__init__.py
+-rw-r--r--   0 omer       (502) staff       (20)      866 2023-08-05 16:53:27.000000 django-redis-session-store-0.1.1/django_redis_session_store/redis_server.py
+-rw-r--r--   0 omer       (502) staff       (20)     5101 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.1/django_redis_session_store/session_store.py
+-rw-r--r--   0 omer       (502) staff       (20)     1748 2023-08-06 13:01:14.000000 django-redis-session-store-0.1.1/django_redis_session_store/tests.py
+drwxr-xr-x   0 omer       (502) staff       (20)        0 2023-08-06 13:08:10.688332 django-redis-session-store-0.1.1/django_redis_session_store.egg-info/
+-rw-r--r--   0 omer       (502) staff       (20)     3877 2023-08-06 13:08:10.000000 django-redis-session-store-0.1.1/django_redis_session_store.egg-info/PKG-INFO
+-rw-r--r--   0 omer       (502) staff       (20)      394 2023-08-06 13:08:10.000000 django-redis-session-store-0.1.1/django_redis_session_store.egg-info/SOURCES.txt
+-rw-r--r--   0 omer       (502) staff       (20)        1 2023-08-06 13:08:10.000000 django-redis-session-store-0.1.1/django_redis_session_store.egg-info/dependency_links.txt
+-rw-r--r--   0 omer       (502) staff       (20)       27 2023-08-06 13:08:10.000000 django-redis-session-store-0.1.1/django_redis_session_store.egg-info/top_level.txt
+-rw-r--r--   0 omer       (502) staff       (20)      928 2023-08-06 13:07:57.000000 django-redis-session-store-0.1.1/pyproject.toml
+-rw-r--r--   0 omer       (502) staff       (20)       38 2023-08-06 13:08:10.688798 django-redis-session-store-0.1.1/setup.cfg
```

### Comparing `django-redis-session-store-0.1.0/LICENSE` & `django-redis-session-store-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-redis-session-store-0.1.0/PKG-INFO` & `django-redis-session-store-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-redis-session-store
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Django session backend with Redis storage.
 Author-email: Ömer Alkın <omeralkin7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ömer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,16 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Home, https://github.com/mrlkn/django-redis-session
-Project-URL: Documentation, https://github.com/mrlkn/django-redis-session/README.md
-Project-URL: Source, https://github.com/mrlkn/django-redis-session
+Project-URL: Documentation, https://github.com/mrlkn/django-redis-session/blob/master/README.md
+Project-URL: Source, https://github.com/mrlkn/django-redis-session/tree/master/django_redis_session_store
 Keywords: django,session,redis,store
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `django-redis-session-store-0.1.0/README.md` & `django-redis-session-store-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-redis-session-store-0.1.0/django_redis_session_store/redis_server.py` & `django-redis-session-store-0.1.1/django_redis_session_store/redis_server.py`

 * *Files identical despite different names*

### Comparing `django-redis-session-store-0.1.0/django_redis_session_store/session_store.py` & `django-redis-session-store-0.1.1/django_redis_session_store/session_store.py`

 * *Files identical despite different names*

### Comparing `django-redis-session-store-0.1.0/django_redis_session_store/tests.py` & `django-redis-session-store-0.1.1/django_redis_session_store/tests.py`

 * *Files identical despite different names*

### Comparing `django-redis-session-store-0.1.0/django_redis_session_store.egg-info/PKG-INFO` & `django-redis-session-store-0.1.1/django_redis_session_store.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-redis-session-store
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Django session backend with Redis storage.
 Author-email: Ömer Alkın <omeralkin7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ömer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,16 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Home, https://github.com/mrlkn/django-redis-session
-Project-URL: Documentation, https://github.com/mrlkn/django-redis-session/README.md
-Project-URL: Source, https://github.com/mrlkn/django-redis-session
+Project-URL: Documentation, https://github.com/mrlkn/django-redis-session/blob/master/README.md
+Project-URL: Source, https://github.com/mrlkn/django-redis-session/tree/master/django_redis_session_store
 Keywords: django,session,redis,store
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `django-redis-session-store-0.1.0/pyproject.toml` & `django-redis-session-store-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "django-redis-session-store"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Django session backend with Redis storage."
 readme = "README.md"
 authors = [
     {name = "Ömer Alkın", email = "omeralkin7@gmail.com"},
 ]
 license = { file = "LICENSE" }
 keywords = ["django", "session", "redis", "store"]
@@ -19,9 +19,9 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [project.urls]
 Home = "https://github.com/mrlkn/django-redis-session"
-Documentation = "https://github.com/mrlkn/django-redis-session/README.md"
-Source = "https://github.com/mrlkn/django-redis-session"
+Documentation = "https://github.com/mrlkn/django-redis-session/blob/master/README.md"
+Source = "https://github.com/mrlkn/django-redis-session/tree/master/django_redis_session_store"
```

