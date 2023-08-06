# Comparing `tmp/CFSession-1.0.0.tar.gz` & `tmp/CFSession-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CFSession-1.0.0.tar", last modified: Thu Jul 20 08:28:40 2023, max compression
+gzip compressed data, was "dist\CFSession-1.1.0.tar", last modified: Sun Aug  6 12:32:59 2023, max compression
```

## Comparing `CFSession-1.0.0.tar` & `CFSession-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:28:40.000000 CFSession-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession/
--rw-rw-rw-   0        0        0      472 2022-11-30 08:50:37.000000 CFSession-1.0.0/CFSession/__init__.py
--rw-rw-rw-   0        0        0     8147 2023-07-19 22:02:31.000000 CFSession-1.0.0/CFSession/cf.py
--rw-rw-rw-   0        0        0    12589 2023-07-20 06:57:53.000000 CFSession-1.0.0/CFSession/cfbrowser.py
--rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-1.0.0/CFSession/cfcookie.py
--rw-rw-rw-   0        0        0     1807 2023-07-19 17:41:30.000000 CFSession-1.0.0/CFSession/cfdefaults.py
--rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-1.0.0/CFSession/cfdirmodel.py
--rw-rw-rw-   0        0        0     2882 2023-04-09 04:00:18.000000 CFSession-1.0.0/CFSession/cfexception.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/
--rw-rw-rw-   0        0        0     3664 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 08:28:40.000000 CFSession-1.0.0/CFSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3664 2023-07-20 08:28:40.000000 CFSession-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2023-07-19 19:15:56.000000 CFSession-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-20 08:28:40.000000 CFSession-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-14 17:12:54.000000 CFSession-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 12:32:59.000000 CFSession-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-08-06 12:32:59.000000 CFSession-1.1.0/CFSession/
+-rw-rw-rw-   0        0        0      515 2023-08-06 11:58:53.000000 CFSession-1.1.0/CFSession/__init__.py
+-rw-rw-rw-   0        0        0     8180 2023-08-06 12:03:13.000000 CFSession-1.1.0/CFSession/cf.py
+-rw-rw-rw-   0        0        0    12753 2023-08-06 12:08:31.000000 CFSession-1.1.0/CFSession/cfbrowser.py
+-rw-rw-rw-   0        0        0      802 2022-10-24 18:04:11.000000 CFSession-1.1.0/CFSession/cfcookie.py
+-rw-rw-rw-   0        0        0     1958 2023-08-06 11:56:03.000000 CFSession-1.1.0/CFSession/cfdefaults.py
+-rw-rw-rw-   0        0        0     1338 2022-10-24 18:04:11.000000 CFSession-1.1.0/CFSession/cfdirmodel.py
+-rw-rw-rw-   0        0        0     2882 2023-04-09 04:00:18.000000 CFSession-1.1.0/CFSession/cfexception.py
+drwxrwxrwx   0        0        0        0 2023-08-06 12:32:59.000000 CFSession-1.1.0/CFSession.egg-info/
+-rw-rw-rw-   0        0        0     3664 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 12:32:57.000000 CFSession-1.1.0/CFSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-10-24 18:04:11.000000 CFSession-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3664 2023-08-06 12:32:59.000000 CFSession-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2023-07-20 10:13:27.000000 CFSession-1.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-06 12:32:59.000000 CFSession-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-08-05 19:24:50.000000 CFSession-1.1.0/setup.py
```

### Comparing `CFSession-1.0.0/CFSession/cf.py` & `CFSession-1.1.0/CFSession/cf.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,42 +11,40 @@
 #Modules
 from .cfdefaults import Required_defaults
 from pathlib import Path
 import typing
 import time
 import sys
 import json
-import threading
 
 #Not a constant. CAPITAL for more readable syntax
 #If constant is ever declared we will use CONST_VARIABLE_NAME
 IGNORE_WARN = True
 STDOUT = False
 DEBUG = False
 DUMMY = False
 
 def de_print(text: str):
     if DEBUG:
         try:
             print(text)
         except UnicodeEncodeError:
             print("Uni Err, ascii md")
-            text = text.encode('ascii', 'ignore')
-            print(text)
+            print(text.encode('ascii', 'ignore'))
         except Exception as e:
             print("[warn] Error occured on a debugger de", e)
     
     
-def norm_print(text):
+def norm_print(text: str):
     if STDOUT or DEBUG:
-        text = text.encode('ascii', 'ignore')
         try:
             print(text)
         except UnicodeEncodeError:
-            print("Unicode error occured cannot print")
+            print("Uni Err, ascii md")
+            print(text.encode('ascii', 'ignore'))
         except Exception as e:
             print("[warn] Error occured on a debugger norm", e)
 
 def warn_print(text, level: int = 2): # 0-Important, 1-If possible, 2-Unimportant (debug purposes)
     acceptable = STDOUT + DEBUG
     if IGNORE_WARN and not DEBUG:
         return
@@ -66,41 +64,41 @@
         self.directory = directory
         self.timeout = timeout
         self.bypass_mode = bypass_mode
     
     def start(self):
         return self._main_process()
     
-    def find_element(self, element, max_attempts=3):
+    def find_element(self, element, max_attempts=3, target: uc.Chrome =False):
         attempt = 1
         while True:
             de_print(f"Finding element: {element}")
             try:
