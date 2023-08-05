# Comparing `tmp/pypayment-1.7.0.tar.gz` & `tmp/pypayment-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypayment-1.7.0.tar", last modified: Sat Aug  5 16:58:15 2023, max compression
+gzip compressed data, was "pypayment-1.7.1.tar", last modified: Sat Aug  5 22:45:32 2023, max compression
```

## Comparing `pypayment-1.7.0.tar` & `pypayment-1.7.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-05 16:58:15.527868 pypayment-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-05 16:58:05.000000 pypayment-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.523868 pypayment-1.7.0/pypayment/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/pypayment/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/enums/commission.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/enums/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/payment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/pypayment/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/betatransfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/lava.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/payok.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/qiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/yoomoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/pypayment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 16:58:05.000000 pypayment-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 16:58:15.527868 pypayment-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-05 16:58:05.000000 pypayment-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_lava.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_payok.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_qiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_yoomoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:32.836496 pypayment-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-05 22:45:32.836496 pypayment-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-05 22:45:17.000000 pypayment-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:32.828496 pypayment-1.7.1/pypayment/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:32.832496 pypayment-1.7.1/pypayment/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/enums/commission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/enums/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:32.832496 pypayment-1.7.1/pypayment/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/providers/betatransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/providers/lava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/providers/payok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/providers/qiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-05 22:45:17.000000 pypayment-1.7.1/pypayment/providers/yoomoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:32.832496 pypayment-1.7.1/pypayment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-05 22:45:32.000000 pypayment-1.7.1/pypayment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-05 22:45:32.000000 pypayment-1.7.1/pypayment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 22:45:32.000000 pypayment-1.7.1/pypayment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 22:45:32.000000 pypayment-1.7.1/pypayment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 22:45:32.000000 pypayment-1.7.1/pypayment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 22:45:17.000000 pypayment-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 22:45:32.836496 pypayment-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-05 22:45:17.000000 pypayment-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:45:32.836496 pypayment-1.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/test_lava.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/test_payok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/test_qiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-05 22:45:17.000000 pypayment-1.7.1/test/test_yoomoney.py
```

### Comparing `pypayment-1.7.0/PKG-INFO` & `pypayment-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypayment
-Version: 1.7.0
+Version: 1.7.1
 Summary: Payment providers API wrapper
 Home-page: https://github.com/TimNekk/pypayment
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypayment Version: 1.7.0 Summary: Payment providers
+Metadata-Version: 2.1 Name: pypayment Version: 1.7.1 Summary: Payment providers
 API wrapper Home-page: https://github.com/TimNekk/pypayment Author: TimNekk
 Author-email: herew26@gmail.com License: Apache License, Version 2.0, see
 LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pypayment-1.7.0/README.md` & `pypayment-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/__init__.py` & `pypayment-1.7.1/pypayment/__init__.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/exceptions.py` & `pypayment-1.7.1/pypayment/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/payment.py` & `pypayment-1.7.1/pypayment/payment.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/providers/betatransfer.py` & `pypayment-1.7.1/pypayment/providers/betatransfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional, Tuple, Mapping, Any
 
 import requests
 
 from pypayment import Payment, PaymentStatus, AuthorizationError, PaymentCreationError, PaymentGettingError, \
-    PaymentNotFound
+    PaymentNotFound, ChargeCommission
 
 
 class BetaTransferCurrency(Enum):
     """BetaTransfer payment currency enum."""
 
     RUB = "RUB"
     """Russian ruble."""
@@ -151,14 +151,15 @@
     _public_key: Optional[str] = None
     _private_key: Optional[str] = None
     _payment_type: Optional[BetaTransferPaymentType] = None
     _url_result: Optional[str] = None
     _url_success: Optional[str] = None
     _url_fail: Optional[str] = None
     _locale: Optional[BetaTransferLocale] = None
+    _charge_commission: Optional[ChargeCommission] = None
     _BASE_URL = "https://merchant.betatransfer.io/api"
     _PAYMENT_URL = _BASE_URL + "/payment"
     _INFO_URL = _BASE_URL + "/info"
     _ACCOUNT_INFO_URL = _BASE_URL + "/account-info"
     _STATUS_MAP = {
         "success": PaymentStatus.PAID,
         "cancel": PaymentStatus.REJECTED,
@@ -180,15 +181,16 @@
                  amount: float,
                  description: str = "",
                  id: Optional[str] = None,
                  payment_type: Optional[BetaTransferPaymentType] = None,
                  url_result: Optional[str] = None,
                  url_success: Optional[str] = None,
                  url_fail: Optional[str] = None,
-                 locale: Optional[BetaTransferLocale] = None) -> None:
+                 locale: Optional[BetaTransferLocale] = None,
+                 charge_commission: Optional[ChargeCommission] = None) -> None:
         """
         You need to BetaTransferPayment.authorize() first!
 
         Instantiation generates new BetaTransfer invoice instance right away.
 
         Passed parameters will be applied to instance, but won't override default ones.
 
@@ -196,23 +198,26 @@
         :param description: Payment comment.
         :param id: (default: generated with uuid4).
         :param payment_type: BetaTransferPaymentType enum.
         :param url_result: Callback URL.
         :param url_success: User will be redirected to this url after paying successfully.
         :param url_fail: User will be redirected to this url after paying unsuccessfully.
         :param locale: BetaTransferLocale enum.
+        :param charge_commission: ChargeCommission enum.
 
         :raises NotAuthorizedError: When class was not authorized with BetaTransferPayment.authorize()
         :raises PaymentCreationError: When payment creation failed.
         """
         self._payment_type = BetaTransferPayment._payment_type if payment_type is None else payment_type
         self._url_result = BetaTransferPayment._url_result if url_result is None else url_result
         self._url_success = BetaTransferPayment._url_success if url_success is None else url_success
         self._url_fail = BetaTransferPayment._url_fail if url_fail is None else url_fail
         self._locale = BetaTransferPayment._locale if locale is None else locale
