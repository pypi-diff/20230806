# Comparing `tmp/playwright-recaptcha-0.3.1.tar.gz` & `tmp/playwright-recaptcha-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright-recaptcha-0.3.1.tar", last modified: Sat Jul 29 16:06:56 2023, max compression
+gzip compressed data, was "playwright-recaptcha-0.3.2.tar", last modified: Sun Aug  6 19:31:20 2023, max compression
```

## Comparing `playwright-recaptcha-0.3.1.tar` & `playwright-recaptcha-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19240 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/recaptcha_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/sync_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/sync_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_async_recaptchav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_async_recaptchav3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_sync_recaptchav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_sync_recaptchav3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:31:20.068080 playwright-recaptcha-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-06 19:31:20.068080 playwright-recaptcha-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:31:20.064080 playwright-recaptcha-0.3.2/playwright_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:31:20.064080 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/recaptcha_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:31:20.068080 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav3/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav3/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav3/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:31:20.064080 playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-08-06 19:31:20.000000 playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-06 19:31:20.000000 playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:31:20.000000 playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-06 19:31:20.000000 playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 19:31:20.000000 playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:31:20.068080 playwright-recaptcha-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:31:20.068080 playwright-recaptcha-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/tests/test_async_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/tests/test_async_recaptchav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/tests/test_sync_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-06 19:31:10.000000 playwright-recaptcha-0.3.2/tests/test_sync_recaptchav3.py
```

### Comparing `playwright-recaptcha-0.3.1/LICENSE` & `playwright-recaptcha-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/PKG-INFO` & `playwright-recaptcha-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-recaptcha
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
 Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
 Author: Xewdy444
 Author-email: xewdy@xewdy.tech
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.1 Summary: A
+Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.2 Summary: A
 library for solving reCAPTCHA v2 and v3 with Playwright Home-page: https://
 github.com/Xewdy444/Playwright-reCAPTCHA Author: Xewdy444 Author-email:
 xewdy@xewdy.tech License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `playwright-recaptcha-0.3.1/README.md` & `playwright-recaptcha-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/__init__.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A library for solving reCAPTCHA v2 and v3 with Playwright."""
 
 __author__ = "Xewdy444"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __license__ = "MIT"
 
 from playwright_recaptcha.errors import (
     CapSolverError,
     RecaptchaError,
     RecaptchaNotFoundError,
     RecaptchaRateLimitError,
```

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/errors.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/errors.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/async_solver.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/async_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     ) -> None:
         self._page = page
         self._attempts = attempts
         self._capsolver_api_key = capsolver_api_key or os.getenv("CAPSOLVER_API_KEY")
 
         self._token: Optional[str] = None
         self._payload_response: Union[APIResponse, Response, None] = None
-        self._page.on("response", self._response_listener)
+        self._page.on("response", self._response_callback)
 
     def __repr__(self) -> str:
         return (
             f"AsyncSolver(page={self._page!r}, "
             f"attempts={self._attempts!r}, "
             f"capsolver_api_key={self._capsolver_api_key!r})"
         )
@@ -108,17 +108,17 @@
 
         for object_name, object_id in object_dict.items():
             if object_name in task[0]:
                 return object_id
 
         return None
 
-    async def _response_listener(self, response: Response) -> None:
+    async def _response_callback(self, response: Response) -> None:
         """
-        Listen for payload and userverify responses.
+        The callback for intercepting payload and userverify responses.
 
         Parameters
         ----------
         response : Response
             The response.
         """
         if (
@@ -513,23 +513,18 @@
             await recaptcha_box.checkbox.is_hidden()
             and await recaptcha_box.audio_challenge_button.is_disabled()
         ):
             raise RecaptchaNotFoundError
 
         return recaptcha_box
 
-    @property
-    def token(self) -> Optional[str]:
-        """The `g-recaptcha-response` token."""
-        return self._token
-
     def close(self) -> None:
         """Remove the response listener."""
         try:
