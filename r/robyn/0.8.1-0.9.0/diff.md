# Comparing `tmp/robyn-0.8.1.tar.gz` & `tmp/robyn-0.9.0.tar.gz`

## Comparing `robyn-0.8.1.tar` & `robyn-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 robyn-0.8.1/Cargo.toml
--rw-r--r--   0      501       20      224 2021-11-17 23:11:35.000000 robyn-0.8.1/.cargo/config
--rw-r--r--   0      501       20     6208 2021-11-17 23:11:35.000000 robyn-0.8.1/.circleci/config.yml
--rw-r--r--   0      501       20     5480 2021-11-17 23:11:35.000000 robyn-0.8.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20      130 2021-11-17 23:11:35.000000 robyn-0.8.1/.gitignore
--rw-r--r--   0      501       20     9388 2021-11-17 23:11:35.000000 robyn-0.8.1/CHANGELOG.md
--rw-r--r--   0      501       20     1323 2021-11-17 23:11:35.000000 robyn-0.8.1/LICENSE
--rw-r--r--   0      501       20     2107 2021-11-17 23:11:35.000000 robyn-0.8.1/README.md
--rw-r--r--   0      501       20        0 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/.nojekyll
--rw-r--r--   0      501       20     1070 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/README.md
--rw-r--r--   0      501       20      174 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/_sidebar.md
--rw-r--r--   0      501       20     3068 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/api.md
--rw-r--r--   0      501       20      373 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/architecture.md
--rw-r--r--   0      501       20     6025 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/comparison.md
--rw-r--r--   0      501       20     2383 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/index.html
--rw-r--r--   0      501       20   124245 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/landing_page/css/bootstrap.css
--rw-r--r--   0      501       20    96572 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/landing_page/css/bootstrap.min.css
--rw-r--r--   0      501       20     9415 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/landing_page/index.html
--rw-r--r--   0      501       20       68 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/landing_page/js/scripts.js
--rw-r--r--   0      501       20     5109 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/landing_page/scss/_custom.scss
--rw-r--r--   0      501       20    23975 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/landing_page/scss/_variables.scss
--rw-r--r--   0      501       20      141 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/plugins.md
--rw-r--r--   0      501       20      143 2021-11-17 23:11:35.000000 robyn-0.8.1/docs/roadmap.md
--rw-r--r--   0      501       20     2233 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/base_routes.py
--rw-r--r--   0      501       20      711 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/conftest.py
--rw-r--r--   0      501       20      243 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/index.html
--rw-r--r--   0      501       20      328 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_base_url.py
--rw-r--r--   0      501       20      410 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_delete_requests.py
--rw-r--r--   0      501       20      230 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_dir/build/index.html
--rw-r--r--   0      501       20      420 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_get_requests.py
--rw-r--r--   0      501       20      402 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_patch_requests.py
--rw-r--r--   0      501       20      560 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_post_requests.py
--rw-r--r--   0      501       20      389 2021-11-17 23:11:35.000000 robyn-0.8.1/integration_tests/test_put_requests.py
--rw-r--r--   0      501       20      591 2021-11-17 23:11:35.000000 robyn-0.8.1/pyproject.toml
--rw-r--r--   0      501       20       79 2021-11-17 23:11:35.000000 robyn-0.8.1/requirements.txt
--rw-r--r--   0      501       20     5854 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/__init__.py
--rw-r--r--   0      501       20      885 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/argument_parser.py
--rw-r--r--   0      501       20     1137 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/dev_event_handler.py
--rw-r--r--   0      501       20      226 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/log_colors.py
--rw-r--r--   0      501       20     2098 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/processpool.py
--rw-r--r--   0      501       20      465 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/responses.py
--rw-r--r--   0      501       20       87 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/test-requirements.txt
--rw-r--r--   0      501       20      223 2021-11-17 23:11:35.000000 robyn-0.8.1/robyn/test_robyn.py
--rw-r--r--   0      501       20      416 2021-11-17 23:11:35.000000 robyn-0.8.1/src/lib.rs
--rw-r--r--   0      501       20     7190 2021-11-17 23:11:35.000000 robyn-0.8.1/src/processor.rs
--rw-r--r--   0      501       20     3739 2021-11-17 23:11:35.000000 robyn-0.8.1/src/router.rs
--rw-r--r--   0      501       20     6970 2021-11-17 23:11:35.000000 robyn-0.8.1/src/server.rs
--rw-r--r--   0      501       20      892 2021-11-17 23:11:35.000000 robyn-0.8.1/src/shared_socket.rs
--rw-r--r--   0      501       20      193 2021-11-17 23:11:35.000000 robyn-0.8.1/src/types.rs
--rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 robyn-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 robyn-0.9.0/Cargo.toml
+-rw-r--r--   0      501       20      224 2021-12-02 00:18:54.000000 robyn-0.9.0/.cargo/config
+-rw-r--r--   0      501       20     6208 2021-12-02 00:18:54.000000 robyn-0.9.0/.circleci/config.yml
+-rw-r--r--   0      501       20     5480 2021-12-02 00:18:54.000000 robyn-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      130 2021-12-02 00:18:54.000000 robyn-0.9.0/.gitignore
+-rw-r--r--   0      501       20     9388 2021-12-02 00:18:54.000000 robyn-0.9.0/CHANGELOG.md
+-rw-r--r--   0      501       20     1323 2021-12-02 00:18:54.000000 robyn-0.9.0/LICENSE
+-rw-r--r--   0      501       20     2107 2021-12-02 00:18:54.000000 robyn-0.9.0/README.md
+-rw-r--r--   0      501       20        0 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/.nojekyll
+-rw-r--r--   0      501       20     1070 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/README.md
+-rw-r--r--   0      501       20      174 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/_sidebar.md
+-rw-r--r--   0      501       20     4314 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/api.md
+-rw-r--r--   0      501       20      373 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/architecture.md
+-rw-r--r--   0      501       20     6025 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/comparison.md
+-rw-r--r--   0      501       20     2383 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/index.html
+-rw-r--r--   0      501       20   124245 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/landing_page/css/bootstrap.css
+-rw-r--r--   0      501       20    96572 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/landing_page/css/bootstrap.min.css
+-rw-r--r--   0      501       20     9415 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/landing_page/index.html
+-rw-r--r--   0      501       20       68 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/landing_page/js/scripts.js
+-rw-r--r--   0      501       20     5109 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/landing_page/scss/_custom.scss
+-rw-r--r--   0      501       20    23975 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/landing_page/scss/_variables.scss
+-rw-r--r--   0      501       20      141 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/plugins.md
+-rw-r--r--   0      501       20      103 2021-12-02 00:18:54.000000 robyn-0.9.0/docs/roadmap.md
+-rw-r--r--   0      501       20     2560 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/base_routes.py
+-rw-r--r--   0      501       20      818 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/conftest.py
+-rw-r--r--   0      501       20      243 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/index.html
+-rw-r--r--   0      501       20      328 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_base_url.py
+-rw-r--r--   0      501       20      410 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_delete_requests.py
+-rw-r--r--   0      501       20      230 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_dir/build/index.html
+-rw-r--r--   0      501       20      420 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_get_requests.py
+-rw-r--r--   0      501       20      402 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_patch_requests.py
+-rw-r--r--   0      501       20      560 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_post_requests.py
+-rw-r--r--   0      501       20      389 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_put_requests.py
+-rw-r--r--   0      501       20      577 2021-12-02 00:18:54.000000 robyn-0.9.0/integration_tests/test_web_sockets.py
+-rw-r--r--   0      501       20      591 2021-12-02 00:18:54.000000 robyn-0.9.0/pyproject.toml
+-rw-r--r--   0      501       20       79 2021-12-02 00:18:54.000000 robyn-0.9.0/requirements.txt
+-rw-r--r--   0      501       20     6017 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/__init__.py
+-rw-r--r--   0      501       20      885 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/argument_parser.py
+-rw-r--r--   0      501       20     1137 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/dev_event_handler.py
+-rw-r--r--   0      501       20      226 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/log_colors.py
+-rw-r--r--   0      501       20     2360 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/processpool.py
+-rw-r--r--   0      501       20      465 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/responses.py
+-rw-r--r--   0      501       20      121 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/test-requirements.txt
+-rw-r--r--   0      501       20      223 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/test_robyn.py
+-rw-r--r--   0      501       20      870 2021-12-02 00:18:54.000000 robyn-0.9.0/robyn/ws.py
+-rw-r--r--   0      501       20      443 2021-12-02 00:18:54.000000 robyn-0.9.0/src/lib.rs
+-rw-r--r--   0      501       20     7216 2021-12-02 00:18:54.000000 robyn-0.9.0/src/processor.rs
+-rw-r--r--   0      501       20     6236 2021-12-02 00:18:54.000000 robyn-0.9.0/src/router.rs
+-rw-r--r--   0      501       20     8387 2021-12-02 00:18:54.000000 robyn-0.9.0/src/server.rs
+-rw-r--r--   0      501       20      892 2021-12-02 00:18:54.000000 robyn-0.9.0/src/shared_socket.rs
+-rw-r--r--   0      501       20      193 2021-12-02 00:18:54.000000 robyn-0.9.0/src/types.rs
+-rw-r--r--   0      501       20     4411 2021-12-02 00:18:54.000000 robyn-0.9.0/src/web_socket_connection.rs
+-rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 robyn-0.9.0/PKG-INFO
```

### Comparing `robyn-0.8.1/Cargo.toml` & `robyn-0.9.0/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "robyn"
-version = "0.8.1"
+version = "0.9.0"
 authors = ["Sanskar Jethi <sansyrox@gmail.com>"]
 edition = "2018"
 description = "A web server that is fast!"
 license = "MIT"
 homepage = "https://github.com/sansyrox/robyn"
 readme = "README.md"
 
