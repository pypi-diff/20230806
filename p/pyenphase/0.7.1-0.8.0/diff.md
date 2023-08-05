# Comparing `tmp/pyenphase-0.7.1.tar.gz` & `tmp/pyenphase-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.7.1.tar", max compression
+gzip compressed data, was "pyenphase-0.8.0.tar", max compression
```

## Comparing `pyenphase-0.7.1.tar` & `pyenphase-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-08-05 19:04:46.195084 pyenphase-0.7.1/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-05 19:04:46.195084 pyenphase-0.7.1/README.md
--rw-r--r--   0        0        0     2313 2023-08-05 19:04:47.075095 pyenphase-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      823 2023-08-05 19:04:47.047094 pyenphase-0.7.1/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     7305 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/auth.py
--rw-r--r--   0        0        0      690 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/const.py
--rw-r--r--   0        0        0    10499 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1175 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1765 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     4170 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     2941 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0      833 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      825 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1388 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-08-05 19:04:46.195084 pyenphase-0.7.1/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-05 21:33:42.864390 pyenphase-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-05 21:33:42.864390 pyenphase-0.8.0/README.md
+-rw-r--r--   0        0        0     2313 2023-08-05 21:33:43.984418 pyenphase-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      876 2023-08-05 21:33:43.948417 pyenphase-0.8.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     7305 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      690 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0    10499 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1175 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1765 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     4170 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     2941 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0      833 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      825 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1388 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-08-05 21:33:42.868390 pyenphase-0.8.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.8.0/PKG-INFO
```

### Comparing `pyenphase-0.7.1/LICENSE` & `pyenphase-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/README.md` & `pyenphase-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/pyproject.toml` & `pyenphase-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.7.1"
+version = "0.8.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.7.1/src/pyenphase/__init__.py` & `pyenphase-0.8.0/src/pyenphase/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     EnvoyAuthenticationRequired,
     EnvoyCommunicationError,
     EnvoyError,
     EnvoyFirmwareCheckError,
     EnvoyFirmwareFatalCheckError,
     EnvoyProbeFailed,
 )
+from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
 from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
 
 __all__ = (
     AUTH_TOKEN_MIN_VERSION,
     "Envoy",
+    "EnvoyData",
     "EnvoyError",
     "EnvoyCommunicationError",
     "EnvoyFirmwareCheckError",
     "EnvoyFirmwareFatalCheckError",
     "EnvoyAuthenticationError",
     "EnvoyAuthenticationRequired",
     "EnvoyProbeFailed",
```

### Comparing `pyenphase-0.7.1/src/pyenphase/auth.py` & `pyenphase-0.8.0/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/const.py` & `pyenphase-0.8.0/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/envoy.py` & `pyenphase-0.8.0/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/exceptions.py` & `pyenphase-0.8.0/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/firmware.py` & `pyenphase-0.8.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/dry_contacts.py` & `pyenphase-0.8.0/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/encharge.py` & `pyenphase-0.8.0/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/enpower.py` & `pyenphase-0.8.0/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/envoy.py` & `pyenphase-0.8.0/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/inverter.py` & `pyenphase-0.8.0/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/system_consumption.py` & `pyenphase-0.8.0/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/models/system_production.py` & `pyenphase-0.8.0/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/src/pyenphase/ssl.py` & `pyenphase-0.8.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.7.1/PKG-INFO` & `pyenphase-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.7.1
+Version: 0.8.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 0.7.1 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.8.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

