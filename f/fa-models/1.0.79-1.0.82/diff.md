# Comparing `tmp/fa-models-1.0.79.tar.gz` & `tmp/fa-models-1.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.79.tar", last modified: Sun Jul 16 20:16:16 2023, max compression
+gzip compressed data, was "fa-models-1.0.82.tar", last modified: Sun Aug  6 13:17:35 2023, max compression
```

## Comparing `fa-models-1.0.79.tar` & `fa-models-1.0.82.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:16:16.906033 fa-models-1.0.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-16 20:15:38.000000 fa-models-1.0.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.902033 fa-models-1.0.79/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 20:16:16.000000 fa-models-1.0.79/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.902033 fa-models-1.0.79/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-16 20:15:38.000000 fa-models-1.0.79/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-16 20:16:06.000000 fa-models-1.0.79/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:16:16.906033 fa-models-1.0.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-16 20:15:38.000000 fa-models-1.0.79/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:16:16.906033 fa-models-1.0.79/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-16 20:15:38.000000 fa-models-1.0.79/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-16 20:15:38.000000 fa-models-1.0.79/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-06 13:17:35.568759 fa-models-1.0.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-06 13:17:03.000000 fa-models-1.0.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-06 13:17:35.000000 fa-models-1.0.82/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-06 13:17:35.000000 fa-models-1.0.82/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:17:35.000000 fa-models-1.0.82/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 13:17:35.000000 fa-models-1.0.82/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 13:17:35.000000 fa-models-1.0.82/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/famodels/models/db_independent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/db_independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/db_independent/investor_exchange_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-06 13:17:03.000000 fa-models-1.0.82/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-06 13:17:27.000000 fa-models-1.0.82/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:17:35.568759 fa-models-1.0.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-06 13:17:03.000000 fa-models-1.0.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:35.568759 fa-models-1.0.82/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-08-06 13:17:03.000000 fa-models-1.0.82/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-06 13:17:03.000000 fa-models-1.0.82/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.79/PKG-INFO` & `fa-models-1.0.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.79
+Version: 1.0.82
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.79/README.md` & `fa-models-1.0.82/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.82/fa_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.79
+Version: 1.0.82
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.79/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.82/fa_models.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,11 +15,13 @@
 famodels/models/person.py
 famodels/models/processed_signal.py
 famodels/models/side.py
 famodels/models/signal_provider.py
 famodels/models/trade.py
 famodels/models/trading_signal.py
 famodels/models/virtual_order.py
+famodels/models/db_independent/__init__.py
+famodels/models/db_independent/investor_exchange_data.py
 famodels/models/market/__init__.py
 famodels/models/market/public_trade.py
 tests/test_investor.py
 tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.79/famodels/models/algorithm.py` & `fa-models-1.0.82/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/investor.py` & `fa-models-1.0.82/famodels/models/investor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from datetime import datetime
 import os
 import time
 from typing import List, Optional
 from pydantic import EmailStr
 from redis_om import Field, JsonModel, EmbeddedJsonModel
 from redis_om.connections import get_redis_connection
 from famodels.models.person import Person
 from cryptography.fernet import Fernet
 from hashlib import sha256
 import bcrypt
 from base64 import urlsafe_b64encode
-
 from enum import Enum
 
 class StateOfInvestor(str, Enum):    
     """Describing the possible states of an Investor. Keep it simple. Also, we added the str to inherit from, so that the ENUM is serializable.         """
     REGISTERED = "registered"
     """When an investor is merely registered, but NOT authenticated with an official document. Registered allows cold trading."""
     QUALIFIED = "qualified"
@@ -98,40 +98,49 @@
     class Meta:
         model_key_prefix = "exchange-key"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 
 class Investor(JsonModel):
     id: str = Field(index=True)
-    name: str = Field(index=True, full_text_search=True)
-    """company name or givenname & family name"""
+    name: str = Field(index=True, full_text_search=True, default="")
+    """company name or full private name"""
     email: EmailStr = Field(index=True)
-    accountable: Person = Field(index=True)        
+    is_company: int = Field(index=True, default=0)
+    accountable: Optional[Person] #= Field(index=True) # cannot be optional, otherwise, we need to send full person data on creation-time.      
+    """Mandatory, if it is a company."""
     state: StateOfInvestor = Field(index=True, default=StateOfInvestor.REGISTERED.value)
+    # credential: Credential = Field(index=False)
     _passphrase: Optional[str]
     #library constraint: "redis_om.model.model.RedisModelError: In this Preview release, list and tuple fields can only contain strings. Problem field: compounding"
     funds: Optional[List[Fund]]
     exchange_keys: Optional[List[ExchangeKey]]
     priviledge_rank: int = Field(index=True, default=1, sortable=True)
     """The higher the value, the higher the priviledge."""
