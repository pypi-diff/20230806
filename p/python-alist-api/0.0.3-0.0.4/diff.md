# Comparing `tmp/python-alist-api-0.0.3.tar.gz` & `tmp/python-alist-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-alist-api-0.0.3.tar", last modified: Sun Jul 16 09:45:28 2023, max compression
+gzip compressed data, was "python-alist-api-0.0.4.tar", last modified: Sun Aug  6 13:10:50 2023, max compression
```

## Comparing `python-alist-api-0.0.3.tar` & `python-alist-api-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/alist/
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/public.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/alist/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-16 09:45:14.000000 python-alist-api-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/python_alist_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 09:45:28.000000 python-alist-api-0.0.3/python_alist_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 09:45:28.374380 python-alist-api-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:10:50.901511 python-alist-api-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-08-06 13:10:50.901511 python-alist-api-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:10:50.901511 python-alist-api-0.0.4/alist/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/alist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:10:50.901511 python-alist-api-0.0.4/python_alist_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-08-06 13:10:50.000000 python-alist-api-0.0.4/python_alist_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-06 13:10:50.000000 python-alist-api-0.0.4/python_alist_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:10:50.000000 python-alist-api-0.0.4/python_alist_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 13:10:50.000000 python-alist-api-0.0.4/python_alist_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 13:10:50.000000 python-alist-api-0.0.4/python_alist_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:10:50.901511 python-alist-api-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:10:50.901511 python-alist-api-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/tests/test_basic_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-06 13:10:41.000000 python-alist-api-0.0.4/tests/test_public.py
```

### Comparing `python-alist-api-0.0.3/LICENSE` & `python-alist-api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.3/PKG-INFO` & `python-alist-api-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for the Alist API
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
         
@@ -49,16 +49,28 @@
 
 ## 安装
 
 ```shell
 pip install python-alist-api
 ```
 
+## 测试
+
+安装`pytest`和`pytest-ordering`。
+
+```
+pip install pytest pytest-ordering
+```
+
+在[conftest.py](tests/conftest.py)设置`BASE_URL`和`PASSWORD`。在项目根目录执行`pytest`命令开始测试。
+
 ## 使用方法
 