-            self._page.remove_listener("response", self._response_listener)
+            self._page.remove_listener("response", self._response_callback)
         except KeyError:
             pass
 
     async def solve_recaptcha(
         self,
         *,
         attempts: Optional[int] = None,
```

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/recaptcha_box.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/recaptcha_box.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/sync_solver.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav2/sync_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     ) -> None:
         self._page = page
         self._attempts = attempts
         self._capsolver_api_key = capsolver_api_key or os.getenv("CAPSOLVER_API_KEY")
 
         self._token: Optional[str] = None
         self._payload_response: Union[APIResponse, Response, None] = None
-        self._page.on("response", self._response_listener)
+        self._page.on("response", self._response_callback)
 
     def __repr__(self) -> str:
         return (
             f"SyncSolver(page={self._page!r}, "
             f"attempts={self._attempts!r}, "
             f"capsolver_api_key={self._capsolver_api_key!r})"
         )
@@ -100,17 +100,17 @@
 
         for object_name, object_id in object_dict.items():
             if object_name in task[0]:
                 return object_id
 
         return None
 
-    def _response_listener(self, response: Response) -> None:
+    def _response_callback(self, response: Response) -> None:
         """
-        Listen for payload and userverify responses.
+        The callback for intercepting payload and userverify responses.
 
         Parameters
         ----------
         response : Response
             The response.
         """
         if (
@@ -486,23 +486,18 @@
             recaptcha_box.checkbox.is_hidden()
             and recaptcha_box.audio_challenge_button.is_disabled()
         ):
             raise RecaptchaNotFoundError
 
         return recaptcha_box
 
-    @property
-    def token(self) -> Optional[str]:
-        """The `g-recaptcha-response` token."""
-        return self._token
-
     def close(self) -> None:
         """Remove the response listener."""
         try:
-            self._page.remove_listener("response", self._response_listener)
+            self._page.remove_listener("response", self._response_callback)
         except KeyError:
             pass
 
     def solve_recaptcha(
         self,
         *,
         attempts: Optional[int] = None,
```

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/async_solver.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav3/async_solver.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/sync_solver.py` & `playwright-recaptcha-0.3.2/playwright_recaptcha/recaptchav3/sync_solver.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/PKG-INFO` & `playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-recaptcha
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
 Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
 Author: Xewdy444
 Author-email: xewdy@xewdy.tech
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.1 Summary: A
+Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.2 Summary: A
 library for solving reCAPTCHA v2 and v3 with Playwright Home-page: https://
 github.com/Xewdy444/Playwright-reCAPTCHA Author: Xewdy444 Author-email:
 xewdy@xewdy.tech License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/SOURCES.txt` & `playwright-recaptcha-0.3.2/playwright_recaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/setup.py` & `playwright-recaptcha-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as file:
     long_description = file.read()
 
 setup(
     name="playwright-recaptcha",
-    version="0.3.1",
+    version="0.3.2",
     author="Xewdy444",
     author_email="xewdy@xewdy.tech",
     description="A library for solving reCAPTCHA v2 and v3 with Playwright",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xewdy444/Playwright-reCAPTCHA",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
-        "playwright==1.36.0",
+        "playwright>=1.33.0",
         "pydub==0.25.1",
         "SpeechRecognition==3.10.0",
         "tenacity==8.2.2",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

### Comparing `playwright-recaptcha-0.3.1/tests/test_async_recaptchav2.py` & `playwright-recaptcha-0.3.2/tests/test_async_recaptchav2.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/tests/test_async_recaptchav3.py` & `playwright-recaptcha-0.3.2/tests/test_async_recaptchav3.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/tests/test_sync_recaptchav2.py` & `playwright-recaptcha-0.3.2/tests/test_sync_recaptchav2.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.1/tests/test_sync_recaptchav3.py` & `playwright-recaptcha-0.3.2/tests/test_sync_recaptchav3.py`

 * *Files identical despite different names*