+    timestamp: Optional[datetime]
+    """Record, when this record was created. Needs to be determined by the business logic, not by the data logic."""    
 
     @property
     def passphrase(self):
         raise Exception("Cannot retrieve passphrase.")
     
     def setPassphrase(self, passphrase:str):
         """Use this method to set a password. The pydantic setter method does not work with JsonModel."""
-        encoded_pw = passphrase.encode()
+        if isinstance(passphrase, str):
+            passphrase = passphrase.encode()
         # Adding the salt to prefent Rainbow Table Attacks and avoiding to hash the same password with the same hash.
         # DO NOT USE A STATIC SALT!
         salt = bcrypt.gensalt()
-        self._passphrase = bcrypt.hashpw(encoded_pw, salt)
+        self._passphrase = bcrypt.hashpw(passphrase, salt)
 
     def verify_passphrase(self, passphrase: str):
-        return bcrypt.checkpw(passphrase.encode(), self._passphrase)    
+        if isinstance(passphrase, str):
+            passphrase = passphrase.encode()
+        encoded_passphrase = self._passphrase.encode() if isinstance(self._passphrase, str) else self._passphrase
+        return bcrypt.checkpw(passphrase, encoded_passphrase)    
     
     def is_qualified(self):
         return self.state == StateOfInvestor.QUALIFIED
     
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="investor"
```

### Comparing `fa-models-1.0.79/famodels/models/investor_statement.py` & `fa-models-1.0.82/famodels/models/investor_statement.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/market/public_trade.py` & `fa-models-1.0.82/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/processed_signal.py` & `fa-models-1.0.82/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/signal_provider.py` & `fa-models-1.0.82/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/trade.py` & `fa-models-1.0.82/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/trading_signal.py` & `fa-models-1.0.82/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/famodels/models/virtual_order.py` & `fa-models-1.0.82/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.79/pyproject.toml` & `fa-models-1.0.82/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.79"
+version = "1.0.82"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.79"
+current_version = "1.0.82"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.79/setup.py` & `fa-models-1.0.82/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 #                 #     if obj.__module__ == module_name:
 #                 #         print(name)
 
 #         build.run(self)
 
 setup(
     name='fa-models',
-    packages=find_packages(include=['famodels', 'famodels.models', 'famodels.models.market'], exclude=['tests*']),
+    packages=find_packages(include=['famodels', 
+                                    'famodels.models', 
+                                    'famodels.models.market',
+                                    'famodels.models.db_independent'
+                                    ], exclude=['tests*']),
     # packages=['famodels'],
     # package_dir={'famodels':'src'}
     #packages=find_packages(),
     #version='0.1.0',
     # description='The library describes the most common models used in trading systems.',
     # author='Brayan Svan',
     # license='MIT',
```

### Comparing `fa-models-1.0.79/tests/test_investor.py` & `fa-models-1.0.82/tests/test_investor.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,59 +23,59 @@
     if 'CI' not in os.environ:
         os.system('docker stop redis-unit-test')
         os.system('docker rm redis-unit-test')
 
 
 def test_investor_model():
     """Simple test if we can create a Investor model."""
-    person = Person(given_name="john", family_name="Doe", email="john@doe.com", gender="f", nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    person = Person(given_name="john", family_name="Doe", email="john@doe.com", gender="f", nationality_iso2="UK", country_of_residence_iso2="IR", phone="+43 681 11 24")
     investor = Investor(id='123', name="Jonathans Investements Ltd", email='test@example.com', accountable=person)    
 
 
 @pytest.mark.parametrize(
-    "email, nationality_iso3, country_of_residence_iso3",
+    "email, nationality_iso2, country_of_residence_iso2",
     [
-        ("invalidemail", "GBR", "IRE"),  # invalid email
-        ("john@doe.com", "GB", "IRE"),  # invalid nationality_iso3
-        ("john@doe.com", "GBR", "IR"),  # invalid country_of_residence_iso3
-        ("john@doe.com", "GBRRA", "IRE"),  # invalid nationality_iso3
-        ("john@doe.com", "GBR", "IRELA"),  # invalid country_of_residence_iso3
+        ("invalidemail", "UK", "IRE"),  # invalid email
+        ("john@doe.com", "GB", "IRE"),  # invalid nationality_iso2
+        ("john@doe.com", "UKI", "IR"),  # invalid country_of_residence_iso2
+        ("john@doe.com", "UKRA", "IRE"),  # invalid nationality_iso2
+        ("john@doe.com", "UK", "IRELA"),  # invalid country_of_residence_iso2
     ],
 )
-def test_negative_person(email, nationality_iso3, country_of_residence_iso3):
+def test_negative_person(email, nationality_iso2, country_of_residence_iso2):
     with pytest.raises(ValidationError):
         Person(
             given_name="john",
             family_name="Doe",
             email=email,
             gender="f",
-            nationality_iso3=nationality_iso3,
-            country_of_residence_iso3=country_of_residence_iso3,
+            nationality_iso2=nationality_iso2,
+            country_of_residence_iso2=country_of_residence_iso2,
             phone="+43 681 11 24",
         )
 
 @pytest.mark.parametrize(
-    "email, nationality_iso3, country_of_residence_iso3",
+    "email, nationality_iso2, country_of_residence_iso2",
     [
-        ("john.doe+test@domain.com", "GBR", "IRE"),  # valid email with plus addressing and country codes
-        ("jane-doe@sub.domain.com", "USA", "CAN"),  # valid email with hyphen and subdomain
-        ("bob_smith@edu.domain.ac.uk", "AUS", "NZL"),  # valid email with underscore and multiple domain levels
-        ("alice.johnson@long-domain-name.com", "IND", "GBR"),  # valid email with long domain name
-        ("charles-brown@domain.io", "BRA", "ARG"),  # valid email with country code top-level domain (ccTLD)
+        ("john.doe+test@domain.com", "UK", "IR"),  # valid email with plus addressing and country codes
+        ("jane-doe@sub.domain.com", "US", "CA"),  # valid email with hyphen and subdomain
+        ("bob_smith@edu.domain.ac.uk", "AU", "NZ"),  # valid email with underscore and multiple domain levels
+        ("alice.johnson@long-domain-name.com", "IN", "UK"),  # valid email with long domain name
+        ("charles-brown@domain.io", "BR", "AR"),  # valid email with country code top-level domain (ccTLD)
     ],
 )
-def test_positive_person(email, nationality_iso3, country_of_residence_iso3):
+def test_positive_person(email, nationality_iso2, country_of_residence_iso2):
     try:
         Person(
             given_name="john",
             family_name="Doe",
             email=email,
             gender="f",
-            nationality_iso3=nationality_iso3,
-            country_of_residence_iso3=country_of_residence_iso3,
+            nationality_iso2=nationality_iso2,
+            country_of_residence_iso2=country_of_residence_iso2,
             phone="+43 681 11 24",
         )
     except ValidationError:
         pytest.fail("ValidationError raised unexpectedly!")
 
 
 @pytest.mark.parametrize(
@@ -105,15 +105,15 @@
     [
         ("1", "Superion Corp.", "investor1@example.com", [{"id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"id": "s2", "algo_id": "a2"}, {"id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
         ("2", "Super Investment Ltd", "investor2@example.com", [{"id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"id": "s4", "algo_id": "a4"}, {"id": "s5", "algo_id": "a5"}, {"id": "s6", "algo_id": "a6"}], "compounding": 1}]),
         ("3", "XY Funds", "investor3@example.com", [{"id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"id": "s8", "algo_id": "a8"}, {"id": "s9", "algo_id": "a9"}, {"id": "s10", "algo_id": "a10"}]}])
     ]
 )
 def test_investor_funds(investor_id, name, email, funds):
-    person = Person(given_name="john", family_name="Doe", email=email, gender="f", nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    person = Person(given_name="john", family_name="Doe", email=email, gender="f", nationality_iso2="UK", country_of_residence_iso2="IR", phone="+43 681 11 24")
 
     funds_objects = []
     for fund in funds:
         subscriptions = [Subscription(**subscription) for subscription in fund.pop('subscriptions')]
         fund_obj = Fund(subscriptions=subscriptions, **fund)
         funds_objects.append(fund_obj)
 
@@ -128,15 +128,15 @@
         assert investor.funds[i].name == funds_objects[i].name
         assert investor.funds[i].compounding == funds_objects[i].compounding
         assert len(investor.funds[i].subscriptions) == len(funds_objects[i].subscriptions)
 
 
 def test_passphrase():
     # Create an Investor instance
-    person = Person(given_name="john", family_name="Doe", email="john@doe.com", gender="f", nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    person = Person(given_name="john", family_name="Doe", email="john@doe.com", gender="f", nationality_iso2="UK", country_of_residence_iso2="IR", phone="+43 681 11 24")
     investor = Investor(id='123', name="Johnny's Investments", email='test@example.com', accountable=person)
     investor.setPassphrase("testpass")
     # Check that passphrase can't be retrieved directly
     with pytest.raises(Exception) as e:
         print(f"INVOKING IS FORBIDDEN --> {investor.passphrase}")
     assert str(e.value) == "Cannot retrieve passphrase."
```

### Comparing `fa-models-1.0.79/tests/test_processed_trading_signal.py` & `fa-models-1.0.82/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