+完整的信息请参考[文档](https://python-alist-api.readthedocs.io/zh/latest/)。
+
 ### 示例1：创建alist客户端
 
 匿名登录，只能使用`/public` API。
 
 ```python
 from alist import AlistClient
 client = AlistClient('https://your.alist.domain')
```

### Comparing `python-alist-api-0.0.3/README.md` & `python-alist-api-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,28 @@
 
 ## 安装
 
 ```shell
 pip install python-alist-api
 ```
 
+## 测试
+
+安装`pytest`和`pytest-ordering`。
+
+```
+pip install pytest pytest-ordering
+```
+
+在[conftest.py](tests/conftest.py)设置`BASE_URL`和`PASSWORD`。在项目根目录执行`pytest`命令开始测试。
+
 ## 使用方法
 
+完整的信息请参考[文档](https://python-alist-api.readthedocs.io/zh/latest/)。
+
 ### 示例1：创建alist客户端
 
 匿名登录，只能使用`/public` API。
 
 ```python
 from alist import AlistClient
 client = AlistClient('https://your.alist.domain')
```

### Comparing `python-alist-api-0.0.3/alist/__init__.py` & `python-alist-api-0.0.4/alist/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Kai Peng
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 from requests import Session
 from requests import HTTPError
 import json
 from urllib.parse import urlparse
 from alist.public import AlistPublic
 from alist.admin import AlistAdmin
-import hashlib
+from alist import utils
 import alist.setting
 
 
 class AlistClient(object):
     """
     Python wrapper for the Alist API.
     """
@@ -34,55 +34,50 @@
         self.cert = cert
 
         self.url = urlparse(self.base_url)
 
         self.authorization = None
         self.login(password, authorization)
 
-    def calc_authorization(self, password):
-        """ 根据密码计算出 authorization
-        :param password: 登录密码
-        :returns: authorization
+    def login(self, password = None, authorization = None):
         """
-        magic = f'https://github.com/Xhofe/alist-{password}'
-        return hashlib.md5(magic.encode('utf8')).hexdigest()
+        使用password或authorization登录。
 
-    def login(self, password = None, authorization = None):
-        """ 登录
-        :returns:
-            登录成功返回Ture，登录失败触发异常。
+        :param password: 密码
+        :param authorization: 授权码
+        :return: 登录成功返回Ture，登录失败触发异常。
         """
         if self.is_login():
             return True
 
         self.authorization = authorization
         self.password = password
         if self.password != None and self.authorization == None:
-            self.authorization = self.calc_authorization(self.password)
+            self.authorization = utils.calc_authorization(password)
 
         if self.authorization:
             self.admin = AlistAdmin(self)
             return self.admin.login()
         return False
 
     def is_login(self):
-        """ 是否登录
-        :returns:
-            如果已登录，返回True；否则返回Flase。
+        """
+        是否登录
+
+        :return: 如果已登录，返回True；否则返回Flase。
         """
         return self.authorization != None
 
     @staticmethod
     def decode_response(response):
-        """decode a response.
-        :returns:
-            Decoded JSON content as a dict, or raw text if content could not be
-            decoded as JSON.
-        :raises:
-            requests.HTTPError if the response contains an HTTP error status code.
+        """
+        解析服务器的响应。
+
+        :return: 将JSON解析为字典，如果不是JSON则返回原始字符串。
+        :raises: 如果响应包含HTTP错误则触发requests.HTTPError。
         """
         content_type = response.headers.get("content-type", "")
 
         content = response.content.strip()
         if response.encoding:
             content = content.decode(response.encoding)
         if not content:
@@ -101,16 +96,20 @@
         if content['data'] is None:
             return True
         else:
             return content['data']
 
     def get_request_dict(self, method, endpoint, **kwargs):
         """
-        :param kwargs:
-        :return:
+        获取requests请求参数。
+
+        :param method: 请求方法，GET、POST或DELETE。
+        :param endpoint: URL端点。
+        :param kwargs: 其他可选参数。
+        :return: requests请求参数。
         """
         headers = {
             "Method": method,
             "Path": self.get_api_url(endpoint),
             "Authority": self.url.hostname,
             "Scheme": self.url.scheme,
             "Accept": "application/json, text/plain, */*",
@@ -126,57 +125,59 @@
         request_kwargs['verify'] = self.ssl_verify
         request_kwargs['cert']   = self.cert
 
         return request_kwargs
 
     def get_api_url(self, endpoint):
         """
-        Return the api url including host and port for a given endpoint.
-        :param endpoint: service endpoint as str
-        :return: api url (including host and port) as str
+        返回指定端点的api url，不包含主机和端口。
+
+        :param endpoint: 服务端点。
+        :return: api url
         """
         return f'/api{endpoint}'
 
     def get_endpoint_url(self, endpoint):
         """
-        Return the complete url including host and port for a given endpoint.
-        :param endpoint: service endpoint as str
-        :return: complete url (including host and port) as str
+        返回指定端点的完整URL，包含主机和端口。
+
+        :param endpoint: 服务端点。
+        :return: 完整的URL。
         """
 
         return f'{self.base_url}{self.get_api_url(endpoint)}'
 
     def get(self, endpoint, **kwargs):
         """
-        Send HTTP GET to the endpoint.
+        发送HTTP GET请求到端点。
 
-        :param endpoint: The endpoint to send to.
-        :return:
+        :param endpoint: 发送请求的端点。
+        :return: 服务器返回的数据。
         """
         request_kwargs = self.get_request_dict("GET", endpoint, **kwargs)
         response = self.session.get(self.get_endpoint_url(endpoint), **request_kwargs)
         return self.decode_response(response)
 
     def post(self, endpoint, **kwargs):
         """
-        Send HTTP POST to the endpoint.
+        发送HTTP POST请求到端点。
 
-        :param endpoint: The endpoint to send to.
-        :return:
+        :param endpoint: 发送请求的端点。
+        :return: 服务器返回的数据。
         """
         request_kwargs = self.get_request_dict("POST", endpoint, **kwargs)
         response = self.session.post(self.get_endpoint_url(endpoint), **request_kwargs)
         # return response
         return self.decode_response(response)
 
     def delete(self, endpoint, **kwargs):
         """
-        Send HTTP DELETE to the endpoint.
+        发送HTTP DELETE请求到端点。
 
-        :param endpoint: The endpoint to send to.
-        :return:
+        :param endpoint: 发送请求的端点。
+        :return: 服务器返回的数据。
         """
         request_kwargs = self.get_request_dict("DELETE", endpoint, **kwargs)
         response = self.session.delete(self.get_endpoint_url(endpoint), **request_kwargs)
         # return response
         return self.decode_response(response)
```

### Comparing `python-alist-api-0.0.3/alist/driver.py` & `python-alist-api-0.0.4/alist/driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 # @Author: Kai Peng
 
 from copy import deepcopy
 from typing import Any
 
 class AlistDriverAttribute(dict):
     """
-    驱动属性
+    驱动属性。驱动包含 ``name``、``label``、``type``、``default``、
+    ``values``、``required``、``description`` 等字段。所有字段初始化之后无法修改。
     """
 
     def __init__(self, **attr):
         super().__init__()
 
         for key in ['name', 'label', 'type', 'default',
                     'values', 'required', 'description']:
             super().__setitem__(key, attr[key])
 
     def get_name(self):
+        """获取驱动属性的名字"""
         return self['name']
 
     def is_required(self):
+        """属性是否必须提供。返回True表示必须提供。"""
         return self['required']
 
     def __str__(self) -> str:
         return f'attr: {self.get_name()} required: {self["required"]}'
 
     def __repr__(self) -> str:
         return self.__str__()
@@ -33,32 +36,39 @@
         raise NotImplemented
 
     def __delitem__(self, __key: Any) -> None:
         raise NotImplemented
 
 class AlistDriver(object):
     """
-    驱动
+    描述Alist驱动。一个驱动包含若干个属性。
     """
     def __init__(self, name, attrs):
         self.name = name
         self.attrs = list()
         for attr in attrs:
             self.attrs.append(AlistDriverAttribute(**attr))
 
-    def get_attr(self, name):
+    def get_attr(self, name) -> AlistDriverAttribute:
+        """
+        获取驱动属性。
+
+        :param name: 属性的名字
+        """
         for attr in self.attrs:
             if name == attr['name']:
                 return attr
         raise KeyError(f"{name} not found")
 
     def get_name(self):
+        """获取驱动的名字"""
         return self.name
 
     def get_required(self):
+        """获取驱动必须提供的属性"""
         required = list()
         for attr in self.attrs:
             if attr['required']:
                 required.append(attr.get_name())
         return required
 
     def __str__(self) -> str:
@@ -68,40 +78,45 @@
         return s
 
     def __repr__(self) -> str:
         return self.__str__()
 
 class AlistAdminDrivers(object):
     """
-    驱动列表
+    驱动列表。api ``/api/admin/drivers`` 的实现。
     """
     drivers = list()
 
     def __init__(self, alist, endpoint) -> None:
         self.alist = alist
         self.endpoint = f'{endpoint}/drivers'
         self.drivers = deepcopy(self.drivers)
 
     def get(self):
-        """ 获取驱动列表，包含驱动需要配置的字段列表
-        :returns:
-            驱动列表
+        """ 获取所有驱动的列表，包含驱动必须提供的属性。
+
+        :return: 驱动列表
         """
         if len(self.drivers) == 0:
             results = self.alist.get(self.endpoint)
             for name in results:
                 self.drivers.append(AlistDriver(name, results[name]))
                 func_name = f"driver_{name.replace('.', '_')}"
                 setattr(self.alist, func_name, self._factory_get_driver(name))
         return self.drivers
 
     def __call__(self) -> Any:
         return self.get()
 
-    def get_driver(self, name):
+    def get_driver(self, name) -> AlistDriver:
+        """
+        获取指定名字的驱动。
+
+        :param name: 驱动的名字。
+        """
         drivers = self.get()
         for d in drivers:
             if d.get_name() == name:
                 return d
         raise KeyError(f'driver \'{name}\' not found')
 
     def  _factory_get_driver(self, name):
```

### Comparing `python-alist-api-0.0.3/pyproject.toml` & `python-alist-api-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-alist-api-0.0.3/python_alist_api.egg-info/PKG-INFO` & `python-alist-api-0.0.4/python_alist_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-alist-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for the Alist API
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
         
@@ -49,16 +49,28 @@
 
 ## 安装
 
 ```shell
 pip install python-alist-api
 ```
 
+## 测试
+
+安装`pytest`和`pytest-ordering`。
+
+```
+pip install pytest pytest-ordering
+```
+
+在[conftest.py](tests/conftest.py)设置`BASE_URL`和`PASSWORD`。在项目根目录执行`pytest`命令开始测试。
+
 ## 使用方法
 
+完整的信息请参考[文档](https://python-alist-api.readthedocs.io/zh/latest/)。
+
 ### 示例1：创建alist客户端
 
 匿名登录，只能使用`/public` API。
 
 ```python
 from alist import AlistClient
 client = AlistClient('https://your.alist.domain')
```

