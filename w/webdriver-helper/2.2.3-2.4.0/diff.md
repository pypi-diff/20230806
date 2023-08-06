# Comparing `tmp/webdriver_helper-2.2.3-py3-none-any.whl.zip` & `tmp/webdriver_helper-2.4.0-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,14 @@
-Zip file size: 4254 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       86 b- defN 16-Jan-01 00:00 webdriver_helper/__init__.pyi
--rw-rw-rw-  2.0 fat      691 b- defN 16-Jan-01 00:00 webdriver_helper/driver.pyi
--rw-rw-rw-  2.0 fat     2513 b- defN 16-Jan-01 00:00 webdriver_helper/pom.pyi
+Zip file size: 207443 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      120 b- defN 16-Jan-01 00:00 webdriver_helper/__init__.pyi
+-rw-rw-rw-  2.0 fat     1596 b- defN 16-Jan-01 00:00 webdriver_helper/_driver.pyi
+-rw-rw-rw-  2.0 fat      504 b- defN 16-Jan-01 00:00 webdriver_helper/driver.pyi
+-rw-rw-rw-  2.0 fat     2459 b- defN 16-Jan-01 00:00 webdriver_helper/pom.pyi
 -rw-rw-rw-  2.0 fat     1717 b- defN 16-Jan-01 00:00 webdriver_helper/upload_by_drop.js
-?rw-------  2.0 fat       87 b- defN 16-Jan-01 00:00 webdriver_helper-2.2.3.dist-info/WHEEL
-?rw-------  2.0 fat     1292 b- defN 16-Jan-01 00:00 webdriver_helper-2.2.3.dist-info/METADATA
-?rw-------  2.0 fat      572 b- defN 16-Jan-01 00:00 webdriver_helper-2.2.3.dist-info/RECORD
-7 files, 6958 bytes uncompressed, 3236 bytes compressed:  53.5%
+-rw-rw-rw-  2.0 fat    77312 b- defN 16-Jan-01 00:00 webdriver_helper/driver.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   221696 b- defN 16-Jan-01 00:00 webdriver_helper/pom.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   137728 b- defN 16-Jan-01 00:00 webdriver_helper/_driver.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    29696 b- defN 16-Jan-01 00:00 webdriver_helper/__init__.cp310-win_amd64.pyd
+?rw-------  2.0 fat       97 b- defN 16-Jan-01 00:00 webdriver_helper-2.4.0.dist-info/WHEEL
+?rw-------  2.0 fat     1374 b- defN 16-Jan-01 00:00 webdriver_helper-2.4.0.dist-info/METADATA
+?rw-------  2.0 fat     1064 b- defN 16-Jan-01 00:00 webdriver_helper-2.4.0.dist-info/RECORD
+12 files, 475363 bytes uncompressed, 205645 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -1,22 +1,37 @@
 Filename: webdriver_helper/__init__.pyi
 Comment: 
 
+Filename: webdriver_helper/_driver.pyi
+Comment: 
+
 Filename: webdriver_helper/driver.pyi
 Comment: 
 
 Filename: webdriver_helper/pom.pyi
 Comment: 
 
 Filename: webdriver_helper/upload_by_drop.js
 Comment: 
 
-Filename: webdriver_helper-2.2.3.dist-info/WHEEL
+Filename: webdriver_helper/driver.cp310-win_amd64.pyd
+Comment: 
+
+Filename: webdriver_helper/pom.cp310-win_amd64.pyd
+Comment: 
+
+Filename: webdriver_helper/_driver.cp310-win_amd64.pyd
+Comment: 
+
+Filename: webdriver_helper/__init__.cp310-win_amd64.pyd
+Comment: 
+
+Filename: webdriver_helper-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: webdriver_helper-2.2.3.dist-info/METADATA
+Filename: webdriver_helper-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: webdriver_helper-2.2.3.dist-info/RECORD
+Filename: webdriver_helper-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webdriver_helper/__init__.pyi