@@ -24,10 +24,12 @@
 anyhow = "1.0.38"
 actix-web = "4.0.0-beta.8"
 actix-files = "0.6.0-beta.4"
 futures-util = "0.3.15"
 matchit = "0.4.3"
 actix-http = "3.0.0-beta.8"
 socket2 = { version = "0.4.1", features = ["all"] }
+actix = "0.12.0"
+actix-web-actors = "4.0.0-beta.1"
 
 [package.metadata.maturin]
 name = "robyn"
```

### Comparing `robyn-0.8.1/.circleci/config.yml` & `robyn-0.9.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/.github/workflows/CI.yml` & `robyn-0.9.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/CHANGELOG.md` & `robyn-0.9.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/LICENSE` & `robyn-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/README.md` & `robyn-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/README.md` & `robyn-0.9.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/api.md` & `robyn-0.9.0/docs/api.md`

 * *Files 23% similar despite different names*

```diff
@@ -86,16 +86,25 @@
     ```python3
     @app.delete("/delete")
     async def postreq(request):
         return bytearray(request["body"]).decode("utf-8")
     ```
 
 
+### Having Dynamic Routes
+You can now add params in the routes and access them from the request object.
 
-## Returning a JSON Response
+```python3
+@app.post("/jsonify/:id")
+async def json(request):
+    print(request["params"]["id"])
+    return jsonify({"hello": "world"})
+```
+
+### Returning a JSON Response
 You can also serve JSON responses when serving HTTP request using the following way.
 
 ```python3
 from robyn import jsonify
 
 @app.post("/jsonify")
 async def json(request):
@@ -135,8 +144,57 @@
 You can also add global headers for every request.
 
 ```python3
 app.add_header("server", "robyn")
 
 ```
 
-To see a complete service in action, you can go to the folder [../test_python/test.py](../test_python/test.py)
+## WebSockets
+
+You can now serve websockets using Robyn.
+
+Firstly, you need to create a WebSocket Class and wrap it around your Robyn app.
+
+```python3
+from robyn import Robyn, static_file, jsonify, WS
+
+
+app = Robyn(__file__)
+websocket = WS(app, "/web_socket")
+```
+
+Now, you can define 3 methods for every web_socket for their lifecycle, they are as follows:
+
+```python3
+@websocket.on("message")
+def connect():
+    global i
+    i+=1
+    if i==0:
+        return "Whaaat??"
+    elif i==1:
+        return "Whooo??"
+    elif i==2:
+        return "*chika* *chika* Slim Shady."
+    elif i==3:
+        i= -1
+        return ""
+
+@websocket.on("close")
+def close():
+    return "Goodbye world, from ws"
+
+@websocket.on("connect")
+def message():
+    return "Hello world, from ws"
+
+```
+
+
+## MutliCore Scaling
+
+The three methods:
+ - "message" is called when the socket receives a message
+ - "close" is called when the socket is disconnected
+ - "connect" is called when the socket connects
+
+To see a complete service in action, you can go to the folder [../integration_tests/base_routes.py](../integration_tests/base_routes.py)
```