+                if target:
+                    target.find_element(*element)
                 return self.driver.find_element(*element)
             except StaleElementReferenceException as e:
                 de_print(f"Error element stale {attempt}/{max_attempts} {e}")
                 if attempt == max_attempts:
                     raise
+                time.sleep(1)
                 attempt += 1
 
     def init_bypass(self):
         WaitFor = lambda i: WebDriverWait(self.driver, 10).until(
             EC.visibility_of(
             self.find_element(
             (By.TAG_NAME, 'body'),
             ))) and time.sleep(i)
         self.driver.execute_script(f'window.open("{self.website}","_blank");')
         WaitFor(5)
         self.driver.switch_to.window(window_name=self.driver.window_handles[0])
         self.driver.close() # close first tab
         self.driver.switch_to.window(window_name=self.driver.window_handles[0]) 
         WaitFor(2)
-        self.driver.get("https://google.com")
-        WaitFor(2)
-        self.driver.get(self.website)
         
     def _main_process(self):
         timeout = 0
         if self.bypass_mode: self.init_bypass()
         while any(ext in self.driver.title for ext in self.TARGET_NAME):
             timeout += 1
             if timeout >= self.timeout:
@@ -109,14 +107,15 @@
             de_print(f"cur: {self.driver.title}")
             time.sleep(1)
         else:
             de_print(self.driver.title)
             de_print("Done")
             self.save_cookie_verified()
             return True
+        de_print("Failed to bypass, return failure")
         return False
 
     def save_cookie(self, driver, file):
         """Cookie save, requires driver and file"""
         json.dump(driver, file)
```

### Comparing `CFSession-1.0.0/CFSession/cfbrowser.py` & `CFSession-1.1.0/CFSession/cfbrowser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CFSession.cfbrowser
 ~~~~~~~~~~~~~
 This module contains the wrapper for Requests
 """
 from .cfexception import CFException, CloudflareBlocked, HTTPError, NetworkError, NotFound, URLRequired, TooManyRedirects, Timeout, ConnectTimeout, ReadTimeout
 from .cf import CFBypass, SiteBrowserProcess
 from .cfdirmodel import cfDirectory    
+from .cfdefaults import cfConstant
 from datetime import timezone
 import requests
 import datetime
 from typing import Union
 import json
 import os
 
@@ -133,26 +134,30 @@
         
     def set_cookies(self):
         try:
             cookies = json.load(open(self.directory.cookie_path(),"r"))
             selenium_headers = json.load(open(self.directory.session_path(),"r"))
         except FileNotFoundError:
             return False
-        self.session.headers.update({"user-agent": selenium_headers})
+        self.set_agent(selenium_headers)
         for cookie in cookies:
             self.session.cookies.set(cookie['name'], cookie['value'], domain=cookie['domain'])
         return True
+    
+    def set_agent(self, user_agent=cfConstant.USER_AGENT):
+        self.session.headers.update({"user-agent": user_agent})
 
     def _handle_equalfunc(self):
         if not self._setcookies_status:
             self.reload_token(self.url)
             self.set_cookies()
 
     def request(self,method,url,**kwargs) -> requests.Response:
         content = None
+        self.set_agent()
         for t in range(0,self.tries):
             try:
                 if method == "GET":
                     content = self.session.get(url, **kwargs)
                 elif method == "POST":
                     content = self.session.post(url, **kwargs)
                 elif method == "PATCH":
```

### Comparing `CFSession-1.0.0/CFSession/cfcookie.py` & `CFSession-1.1.0/CFSession/cfcookie.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.0.0/CFSession/cfdefaults.py` & `CFSession-1.1.0/CFSession/cfdefaults.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,7 +43,10 @@
             self.reset_objects()
             return self.options_default()
         return self.options
 
     def desired_capabilites_default(self) -> DesiredCapabilities:
         self.dcp["pageLoadStrategy"] = "eager"
         return self.dcp
+
+class cfConstant:
+    USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
```

### Comparing `CFSession-1.0.0/CFSession/cfdirmodel.py` & `CFSession-1.1.0/CFSession/cfdirmodel.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.0.0/CFSession/cfexception.py` & `CFSession-1.1.0/CFSession/cfexception.py`

 * *Files identical despite different names*

### Comparing `CFSession-1.0.0/CFSession.egg-info/PKG-INFO` & `CFSession-1.1.0/CFSession.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFSession
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Cloudflare IUAM session grabber
 Home-page: https://github.com/Kinuseka/CFSession
 Author: Kinuseka
 Author-email: realkingseeker1089@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `CFSession-1.0.0/LICENSE` & `CFSession-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CFSession-1.0.0/PKG-INFO` & `CFSession-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CFSession
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Cloudflare IUAM session grabber
 Home-page: https://github.com/Kinuseka/CFSession
 Author: Kinuseka
 Author-email: realkingseeker1089@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `CFSession-1.0.0/README.md` & `CFSession-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `CFSession-1.0.0/setup.py` & `CFSession-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setup(
     name='CFSession',
-    version='1.0.0',
+    version='1.1.0',
     author='Kinuseka',
     author_email='realkingseeker1089@gmail.com',
     description='A Cloudflare IUAM session grabber',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Kinuseka/CFSession',
     classifiers=[
```