```diff
@@ -1,3 +1,3 @@
-from .driver import debugger as debugger, get_webdriver as get_webdriver
+from .driver import debugger as debugger, get_webdriver as get_webdriver, upload_by_drop as upload_by_drop
 
 msg: str
```

## webdriver_helper/driver.pyi

```diff
@@ -1,16 +1,10 @@
 from _typeshed import Incomplete
-from appium.webdriver.webdriver import WebDriver
-from pathlib import Path
 from selenium.webdriver.common.options import ArgOptions as ArgOptions
 from typing import Optional
+from webdriver_helper._driver import WebDriver as WebDriver, WebElement as WebElement
 
-session: Incomplete
 DriverType: Incomplete
 
 def get_webdriver(driver_type: DriverType = ..., *, hub: str = ..., version: Incomplete | None = ..., options: Optional[ArgOptions] = ..., service_args: Optional[dict] = ..., capabilities: Optional[dict] = ...) -> WebDriver: ...
-def debugger(driver): ...
 
-class WebDriverPatch:
-    def set_download_path(self, path: Path): ...
-    def set_think_time(self, think_time: float): ...
-    def execute(self, *args, **kwargs): ...
+debugger: Incomplete
```

## webdriver_helper/pom.pyi

```diff
@@ -1,17 +1,16 @@
 from _typeshed import Incomplete
 from abc import ABCMeta
 from collections import UserList
-from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.common.alert import Alert
 from selenium.webdriver.common.by import By as By
-from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.wait import WebDriverWait
 from typing import List, Optional
+from webdriver_helper.driver import WebDriver, WebElement
 
 class PageMeta(ABCMeta):
     driver: WebDriver
     wait: WebDriverWait
     time_out: float
     poll: float
     url: str
@@ -31,15 +30,15 @@
     check_on_init: Incomplete
     time_out: Incomplete
     poll: Incomplete
     def __init__(self, by, value, check_on_init: bool = ..., time_out: Incomplete | None = ..., poll: Incomplete | None = ..., *args, **kwargs) -> None: ...
 
 class LazyElementList(LazyElement, UserList):
     def __new__(cls, *args, **kwargs) -> UserList[WebElement]: ...
-    def __len__(self): ...
+    def __len__(self) -> int: ...
     def __getitem__(self, index): ...
     def __iter__(self): ...
 
 class LazyAlert(BaseLazy, Alert):
     check_on_init: Incomplete
     time_out: Incomplete
     poll: Incomplete
```

## Comparing `webdriver_helper-2.2.3.dist-info/METADATA` & `webdriver_helper-2.4.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: webdriver-helper
-Version: 2.2.3
+Version: 2.4.0
 Summary: 自动下载浏览器驱动，使selenium 4.0开箱即用，并一些提高增强的功能
 License: Apache-2.0
 Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
 Requires-Python: >=3.9
-Requires-Dist: Appium-Python-Client>=2.6.0
+Requires-Dist: Appium-Python-Client==2.11.1
 Requires-Dist: parse==1.19.0
-Requires-Dist: selenium>=4.0.0
-Requires-Dist: webdriver-manager==3.8.5
+Requires-Dist: selenium==4.11.2
 Project-URL: Homepage, https://github.com/dongfangtianyu/webdriver-helper
 Description-Content-Type: text/markdown
 
 # WebDriver助手
 
 WebDriver助手（webdriver-helpler）是一个第三方库，通过增加一些额外的能力，让selenium更加好用
 
@@ -28,7 +27,8 @@
 
 
 
 
 ## 链接
 - [webdriver-helper安装说明](https://mp.weixin.qq.com/s/vvzdZsQVGLohROZyU_JD1w)
 - [WebDriver助手 2.2.0使用说明](https://mp.weixin.qq.com/s/fvdWRfZowsmcGt8jprgOsw)
+- [Web自动化测试注意：chromedriver 115改变了发布方式](https://mp.weixin.qq.com/s/du3Evw4PtpKOrozPD_xqjA)
```