### Comparing `robyn-0.8.1/docs/comparison.md` & `robyn-0.9.0/docs/comparison.md`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/index.html` & `robyn-0.9.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/landing_page/css/bootstrap.css` & `robyn-0.9.0/docs/landing_page/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/landing_page/css/bootstrap.min.css` & `robyn-0.9.0/docs/landing_page/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/landing_page/index.html` & `robyn-0.9.0/docs/landing_page/index.html`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/landing_page/scss/_custom.scss` & `robyn-0.9.0/docs/landing_page/scss/_custom.scss`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/docs/landing_page/scss/_variables.scss` & `robyn-0.9.0/docs/landing_page/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/integration_tests/base_routes.py` & `robyn-0.9.0/integration_tests/base_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,37 @@
-
-
-# robyn_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../robyn")
-# sys.path.insert(0, robyn_path)
-
-from robyn import Robyn, static_file, jsonify, SocketHeld
+from robyn import Robyn, static_file, jsonify, WS
 import asyncio
 import os
 import pathlib
 
 app = Robyn(__file__)
+websocket = WS(app, "/web_socket")
+i = -1
+
+@websocket.on("message")
+def connect():
+    global i
+    i+=1
+    if i==0:
+        return "Whaaat??"
+    elif i==1:
+        return "Whooo??"
+    elif i==2:
+        i = -1
+        return "*chika* *chika* Slim Shady."
+
+@websocket.on("close")
+def close():
+    print("Hello world")
+    return "Hello world, from ws"
+
+@websocket.on("connect")
+def message():
+    print("Hello world")
+    return "Hello world, from ws"
 
 
 callCount = 0
 
 
 @app.get("/")
 async def hello(request):
