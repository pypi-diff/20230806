# Comparing `tmp/betabageldb-0.2.0.tar.gz` & `tmp/betabageldb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.2.0.tar", last modified: Wed Jul 26 14:56:55 2023, max compression
+gzip compressed data, was "betabageldb-0.2.1.tar", last modified: Sun Aug  6 15:36:00 2023, max compression
```

## Comparing `betabageldb-0.2.0.tar` & `betabageldb-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.370983 betabageldb-0.2.0/
--rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-07-26 14:56:55.370774 betabageldb-0.2.0/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     2643 2023-07-26 14:55:22.000000 betabageldb-0.2.0/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.362925 betabageldb-0.2.0/bagel/
--rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.365964 betabageldb-0.2.0/bagel/api/
--rw-r--r--   0 bidhan     (501) staff       (20)    13827 2023-07-24 20:40:18.000000 betabageldb-0.2.0/bagel/api/Cluster.py
--rw-r--r--   0 bidhan     (501) staff       (20)    10468 2023-07-26 14:53:36.000000 betabageldb-0.2.0/bagel/api/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11927 2023-07-26 14:55:22.000000 betabageldb-0.2.0/bagel/api/fastapi.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/api/types.py
--rw-r--r--   0 bidhan     (501) staff       (20)     5926 2023-07-24 20:40:18.000000 betabageldb-0.2.0/bagel/config.py
--rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/errors.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.366474 betabageldb-0.2.0/bagel/utils/
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/utils/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.370018 betabageldb-0.2.0/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      349 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-26 14:56:55.371019 betabageldb-0.2.0/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)     1641 2023-07-26 14:56:10.000000 betabageldb-0.2.0/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 15:36:00.555711 betabageldb-0.2.1/
+-rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-08-06 15:36:00.555330 betabageldb-0.2.1/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     2643 2023-07-26 14:55:22.000000 betabageldb-0.2.1/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 15:36:00.545099 betabageldb-0.2.1/bagel/
+-rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.2.1/bagel/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 15:36:00.551610 betabageldb-0.2.1/bagel/api/
+-rw-r--r--   0 bidhan     (501) staff       (20)    13827 2023-07-24 20:40:18.000000 betabageldb-0.2.1/bagel/api/Cluster.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    10713 2023-08-01 18:29:23.000000 betabageldb-0.2.1/bagel/api/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    12194 2023-08-01 18:29:23.000000 betabageldb-0.2.1/bagel/api/fastapi.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.2.1/bagel/api/types.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     5926 2023-08-01 18:29:40.000000 betabageldb-0.2.1/bagel/config.py
+-rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.2.1/bagel/errors.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 15:36:00.552481 betabageldb-0.2.1/bagel/utils/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.2.1/bagel/utils/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 15:36:00.554777 betabageldb-0.2.1/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-08-06 15:36:00.000000 betabageldb-0.2.1/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      349 2023-08-06 15:36:00.000000 betabageldb-0.2.1/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-08-06 15:36:00.000000 betabageldb-0.2.1/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-08-06 15:36:00.000000 betabageldb-0.2.1/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-08-06 15:36:00.000000 betabageldb-0.2.1/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-08-06 15:36:00.555750 betabageldb-0.2.1/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1641 2023-08-06 15:33:49.000000 betabageldb-0.2.1/setup.py
```

### Comparing `betabageldb-0.2.0/PKG-INFO` & `betabageldb-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.2.0
+Version: 0.2.1
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betabageldb-0.2.0/README.md` & `betabageldb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.0/bagel/__init__.py` & `betabageldb-0.2.1/bagel/__init__.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.0/bagel/api/Cluster.py` & `betabageldb-0.2.1/bagel/api/Cluster.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.0/bagel/api/__init__.py` & `betabageldb-0.2.1/bagel/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Sequence, Optional
+from typing import Sequence, Optional, Dict
 import pandas as pd
 from uuid import UUID
 from bagel.api.Cluster import Cluster
 from bagel.api.types import (
     ClusterMetadata,
     Document,
     Documents,
@@ -46,14 +46,26 @@
         Returns:
             dict: A dictionary of clusters
 
         """
         pass
 
     @abstractmethod
+    def join_waitlist(self, email: str) -> Dict[str, str]:
+        """
+        Add email to waitlist
+        Args:
+            None
+
+        Returns:
+            dict: A dictionary of resposne
+        """
+        pass
+
+    @abstractmethod
     def create_cluster(
         self,
         name: str,
         metadata: Optional[ClusterMetadata] = None,
         get_or_create: bool = False,
     ) -> Cluster:
         """Creates a new cluster in the database
```

### Comparing `betabageldb-0.2.0/bagel/api/fastapi.py` & `betabageldb-0.2.1/bagel/api/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     QueryResult,
     ClusterMetadata,
     OneOrMany,
 )
 import pandas as pd
 import requests
 import json
-from typing import Sequence
+from typing import Sequence, Dict
 from bagel.api.Cluster import Cluster
 import bagel.errors as errors
 from uuid import UUID
 from overrides import override
 
 
 class FastAPI(API):
@@ -39,14 +39,21 @@
     def ping(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive"""
         resp = requests.get(self._api_url)
         raise_bagel_error(resp)
         return int(resp.json()["nanosecond heartbeat"])
 
     @override
+    def join_waitlist(self, email: str) -> Dict[str, str]:
+        """Add email to waitlist"""
+        url = self._api_url.replace("/api/v1", "")
+        resp = requests.get(url + "/join_waitlist/" + email, timeout=60)
+        return resp.json()
+
+    @override
     def get_all_clusters(self) -> Sequence[Cluster]:
         """Returns a list of all clusters"""
         resp = requests.get(self._api_url + "/clusters")
         raise_bagel_error(resp)
         json_clusters = resp.json()
         clusters = []
         for json_cluster in json_clusters:
```

### Comparing `betabageldb-0.2.0/bagel/api/types.py` & `betabageldb-0.2.1/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.0/bagel/config.py` & `betabageldb-0.2.1/bagel/config.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.0/bagel/errors.py` & `betabageldb-0.2.1/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.0/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.2.1/betabageldb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.2.0
+Version: 0.2.1
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betabageldb-0.2.0/betabageldb.egg-info/requires.txt` & `betabageldb-0.2.1/betabageldb.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 idna==3.4
 monotonic==1.6
 mpmath==1.3.0
 numpy==1.24.4
 onnxruntime==1.15.1
 overrides==7.3.1
 packaging==23.1
-pandas==1.3.5
+pandas==2.0.1
 posthog==3.0.1
 protobuf==4.23.4
 pydantic==1.10.10
 pydantic-core==2.1.2
 pyreadline3==3.4.1
 python-dateutil==2.8.2
 pytz==2023.3
```

### Comparing `betabageldb-0.2.0/setup.py` & `betabageldb-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betabageldb",
-    version="0.2.0",
+    version="0.2.1",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
     packages=find_packages(),
@@ -23,15 +23,15 @@
         "idna==3.4",
         "monotonic==1.6",
         "mpmath==1.3.0",
         "numpy==1.24.4",
         "onnxruntime==1.15.1",
         "overrides==7.3.1",
         "packaging==23.1",
-        "pandas==1.3.5",
+        "pandas==2.0.1",
         "posthog==3.0.1",
         "protobuf==4.23.4",
         "pydantic==1.10.10",
         "pydantic-core==2.1.2",
         "pyreadline3==3.4.1",
         "python-dateutil==2.8.2",
         "pytz==2023.3",
```

