# Comparing `tmp/manageritm-0.1.0.tar.gz` & `tmp/manageritm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manageritm-0.1.0.tar", max compression
+gzip compressed data, was "manageritm-0.3.0.tar", max compression
```

## Comparing `manageritm-0.1.0.tar` & `manageritm-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1072 2022-10-09 16:18:57.113764 manageritm-0.1.0/LICENSE
--rw-r--r--   0        0        0     2199 2022-10-09 16:18:57.113764 manageritm-0.1.0/README.md
--rw-r--r--   0        0        0       65 2022-10-09 16:18:57.841772 manageritm-0.1.0/manageritm/__init__.py
--rw-r--r--   0        0        0      806 2022-10-09 16:18:57.113764 manageritm-0.1.0/manageritm/app.py
--rw-r--r--   0        0        0       75 2022-10-09 16:18:57.113764 manageritm-0.1.0/manageritm/client/__init__.py
--rw-r--r--   0        0        0     2298 2022-10-09 16:18:57.113764 manageritm-0.1.0/manageritm/client/manageritm_client.py
--rw-r--r--   0        0        0      561 2022-10-09 16:18:57.113764 manageritm-0.1.0/manageritm/server/__init__.py
--rw-r--r--   0        0        0     2233 2022-10-09 16:18:57.113764 manageritm-0.1.0/manageritm/server/process_minder.py
--rw-r--r--   0        0        0     5252 2022-10-09 16:18:57.113764 manageritm-0.1.0/manageritm/server/routes.py
--rw-r--r--   0        0        0     7369 2022-10-09 16:18:57.117765 manageritm-0.1.0/manageritm/server/scripts/har_dump.py
--rw-r--r--   0        0        0     1000 2022-10-09 16:18:57.853772 manageritm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3245 1970-01-01 00:00:00.000000 manageritm-0.1.0/setup.py
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 manageritm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-06 19:23:12.187130 manageritm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3135 2023-08-06 19:23:12.187130 manageritm-0.3.0/README.md
+-rw-r--r--   0        0        0       53 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/__init__.py
+-rw-r--r--   0        0        0      866 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/app.py
+-rw-r--r--   0        0        0      741 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/__init__.py
+-rw-r--r--   0        0        0      109 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/client/__init__.py
+-rw-r--r--   0        0        0     4443 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/client/routes.py
+-rw-r--r--   0        0        0      105 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/main/__init__.py
+-rw-r--r--   0        0        0     2151 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/main/routes.py
+-rw-r--r--   0        0        0     3196 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/process_minder.py
+-rw-r--r--   0        0        0       19 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/processes.py
+-rw-r--r--   0        0        0     7413 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/scripts/har_dump.py
+-rw-r--r--   0        0        0      882 2023-08-06 19:23:12.187130 manageritm-0.3.0/manageritm/server/utils.py
+-rw-r--r--   0        0        0     1069 2023-08-06 19:23:13.283174 manageritm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 manageritm-0.3.0/PKG-INFO
```

### Comparing `manageritm-0.1.0/LICENSE` & `manageritm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manageritm-0.1.0/README.md` & `manageritm-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -17,31 +17,70 @@
 
    import manageritm
 
    manageritm_addr = "localhost"
    manageritm_port = "8000"
 
    # create a manageritm client
-   mc = manageritm.client.ManagerITMClient(f'http://{manageritm_addr}:{manageritm_port}')
+   mc = manageritm.client.ManagerITMProxyClient(f'http://{manageritm_addr}:{manageritm_port}')
    proxy_details = mc.client()
 
    print(f"proxy port: {proxy_details['port']}")
    print(f"proxy webport: {proxy_details['webport']}")
 
    # start a proxy server
-   mc.proxy_start()
+   mc.start()
 
    # set your application to use the proxy
    #  host: "localhost"
    #  port: f"{proxy_details['port']}"
 
    # do some work...
 
    # stop the proxy server
