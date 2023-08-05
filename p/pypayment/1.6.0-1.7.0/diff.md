# Comparing `tmp/pypayment-1.6.0.tar.gz` & `tmp/pypayment-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypayment-1.6.0.tar", last modified: Wed Jul 19 18:57:32 2023, max compression
+gzip compressed data, was "pypayment-1.7.0.tar", last modified: Sat Aug  5 16:58:15 2023, max compression
```

## Comparing `pypayment-1.6.0.tar` & `pypayment-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:32.800362 pypayment-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-19 18:57:32.800362 pypayment-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-19 18:57:20.000000 pypayment-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:32.800362 pypayment-1.6.0/pypayment/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:32.800362 pypayment-1.6.0/pypayment/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/enums/commission.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/enums/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/payment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:32.800362 pypayment-1.6.0/pypayment/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/providers/lava.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/providers/payok.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/providers/qiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-19 18:57:20.000000 pypayment-1.6.0/pypayment/providers/yoomoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:32.800362 pypayment-1.6.0/pypayment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-19 18:57:32.000000 pypayment-1.6.0/pypayment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-19 18:57:32.000000 pypayment-1.6.0/pypayment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 18:57:32.000000 pypayment-1.6.0/pypayment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 18:57:32.000000 pypayment-1.6.0/pypayment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 18:57:32.000000 pypayment-1.6.0/pypayment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 18:57:20.000000 pypayment-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 18:57:32.800362 pypayment-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-19 18:57:20.000000 pypayment-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:57:32.800362 pypayment-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/test_lava.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/test_payok.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/test_qiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-19 18:57:20.000000 pypayment-1.6.0/test/test_yoomoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-05 16:58:15.527868 pypayment-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-08-05 16:58:05.000000 pypayment-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.523868 pypayment-1.7.0/pypayment/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/pypayment/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/enums/commission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/enums/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/pypayment/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/betatransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/lava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/payok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/qiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-08-05 16:58:05.000000 pypayment-1.7.0/pypayment/providers/yoomoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/pypayment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 16:58:15.000000 pypayment-1.7.0/pypayment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-05 16:58:05.000000 pypayment-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 16:58:15.527868 pypayment-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-05 16:58:05.000000 pypayment-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:58:15.527868 pypayment-1.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_lava.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_payok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_qiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-05 16:58:05.000000 pypayment-1.7.0/test/test_yoomoney.py
```

### Comparing `pypayment-1.6.0/PKG-INFO` & `pypayment-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypayment
-Version: 1.6.0
+Version: 1.7.0
 Summary: Payment providers API wrapper
 Home-page: https://github.com/TimNekk/pypayment
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -56,14 +56,15 @@
 
 For more details see [documentation](https://pypayment.readthedocs.io).
 
 ## Providers:
 - [Qiwi P2P](https://p2p.qiwi.com/)
 - [YooMoney](https://yoomoney.ru/)
 - [PayOk](https://payok.io/)
+- [BetaTransfer](https://betatransfer.io/)
 - [Lava](https://lava.kz/) *(under development)*
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/pypayment/)
 
 ```bash
 pip install -U pypayment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypayment Version: 1.6.0 Summary: Payment providers
+Metadata-Version: 2.1 Name: pypayment Version: 1.7.0 Summary: Payment providers
 API wrapper Home-page: https://github.com/TimNekk/pypayment Author: TimNekk
 Author-email: herew26@gmail.com License: Apache License, Version 2.0, see
 LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -21,29 +21,30 @@
  Documentation â¢ Providers â¢ Installation â¢ Quickstart â¢ Contributing
                                   â¢ License
 **PyPayment** is a Python wrapper for API of different payment providers. It is
 designed to be a simple and easy to use library for developers to integrate
 payment into their applications. Main idea is to provide a unified interface
 for different payment providers. For more details see [documentation](https://
 pypayment.readthedocs.io). ## Providers: - [Qiwi P2P](https://p2p.qiwi.com/) -
-[YooMoney](https://yoomoney.ru/) - [PayOk](https://payok.io/) - [Lava](https://
-lava.kz/) *(under development)* ## Installation Install the current version
-with [PyPI](https://pypi.org/project/pypayment/) ```bash pip install -
-U pypayment ``` ## Quickstart Choose payment provider and authorize. For
-example, for Qiwi ```python from pypayment import QiwiPayment
-QiwiPayment.authorize("my_secret_key") ``` Create a payment and get it's `url`
-```python from pypayment import Payment, QiwiPayment payment: Payment =
-QiwiPayment(amount=100) # E.x. commission is 10% print(payment.url) # https://
-oplata.qiwi.com/form/?invoice_uid=payment_unique_id ``` Wait for payment to be
-completed and get it's income Use `update()` method to update payment's
-`status` and `income` ```python from pypayment import PaymentStatus while
-payment.status != PaymentStatus.PAID: input("Press Enter to update payment
-status and income") payment.update() print("Payment is completed!") print
-(payment.income) # 90.0 ``` Summary ```python from pypayment import Payment,
-QiwiPayment, PaymentStatus QiwiPayment.authorize("my_secret_key") payment:
+[YooMoney](https://yoomoney.ru/) - [PayOk](https://payok.io/) - [BetaTransfer]
+(https://betatransfer.io/) - [Lava](https://lava.kz/) *(under development)* ##
+Installation Install the current version with [PyPI](https://pypi.org/project/
+pypayment/) ```bash pip install -U pypayment ``` ## Quickstart Choose payment
+provider and authorize. For example, for Qiwi ```python from pypayment import
+QiwiPayment QiwiPayment.authorize("my_secret_key") ``` Create a payment and get
+it's `url` ```python from pypayment import Payment, QiwiPayment payment:
 Payment = QiwiPayment(amount=100) # E.x. commission is 10% print(payment.url) #
-https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id while
-payment.status != PaymentStatus.PAID: input("Press Enter to update payment
-status") payment.update() print("Payment is completed!") print(payment.income)
-# 90.0 ``` ## Contributing Bug reports and/or pull requests are welcome ##
-License The module is available as open source under the terms of the [Apache
-License, Version 2.0](https://opensource.org/licenses/Apache-2.0)
+https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id ``` Wait for
+payment to be completed and get it's income Use `update()` method to update
+payment's `status` and `income` ```python from pypayment import PaymentStatus
+while payment.status != PaymentStatus.PAID: input("Press Enter to update
+payment status and income") payment.update() print("Payment is completed!")
+print(payment.income) # 90.0 ``` Summary ```python from pypayment import
+Payment, QiwiPayment, PaymentStatus QiwiPayment.authorize("my_secret_key")
+payment: Payment = QiwiPayment(amount=100) # E.x. commission is 10% print
+(payment.url) # https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id
+while payment.status != PaymentStatus.PAID: input("Press Enter to update
+payment status") payment.update() print("Payment is completed!") print
+(payment.income) # 90.0 ``` ## Contributing Bug reports and/or pull requests
+are welcome ## License The module is available as open source under the terms
+of the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-
+2.0)
```

### Comparing `pypayment-1.6.0/README.md` & `pypayment-1.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 For more details see [documentation](https://pypayment.readthedocs.io).
 
 ## Providers:
 - [Qiwi P2P](https://p2p.qiwi.com/)
 - [YooMoney](https://yoomoney.ru/)
 - [PayOk](https://payok.io/)
+- [BetaTransfer](https://betatransfer.io/)
 - [Lava](https://lava.kz/) *(under development)*
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/pypayment/)
 
 ```bash
 pip install -U pypayment
```

#### html2text {}

```diff
@@ -7,29 +7,30 @@
  Documentation â¢ Providers â¢ Installation â¢ Quickstart â¢ Contributing
                                   â¢ License
 **PyPayment** is a Python wrapper for API of different payment providers. It is
 designed to be a simple and easy to use library for developers to integrate
 payment into their applications. Main idea is to provide a unified interface
 for different payment providers. For more details see [documentation](https://
 pypayment.readthedocs.io). ## Providers: - [Qiwi P2P](https://p2p.qiwi.com/) -
-[YooMoney](https://yoomoney.ru/) - [PayOk](https://payok.io/) - [Lava](https://
-lava.kz/) *(under development)* ## Installation Install the current version
-with [PyPI](https://pypi.org/project/pypayment/) ```bash pip install -
-U pypayment ``` ## Quickstart Choose payment provider and authorize. For
-example, for Qiwi ```python from pypayment import QiwiPayment
-QiwiPayment.authorize("my_secret_key") ``` Create a payment and get it's `url`
-```python from pypayment import Payment, QiwiPayment payment: Payment =
-QiwiPayment(amount=100) # E.x. commission is 10% print(payment.url) # https://
-oplata.qiwi.com/form/?invoice_uid=payment_unique_id ``` Wait for payment to be
-completed and get it's income Use `update()` method to update payment's
-`status` and `income` ```python from pypayment import PaymentStatus while
-payment.status != PaymentStatus.PAID: input("Press Enter to update payment
-status and income") payment.update() print("Payment is completed!") print
-(payment.income) # 90.0 ``` Summary ```python from pypayment import Payment,
-QiwiPayment, PaymentStatus QiwiPayment.authorize("my_secret_key") payment:
+[YooMoney](https://yoomoney.ru/) - [PayOk](https://payok.io/) - [BetaTransfer]
+(https://betatransfer.io/) - [Lava](https://lava.kz/) *(under development)* ##
+Installation Install the current version with [PyPI](https://pypi.org/project/
+pypayment/) ```bash pip install -U pypayment ``` ## Quickstart Choose payment
+provider and authorize. For example, for Qiwi ```python from pypayment import
+QiwiPayment QiwiPayment.authorize("my_secret_key") ``` Create a payment and get
+it's `url` ```python from pypayment import Payment, QiwiPayment payment:
 Payment = QiwiPayment(amount=100) # E.x. commission is 10% print(payment.url) #
-https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id while
-payment.status != PaymentStatus.PAID: input("Press Enter to update payment
-status") payment.update() print("Payment is completed!") print(payment.income)
-# 90.0 ``` ## Contributing Bug reports and/or pull requests are welcome ##
-License The module is available as open source under the terms of the [Apache
-License, Version 2.0](https://opensource.org/licenses/Apache-2.0)
+https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id ``` Wait for
+payment to be completed and get it's income Use `update()` method to update
+payment's `status` and `income` ```python from pypayment import PaymentStatus
+while payment.status != PaymentStatus.PAID: input("Press Enter to update
+payment status and income") payment.update() print("Payment is completed!")
+print(payment.income) # 90.0 ``` Summary ```python from pypayment import
+Payment, QiwiPayment, PaymentStatus QiwiPayment.authorize("my_secret_key")
+payment: Payment = QiwiPayment(amount=100) # E.x. commission is 10% print
+(payment.url) # https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id
+while payment.status != PaymentStatus.PAID: input("Press Enter to update
+payment status") payment.update() print("Payment is completed!") print
+(payment.income) # 90.0 ``` ## Contributing Bug reports and/or pull requests
+are welcome ## License The module is available as open source under the terms
+of the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-
+2.0)
```

### Comparing `pypayment-1.6.0/pypayment/exceptions.py` & `pypayment-1.7.0/pypayment/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/pypayment/payment.py` & `pypayment-1.7.0/pypayment/payment.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
         self.status: PaymentStatus = PaymentStatus.WAITING
         """Payment status. Use update() to update it."""
 
         self.income: Optional[float] = None
         """Payment income. Use update() to update it."""
 
+        self._validate_params()
+
         self.url: str = self._create_url()
         """Payment URL."""
 
     @classmethod
     @abstractmethod
     def get_status_and_income(cls, payment_id: str) -> Tuple[Optional[PaymentStatus], float]:
         """Returns payment status and income.
@@ -56,7 +58,11 @@
     def _create_url(self) -> str:
         """Creates payment URL."""
 
     def _check_authorization(self) -> None:
         """Raises NotAuthorized if class was not authorized."""
         if not self.authorized:
             raise NotAuthorized(f"You need to authorize first: {self.__class__.__name__}.authorize()")
+
+    def _validate_params(self) -> None:
+        """Validates payment parameters."""
+        pass
```

### Comparing `pypayment-1.6.0/pypayment/providers/lava.py` & `pypayment-1.7.0/pypayment/providers/lava.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/pypayment/providers/payok.py` & `pypayment-1.7.0/pypayment/providers/payok.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/pypayment/providers/qiwi.py` & `pypayment-1.7.0/pypayment/providers/qiwi.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
         status_literal = payment.get("status")
         status = None
         if status_literal:
             status = QiwiPayment._STATUS_MAP.get(status_literal.get("value"))
 
         amount = payment.get("amount")
-        income = 0
+        income = 0.0
         if amount:
             income = float(amount.get("value"))
 
         return status, income
 
     @classmethod
     def _get_headers(cls) -> Mapping[str, str]:
```

### Comparing `pypayment-1.6.0/pypayment/providers/yoomoney.py` & `pypayment-1.7.0/pypayment/providers/yoomoney.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         if not operations:
             raise PaymentNotFound(f"Payment with id {payment_id} not found for {cls.__name__}.")
 
         payment: Mapping[str, Any] = operations[0]
 
         status = YooMoneyPayment._STATUS_MAP.get(str(payment.get("status")))
-        income = payment.get("amount")
+        income = float(str(payment.get("amount")))
         return status, income
 
     def _create_url(self) -> str:
         data = {
             "receiver": YooMoneyPayment._account_id,
             "quickpay-form": "shop",
             "targets": self.id,
```

### Comparing `pypayment-1.6.0/pypayment.egg-info/PKG-INFO` & `pypayment-1.7.0/pypayment.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypayment
-Version: 1.6.0
+Version: 1.7.0
 Summary: Payment providers API wrapper
 Home-page: https://github.com/TimNekk/pypayment
 Author: TimNekk
 Author-email: herew26@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -56,14 +56,15 @@
 
 For more details see [documentation](https://pypayment.readthedocs.io).
 
 ## Providers:
 - [Qiwi P2P](https://p2p.qiwi.com/)
 - [YooMoney](https://yoomoney.ru/)
 - [PayOk](https://payok.io/)
+- [BetaTransfer](https://betatransfer.io/)
 - [Lava](https://lava.kz/) *(under development)*
 ## Installation
 
 Install the current version with [PyPI](https://pypi.org/project/pypayment/)
 
 ```bash
 pip install -U pypayment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypayment Version: 1.6.0 Summary: Payment providers
+Metadata-Version: 2.1 Name: pypayment Version: 1.7.0 Summary: Payment providers
 API wrapper Home-page: https://github.com/TimNekk/pypayment Author: TimNekk
 Author-email: herew26@gmail.com License: Apache License, Version 2.0, see
 LICENSE file Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
@@ -21,29 +21,30 @@
  Documentation â¢ Providers â¢ Installation â¢ Quickstart â¢ Contributing
                                   â¢ License
 **PyPayment** is a Python wrapper for API of different payment providers. It is
 designed to be a simple and easy to use library for developers to integrate
 payment into their applications. Main idea is to provide a unified interface
 for different payment providers. For more details see [documentation](https://
 pypayment.readthedocs.io). ## Providers: - [Qiwi P2P](https://p2p.qiwi.com/) -
-[YooMoney](https://yoomoney.ru/) - [PayOk](https://payok.io/) - [Lava](https://
-lava.kz/) *(under development)* ## Installation Install the current version
-with [PyPI](https://pypi.org/project/pypayment/) ```bash pip install -
-U pypayment ``` ## Quickstart Choose payment provider and authorize. For
-example, for Qiwi ```python from pypayment import QiwiPayment
-QiwiPayment.authorize("my_secret_key") ``` Create a payment and get it's `url`
-```python from pypayment import Payment, QiwiPayment payment: Payment =
-QiwiPayment(amount=100) # E.x. commission is 10% print(payment.url) # https://
-oplata.qiwi.com/form/?invoice_uid=payment_unique_id ``` Wait for payment to be
-completed and get it's income Use `update()` method to update payment's
-`status` and `income` ```python from pypayment import PaymentStatus while
-payment.status != PaymentStatus.PAID: input("Press Enter to update payment
-status and income") payment.update() print("Payment is completed!") print
-(payment.income) # 90.0 ``` Summary ```python from pypayment import Payment,
-QiwiPayment, PaymentStatus QiwiPayment.authorize("my_secret_key") payment:
+[YooMoney](https://yoomoney.ru/) - [PayOk](https://payok.io/) - [BetaTransfer]
+(https://betatransfer.io/) - [Lava](https://lava.kz/) *(under development)* ##
+Installation Install the current version with [PyPI](https://pypi.org/project/
+pypayment/) ```bash pip install -U pypayment ``` ## Quickstart Choose payment
+provider and authorize. For example, for Qiwi ```python from pypayment import
+QiwiPayment QiwiPayment.authorize("my_secret_key") ``` Create a payment and get
+it's `url` ```python from pypayment import Payment, QiwiPayment payment:
 Payment = QiwiPayment(amount=100) # E.x. commission is 10% print(payment.url) #
-https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id while
-payment.status != PaymentStatus.PAID: input("Press Enter to update payment
-status") payment.update() print("Payment is completed!") print(payment.income)
-# 90.0 ``` ## Contributing Bug reports and/or pull requests are welcome ##
-License The module is available as open source under the terms of the [Apache
-License, Version 2.0](https://opensource.org/licenses/Apache-2.0)
+https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id ``` Wait for
+payment to be completed and get it's income Use `update()` method to update
+payment's `status` and `income` ```python from pypayment import PaymentStatus
+while payment.status != PaymentStatus.PAID: input("Press Enter to update
+payment status and income") payment.update() print("Payment is completed!")
+print(payment.income) # 90.0 ``` Summary ```python from pypayment import
+Payment, QiwiPayment, PaymentStatus QiwiPayment.authorize("my_secret_key")
+payment: Payment = QiwiPayment(amount=100) # E.x. commission is 10% print
+(payment.url) # https://oplata.qiwi.com/form/?invoice_uid=payment_unique_id
+while payment.status != PaymentStatus.PAID: input("Press Enter to update
+payment status") payment.update() print("Payment is completed!") print
+(payment.income) # 90.0 ``` ## Contributing Bug reports and/or pull requests
+are welcome ## License The module is available as open source under the terms
+of the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-
+2.0)
```

### Comparing `pypayment-1.6.0/setup.py` & `pypayment-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/test/test_lava.py` & `pypayment-1.7.0/test/test_lava.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/test/test_payok.py` & `pypayment-1.7.0/test/test_payok.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/test/test_qiwi.py` & `pypayment-1.7.0/test/test_qiwi.py`

 * *Files identical despite different names*

### Comparing `pypayment-1.6.0/test/test_yoomoney.py` & `pypayment-1.7.0/test/test_yoomoney.py`

 * *Files identical despite different names*