+        self._charge_commission = BetaTransferPayment._charge_commission if charge_commission is None \
+            else charge_commission
 
         super().__init__(amount, description, id)
 
     def _validate_params(self):
         if not self._url_success or not self._url_fail:
             raise PaymentCreationError("You must specify url_success and url_fail!")
 
@@ -232,51 +237,54 @@
     def authorize(cls,
                   public_key: str,
                   private_key: str,
                   payment_type: BetaTransferPaymentType = BetaTransferPaymentType.RUB_CARD,
                   url_result: Optional[str] = None,
                   url_success: Optional[str] = None,
                   url_fail: Optional[str] = None,
-                  locale: BetaTransferLocale = BetaTransferLocale.RUSSIAN) -> None:
+                  locale: BetaTransferLocale = BetaTransferLocale.RUSSIAN,
+                  charge_commission: ChargeCommission = ChargeCommission.FROM_SELLER) -> None:
         """
         Must be called before the first use of the class!
 
         Tries to authorize to BetaTransfer API.
         Saves passed parameters as default.
 
         :param public_key: Public API key.
         :param private_key: Private (secret) API key.
         :param payment_type: BetaTransferPaymentType enum.
         :param url_result: Callback URL.
         :param url_success: User will be redirected to this url after paying successfully.
         :param url_fail: User will be redirected to this url after paying unsuccessfully.
         :param locale: BetaTransferLocale enum.
+        :param charge_commission: ChargeCommission enum.
 
         :raises AuthorizationError: When authorization fails.
         """
         BetaTransferPayment._public_key = public_key
         BetaTransferPayment._private_key = private_key
         BetaTransferPayment._payment_type = payment_type
         BetaTransferPayment._url_result = url_result
         BetaTransferPayment._url_success = url_success
         BetaTransferPayment._url_fail = url_fail
         BetaTransferPayment._locale = locale
+        BetaTransferPayment._charge_commission = charge_commission
 
         cls._try_authorize()
 
     def _create_url(self) -> str:
         if not self._payment_type or not self._locale:
             raise PaymentCreationError("You must specify payment_type and locale!")
 
         params = {
             "token": BetaTransferPayment._public_key
         }
 
         data = {
-            "amount": self.amount,
+            "amount": self._sum_with_commission,
             "currency": self._payment_type.value.currency.value,
             "orderId": self.id,
             "paymentSystem": self._payment_type.value.name,
             "urlResult": self._url_result,
             "urlSuccess": self._url_success,
             "urlFail": self._url_fail,
             "locale": self._locale.value,
@@ -348,7 +356,14 @@
 
         BetaTransferPayment.authorized = True
 
     @classmethod
     def _get_sign(cls, data: Mapping[str, str]) -> str:
         sign = "".join(str(value) for value in data.values()) + str(BetaTransferPayment._private_key)
         return hashlib.md5(sign.encode()).hexdigest()
+
+    @property
+    def _sum_with_commission(self) -> float:
+        if self._charge_commission == ChargeCommission.FROM_CUSTOMER and self._payment_type:
+            return self.amount + self.amount * self._payment_type.value.commission_in_percent / 100
+
+        return self.amount
```

### Comparing `pypayment-1.7.0/pypayment/providers/lava.py` & `pypayment-1.7.1/pypayment/providers/lava.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/providers/payok.py` & `pypayment-1.7.1/pypayment/providers/payok.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/providers/qiwi.py` & `pypayment-1.7.1/pypayment/providers/qiwi.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment/providers/yoomoney.py` & `pypayment-1.7.1/pypayment/providers/yoomoney.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/pypayment.egg-info/PKG-INFO` & `pypayment-1.7.1/pypayment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypayment
-Version: 1.7.0
+Version: 1.7.1
 Summary: Payment providers API wrapper
 Home-page: https://github.com/TimNekk/pypayment
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypayment Version: 1.7.0 Summary: Payment providers
+Metadata-Version: 2.1 Name: pypayment Version: 1.7.1 Summary: Payment providers
 API wrapper Home-page: https://github.com/TimNekk/pypayment Author: TimNekk
 Author-email: herew26@gmail.com License: Apache License, Version 2.0, see
 LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pypayment-1.7.0/pypayment.egg-info/SOURCES.txt` & `pypayment-1.7.1/pypayment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/setup.py` & `pypayment-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/test/test_lava.py` & `pypayment-1.7.1/test/test_lava.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/test/test_payok.py` & `pypayment-1.7.1/test/test_payok.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/test/test_qiwi.py` & `pypayment-1.7.1/test/test_qiwi.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.7.0/test/test_yoomoney.py` & `pypayment-1.7.1/test/test_yoomoney.py`

 * *Files identical despite different names*