-   mc.proxy_stop()
+   mc.stop()
+   ```
+
+Or start a video client
+
+1. Create a custom configuration file named `flask_config_video.py`
+  ```bash
+  MANAGERITM_CLIENT_COMMAND = ['/opt/bin/video.sh']
+  ```
+
+2. Start manageritm server on port 8000.
+   ```python
+   gunicorn --bind 0.0.0.0:8000 --workers 1 --log-level debug "manageritm.app:main()"
+   ```
+
+3. In Python, create a client, start the ffmpeg service, stop the ffmpeg service
+   ```python
+
+   import manageritm
+
+   manageritm_addr = "localhost"
+   manageritm_port = "8000"
+
+   # create a manageritm client
+   mc = manageritm.client.ManagerITMCommandClient(f'http://{manageritm_addr}:{manageritm_port}')
+   client_details = mc.client(additional_env={
+       'DISPLAY_CONTAINER_NAME': 'hanet_chrome_1',
+       'DISPLAY_NUM': '99',
+       'SE_VIDEO_FOLDER': '/videos',
+       'FILE_NAME': 'blahh.mp4'
+   })
+
+   # start a proxy server
+   mc.start()
+
+   # recording should happening
+   # ...
+
+   # stop the proxy server
+   mc.stop()
    ```
 
 ## Local Development
 
 1. Check out this repository
 2. Create a virtual environment
    ```bash
@@ -60,32 +99,31 @@
 
    import manageritm
 
    manageritm_addr = "localhost"
    manageritm_port = "8000"
 
    # create a manageritm client
-   mc = manageritm.client.ManagerITMClient(f'http://{manageritm_addr}:{manageritm_port}')
+   mc = manageritm.client.ManagerITMProxyClient(f'http://{manageritm_addr}:{manageritm_port}')
    proxy_details = mc.client()
 
    print(f"proxy port: {proxy_details['port']}")
    print(f"proxy webport: {proxy_details['webport']}")
 
    # start a proxy server
-   mc.proxy_start()
+   mc.start()
    ```
 6. Navigate a web browser to `http://localhost:<proxy webport>` to watch the traffic
 7. Configure a web browser to use the proxy port.
 8. Stop the client
    ```python
    # stop the proxy server
-   mc.proxy_stop()
+   mc.stop()
    ```
 
-
 ### Helpful Commands
 
 To build a package for the development version:
 ```python
 make all
 ```
```

### Comparing `manageritm-0.1.0/manageritm/app.py` & `manageritm-0.3.0/manageritm/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,17 +14,21 @@
         type=str,
     )
 
     opts, unknowns = parser.parse_known_args()
     return opts,unknowns
 
 
-def main():
+def main(config=None):
     opts, unknowns = parse_arguments()
-    app = create_app(opts.config)
+
+    if config is None:
+        config = opts.config
+
+    app = create_app(config)
 
     # share flask app logs with gunicorn
     # set the flask app log level to the same as gunicorn
     gunicorn_logger = logging.getLogger('gunicorn.error')
     app.logger.handlers = gunicorn_logger.handlers
     app.logger.setLevel(gunicorn_logger.level)
```

### Comparing `manageritm-0.1.0/manageritm/server/__init__.py` & `manageritm-0.3.0/manageritm/server/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from flask import Flask
-
+from flask import Flask, Blueprint
 
 def create_app(test_config=None):
     # create and configure the app
     app = Flask(__name__, instance_relative_config=True)
     app.config.from_mapping(
         SECRET_KEY='dev',
     )
@@ -11,11 +10,15 @@
     if test_config is None:
         # load the instance config, if it exists, when not testing
         app.config.from_pyfile('flask_config_production.py', silent=True)
     else:
         # load the test config if passed in
         app.config.from_pyfile(test_config)
 
-    from . import routes
-    app.register_blueprint(routes.bp)
+    # register blueprints
+    from manageritm.server.main import bp as main_bp
+    app.register_blueprint(main_bp)
+
+    from manageritm.server.client import bp as client_bp
+    app.register_blueprint(client_bp, url_prefix='/client')
 
     return app