```

### Comparing `robyn-0.8.1/integration_tests/conftest.py` & `robyn-0.9.0/integration_tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 import pathlib
 import os
 import time
 
 
 @pytest.fixture
 def session():
+    subprocess.call(["freeport", "5000"])
     os.environ["ROBYN_URL"] = "127.0.0.1"
     current_file_path = pathlib.Path(__file__).parent.resolve()
     base_routes = os.path.join(current_file_path, "./base_routes.py")
     process = subprocess.Popen(["python3", base_routes])
     time.sleep(1)
     yield
     process.terminate()
+    del os.environ["ROBYN_URL"]
 
 @pytest.fixture
 def global_session():
     os.environ["ROBYN_URL"] = "0.0.0.0"
     current_file_path = pathlib.Path(__file__).parent.resolve()
     base_routes = os.path.join(current_file_path, "./base_routes.py")
     process = subprocess.Popen(["python3", base_routes])
     time.sleep(1)
     yield
     process.terminate()
+    del os.environ["ROBYN_URL"]
+
```

### Comparing `robyn-0.8.1/integration_tests/test_post_requests.py` & `robyn-0.9.0/integration_tests/test_post_requests.py`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/pyproject.toml` & `robyn-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robyn"
-version = "0.8.1"
+version = "0.9.0"
 description = "A web server that is fast!"
 authors = ["Sanskar Jethi <sansyrox@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 watchdog = "^2.1.3"
```

### Comparing `robyn-0.8.1/robyn/__init__.py` & `robyn-0.9.0/robyn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # custom imports and exports
 from .robyn import Server, SocketHeld
 from .argument_parser import ArgumentParser
 from .responses import static_file, jsonify
 from .dev_event_handler import EventHandler
 from .processpool import spawn_process
 from .log_colors import Colors
+from .ws import WS
 
 
 # 3rd party imports and exports
 from multiprocess import Process
 from watchdog.observers import Observer
 
 
@@ -32,14 +33,15 @@
         self.dev = self.parser.is_dev()
         self.processes = self.parser.num_processes() 
         self.workers = self.parser.workers()
         self.routes = []
         self.headers = []
         self.routes = []
         self.directories = []