```

### Comparing `manageritm-0.1.0/manageritm/server/scripts/har_dump.py` & `manageritm-0.3.0/manageritm/server/scripts/har_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         "log": {
             "version": "1.2",
             "creator": {
                 "name": "mitmproxy har_dump",
                 "version": "0.1",
                 "comment": "mitmproxy version %s" % version.MITMPROXY
             },
+            "pages": [{"pageTimings": {}}],
             "entries": []
         }
     })
 
 
 def response(flow: mitmproxy.http.HTTPFlow):
     """
```

### Comparing `manageritm-0.1.0/pyproject.toml` & `manageritm-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "manageritm"
-version = "0.1.0"
+version = "0.3.0"
 description = "Manage processes via an HTTP based API"
 authors = ["dskard"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://github.com/dskard/manageritm"
 repository = "http://github.com/dskard/manageritm"
 packages = [
     {include = "manageritm"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.27.1"
-requests-mock = "^1.9.3"
-pytest-mock = "^3.7.0"
-mitmproxy = "^8.0.0"
-Flask = "*"
+urllib3 = "^1.26.16"
+mitmproxy = "^9.0.1"
+flask = "^2.2.5"
+jsonschema = "^4.18.6"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 pytest = "^7.1.1"
 pdbpp = "^0.10.3"
 gunicorn = "^20.1.0"
+requests-mock = "^1.9.3"
+pytest-mock = "^3.7.0"
+deepdiff = "^6.3.1"
 
 [tool.poetry.scripts]
 manageritm = "manageritm.app:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `manageritm-0.1.0/PKG-INFO` & `manageritm-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: manageritm
-Version: 0.1.0
+Version: 0.3.0
 Summary: Manage processes via an HTTP based API
 Home-page: http://github.com/dskard/manageritm
 License: MIT
 Author: dskard
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Flask
-Requires-Dist: mitmproxy (>=8.0.0,<9.0.0)
-Requires-Dist: pytest-mock (>=3.7.0,<4.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: flask (>=2.2.5,<3.0.0)
+Requires-Dist: jsonschema (>=4.18.6,<5.0.0)
+Requires-Dist: mitmproxy (>=9.0.1,<10.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: requests-mock (>=1.9.3,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, http://github.com/dskard/manageritm
 Description-Content-Type: text/markdown
 
 # manageritm
 
 Manage a mitmproxy service on another system over a RESTful API
 
@@ -37,31 +38,70 @@
 
    import manageritm
 
    manageritm_addr = "localhost"
    manageritm_port = "8000"
 
    # create a manageritm client
-   mc = manageritm.client.ManagerITMClient(f'http://{manageritm_addr}:{manageritm_port}')
+   mc = manageritm.client.ManagerITMProxyClient(f'http://{manageritm_addr}:{manageritm_port}')
    proxy_details = mc.client()
 
    print(f"proxy port: {proxy_details['port']}")
    print(f"proxy webport: {proxy_details['webport']}")
 
    # start a proxy server
-   mc.proxy_start()
+   mc.start()
 
    # set your application to use the proxy
    #  host: "localhost"
    #  port: f"{proxy_details['port']}"
 
    # do some work...
 
    # stop the proxy server
-   mc.proxy_stop()
+   mc.stop()
+   ```
+
+Or start a video client
+
+1. Create a custom configuration file named `flask_config_video.py`
+  ```bash
+  MANAGERITM_CLIENT_COMMAND = ['/opt/bin/video.sh']
+  ```
+
+2. Start manageritm server on port 8000.
+   ```python
+   gunicorn --bind 0.0.0.0:8000 --workers 1 --log-level debug "manageritm.app:main()"
+   ```
+
+3. In Python, create a client, start the ffmpeg service, stop the ffmpeg service
+   ```python
+
+   import manageritm
+
+   manageritm_addr = "localhost"
+   manageritm_port = "8000"
+
+   # create a manageritm client
+   mc = manageritm.client.ManagerITMCommandClient(f'http://{manageritm_addr}:{manageritm_port}')
+   client_details = mc.client(additional_env={
+       'DISPLAY_CONTAINER_NAME': 'hanet_chrome_1',
+       'DISPLAY_NUM': '99',
+       'SE_VIDEO_FOLDER': '/videos',
+       'FILE_NAME': 'blahh.mp4'
+   })
+
+   # start a proxy server
+   mc.start()
+
+   # recording should happening
+   # ...
+
+   # stop the proxy server
+   mc.stop()
    ```
 
 ## Local Development
 
 1. Check out this repository
 2. Create a virtual environment
    ```bash
@@ -80,32 +120,31 @@
 
    import manageritm
 
    manageritm_addr = "localhost"
    manageritm_port = "8000"
 
    # create a manageritm client
-   mc = manageritm.client.ManagerITMClient(f'http://{manageritm_addr}:{manageritm_port}')
+   mc = manageritm.client.ManagerITMProxyClient(f'http://{manageritm_addr}:{manageritm_port}')
    proxy_details = mc.client()
 
    print(f"proxy port: {proxy_details['port']}")
    print(f"proxy webport: {proxy_details['webport']}")
 
    # start a proxy server
-   mc.proxy_start()
+   mc.start()
    ```
 6. Navigate a web browser to `http://localhost:<proxy webport>` to watch the traffic
 7. Configure a web browser to use the proxy port.
 8. Stop the client
    ```python
    # stop the proxy server
-   mc.proxy_stop()
+   mc.stop()
    ```
 
-
 ### Helpful Commands
 
 To build a package for the development version:
 ```python
 make all
 ```
```