+        self.web_sockets = {}
 
 
     def add_route(self, route_type, endpoint, handler):
         """
         [This is base handler for all the decorators]
 
         :param route_type [str]: [route type between GET/POST/PUT/DELETE/PATCH]
@@ -58,29 +60,33 @@
         self.directories.append(( route, directory_path, index_file, show_files_listing ))
 
     def add_header(self, key, value):
         self.headers.append(( key, value ))
 
     def remove_header(self, key):
         self.server.remove_header(key)
+
+    def add_web_socket(self, endpoint, ws):
+        self.web_sockets[endpoint] = ws
+        
     
     def start(self, url="127.0.0.1", port=5000):
         """
         [Starts the server]
 
         :param port [int]: [reperesents the port number at which the server is listening]
         """
         socket = SocketHeld(url, port)
         workers = self.workers
         if not self.dev:
             for process_number in range(self.processes):
                 copied = socket.try_clone()
                 p = Process(
                     target=spawn_process,
-                    args=(url, port, self.directories, self.headers, self.routes, copied, f"Process {process_number}", workers),
+                    args=(url, port, self.directories, self.headers, self.routes, self.web_sockets, copied, f"Process {process_number}", workers),
                 )
                 p.start()
 
             input("Press Cntrl + C to stop \n")
         else:
             event_handler = EventHandler(self.file_path)
             event_handler.start_server_first_time()
@@ -91,14 +97,15 @@
             try:
                 while True:
                     pass
             finally:
                 observer.stop()
                 observer.join()
 
+
     def get(self, endpoint):
         """
         [The @app.get decorator to add a get route]
 
         :param endpoint [str]: [endpoint to server the route]
         """
         def inner(handler):
@@ -191,7 +198,8 @@
         :param endpoint [str]: [endpoint to server the route]
         """
         def inner(handler):
             self.add_route("TRACE", endpoint, handler)
 
         return inner
 
+
```

### Comparing `robyn-0.8.1/robyn/argument_parser.py` & `robyn-0.9.0/robyn/argument_parser.py`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/robyn/dev_event_handler.py` & `robyn-0.9.0/robyn/dev_event_handler.py`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/robyn/processpool.py` & `robyn-0.9.0/robyn/processpool.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 # import platform
 
 
 mp.allow_connection_pickling()
 
 
-def spawn_process(url, port, directories, headers, routes, socket, process_name, workers):
+def spawn_process(url, port, directories, headers, routes, web_sockets, socket, process_name, workers):
     """
     This function is called by the main process handler to create a server runtime.
     This functions allows one runtime per process.
 
     :param url string: the base url at which the server will listen
     :param port string: the port at which the url will listen to
     :param directories tuple: the list of all the directories and related data in a tuple
@@ -47,9 +47,15 @@
         server.add_header(key, val)
 
 
     for route in routes:
         route_type, endpoint, handler, is_async, number_of_params = route
         server.add_route(route_type, endpoint, handler, is_async, number_of_params)
 
+    for endpoint in web_sockets:
+        web_socket = web_sockets[endpoint]
+        print(web_socket.methods)
+        server.add_web_socket_route(endpoint, web_socket.methods["connect"], web_socket.methods["close"], web_socket.methods["message"])
+
+
     server.start(url, port, socket, process_name, workers)
     asyncio.get_event_loop().run_forever()
```

### Comparing `robyn-0.8.1/src/processor.rs` & `robyn-0.9.0/src/processor.rs`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     function: PyFunction,
     number_of_params: u8,
     headers: &Arc<Headers>,
     payload: &mut web::Payload,
     req: &HttpRequest,
     route_params: HashMap<String, String>,
 ) -> HttpResponse {
-    let contents = match execute_function(
+    let contents = match execute_http_function(
         function,
         payload,
         headers,
         req,
         route_params,
         number_of_params,
     )
@@ -75,16 +75,17 @@
 fn read_file(file_path: &str) -> String {
     let mut file = File::open(file_path).unwrap();
     let mut buf = vec![];
     file.read_to_end(&mut buf).unwrap();
     String::from_utf8_lossy(&buf).to_string()
 }
 
+// Change this!
 #[inline]
-async fn execute_function(
+async fn execute_http_function(
     function: PyFunction,
     payload: &mut web::Payload,
     headers: &Headers,
     req: &HttpRequest,
     route_params: HashMap<String, String>,
     number_of_params: u8,
 ) -> Result<String> {
```

### Comparing `robyn-0.8.1/src/server.rs` & `robyn-0.9.0/src/server.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 use crate::processor::{apply_headers, handle_request};
 use crate::router::Router;
 use crate::shared_socket::SocketHeld;
 use crate::types::Headers;
-use actix_files::Files;
+use crate::web_socket_connection::start_web_socket;
+
 use std::convert::TryInto;
 use std::sync::atomic::AtomicBool;
 use std::sync::atomic::Ordering::{Relaxed, SeqCst};
 use std::sync::{Arc, RwLock};
 use std::thread;
-// pyO3 module
+
+use actix_files::Files;
 use actix_http::KeepAlive;
 use actix_web::*;
 use dashmap::DashMap;
+
+// pyO3 module
 use pyo3::prelude::*;
-use pyo3::types::PyAny;
 
 static STARTED: AtomicBool = AtomicBool::new(false);
 
 #[derive(Clone)]
 struct Directory {
     route: String,
     directory_path: String,
@@ -80,22 +83,21 @@
             .call_method1("set_event_loop", (event_loop,))
             .unwrap();
         let event_loop_hdl = PyObject::from(event_loop);
 
         thread::spawn(move || {
             //init_current_thread_once();
             actix_web::rt::System::new().block_on(async move {
-                let addr = format!("{}:{}", url, port);
-
                 println!("The number of workers are {}", workers.clone());
 
                 HttpServer::new(move || {
                     let mut app = App::new();
                     let event_loop_hdl = event_loop_hdl.clone();
                     let directories = directories.read().unwrap();
+                    let router_copy = router.clone();
 
                     // this loop matches three types of directory serving
                     // 1. Serves a build folder. e.g. the build folder generated from yarn build
                     // 2. Shows file listing
                     // 3. Just serves the file without any redirection to sub links
                     for directory in directories.iter() {
                         if let Some(index_file) = &directory.index_file {
@@ -112,21 +114,40 @@
                             );
                         } else {
                             app = app
                                 .service(Files::new(&directory.route, &directory.directory_path));
                         }
                     }
 
-                    app.app_data(web::Data::new(router.clone()))
-                        .app_data(web::Data::new(headers.clone()))
-                        .default_service(web::route().to(move |router, headers, payload, req| {
-                            pyo3_asyncio::tokio::scope_local(event_loop_hdl.clone(), async move {
-                                index(router, headers, payload, req).await
-                            })
-                        }))
+                    app = app
+                        .app_data(web::Data::new(router.clone()))
+                        .app_data(web::Data::new(headers.clone()));
+
+                    let web_socket_map = router_copy.get_web_socket_map();
+                    for elem in (web_socket_map).iter() {
+                        let route = elem.key().clone();
+                        let params = elem.value().clone();
+                        app = app.route(
+                            &route,
+                            web::get().to(
+                                move |_router: web::Data<Arc<Router>>,
+                                      _headers: web::Data<Arc<Headers>>,
+                                      stream: web::Payload,
+                                      req: HttpRequest| {
+                                    start_web_socket(req, stream, Arc::new(params.clone()))
+                                },
+                            ),
+                        );
+                    }
+
+                    app.default_service(web::route().to(move |router, headers, payload, req| {
+                        pyo3_asyncio::tokio::scope_local(event_loop_hdl.clone(), async move {
+                            index(router, headers, payload, req).await
+                        })
+                    }))
                 })
                 .keep_alive(KeepAlive::Os)
                 .workers(*workers.clone())
                 .client_timeout(0)
                 .listen(raw_socket.try_into().unwrap())
                 .unwrap()
                 .run()
@@ -176,14 +197,29 @@
         is_async: bool,
         number_of_params: u8,
     ) {
         println!("Route added for {} {} ", route_type, route);
         self.router
             .add_route(route_type, route, handler, is_async, number_of_params);
     }
+
+    /// Add a new web socket route to the routing tables
+    /// can be called after the server has been started
+    pub fn add_web_socket_route(
+        &self,
+        route: &str,
+        // handler, is_async, number of params
+        connect_route: (Py<PyAny>, bool, u8),
+        close_route: (Py<PyAny>, bool, u8),
+        message_route: (Py<PyAny>, bool, u8),
+    ) {
+        println!("WS Route added for {} ", route);
+        self.router
+            .add_websocket_route(route, connect_route, close_route, message_route);
+    }
 }
 
 impl Default for Server {
     fn default() -> Self {
         Self::new()
     }
 }
```

### Comparing `robyn-0.8.1/src/shared_socket.rs` & `robyn-0.9.0/src/shared_socket.rs`

 * *Files identical despite different names*

### Comparing `robyn-0.8.1/PKG-INFO` & `robyn-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robyn
-Version: 0.8.1
+Version: 0.9.0
 Requires-Dist: watchdog == 2.1.3
 Requires-Dist: multiprocess == 0.70.12.2
 Requires-Dist: uvloop == 0.16.0; sys_platform == "darwin"
 Requires-Dist: uvloop == 0.16.0; platform_machine == "x86_64"
 Requires-Dist: uvloop == 0.16.0; platform_machine == "i686"
 Summary: A web server that is fast!
 Home-Page: https://github.com/sansyrox/robyn
```

