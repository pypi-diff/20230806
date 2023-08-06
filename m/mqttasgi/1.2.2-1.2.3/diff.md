# Comparing `tmp/mqttasgi-1.2.2.tar.gz` & `tmp/mqttasgi-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttasgi-1.2.2.tar", last modified: Sat May 20 11:07:36 2023, max compression
+gzip compressed data, was "mqttasgi-1.2.3.tar", last modified: Sun Aug  6 13:05:45 2023, max compression
```

## Comparing `mqttasgi-1.2.2.tar` & `mqttasgi-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-05-20 11:07:36.853866 mqttasgi-1.2.2/
--rw-r--r--   0 sivulich   (501) staff       (20)     1073 2021-12-26 14:23:26.000000 mqttasgi-1.2.2/LICENSE
--rw-r--r--   0 sivulich   (501) staff       (20)     7094 2023-05-20 11:07:36.853757 mqttasgi-1.2.2/PKG-INFO
--rw-r--r--   0 sivulich   (501) staff       (20)     6042 2023-05-20 11:05:45.000000 mqttasgi-1.2.2/README.md
-drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-05-20 11:07:36.852645 mqttasgi-1.2.2/mqttasgi/
--rw-r--r--   0 sivulich   (501) staff       (20)       22 2023-05-20 09:42:43.000000 mqttasgi-1.2.2/mqttasgi/__init__.py
--rw-r--r--   0 sivulich   (501) staff       (20)     2935 2023-05-20 09:42:11.000000 mqttasgi-1.2.2/mqttasgi/cli.py
--rw-r--r--   0 sivulich   (501) staff       (20)     3622 2022-07-29 22:42:10.000000 mqttasgi-1.2.2/mqttasgi/consumers.py
--rw-r--r--   0 sivulich   (501) staff       (20)    18315 2023-05-20 11:01:15.000000 mqttasgi-1.2.2/mqttasgi/server.py
--rw-r--r--   0 sivulich   (501) staff       (20)     1695 2021-06-04 18:10:17.000000 mqttasgi-1.2.2/mqttasgi/testing.py
--rw-r--r--   0 sivulich   (501) staff       (20)      402 2022-08-29 21:55:32.000000 mqttasgi-1.2.2/mqttasgi/utils.py
-drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-05-20 11:07:36.853595 mqttasgi-1.2.2/mqttasgi.egg-info/
--rw-r--r--   0 sivulich   (501) staff       (20)     7094 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/PKG-INFO
--rw-r--r--   0 sivulich   (501) staff       (20)      336 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/SOURCES.txt
--rw-r--r--   0 sivulich   (501) staff       (20)        1 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/dependency_links.txt
--rw-r--r--   0 sivulich   (501) staff       (20)       48 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/entry_points.txt
--rw-r--r--   0 sivulich   (501) staff       (20)       40 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/requires.txt
--rw-r--r--   0 sivulich   (501) staff       (20)        9 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/top_level.txt
--rw-r--r--   0 sivulich   (501) staff       (20)       38 2023-05-20 11:07:36.853907 mqttasgi-1.2.2/setup.cfg
--rw-r--r--   0 sivulich   (501) staff       (20)     1664 2022-08-29 21:56:42.000000 mqttasgi-1.2.2/setup.py
+drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-08-06 13:05:45.558707 mqttasgi-1.2.3/
+-rw-r--r--   0 sivulich   (501) staff       (20)     1073 2021-12-26 14:23:26.000000 mqttasgi-1.2.3/LICENSE
+-rw-r--r--   0 sivulich   (501) staff       (20)     7266 2023-08-06 13:05:45.558584 mqttasgi-1.2.3/PKG-INFO
+-rw-r--r--   0 sivulich   (501) staff       (20)     6214 2023-08-06 13:03:40.000000 mqttasgi-1.2.3/README.md
+drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-08-06 13:05:45.557551 mqttasgi-1.2.3/mqttasgi/
+-rw-r--r--   0 sivulich   (501) staff       (20)       22 2023-08-06 13:05:05.000000 mqttasgi-1.2.3/mqttasgi/__init__.py
+-rw-r--r--   0 sivulich   (501) staff       (20)     3567 2023-08-06 13:03:40.000000 mqttasgi-1.2.3/mqttasgi/cli.py
+-rw-r--r--   0 sivulich   (501) staff       (20)     3622 2022-07-29 22:42:10.000000 mqttasgi-1.2.3/mqttasgi/consumers.py
+-rw-r--r--   0 sivulich   (501) staff       (20)    18517 2023-08-06 13:03:40.000000 mqttasgi-1.2.3/mqttasgi/server.py
+-rw-r--r--   0 sivulich   (501) staff       (20)     1695 2021-06-04 18:10:17.000000 mqttasgi-1.2.3/mqttasgi/testing.py
+-rw-r--r--   0 sivulich   (501) staff       (20)      402 2022-08-29 21:55:32.000000 mqttasgi-1.2.3/mqttasgi/utils.py
+drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-08-06 13:05:45.558423 mqttasgi-1.2.3/mqttasgi.egg-info/
+-rw-r--r--   0 sivulich   (501) staff       (20)     7266 2023-08-06 13:05:45.000000 mqttasgi-1.2.3/mqttasgi.egg-info/PKG-INFO
+-rw-r--r--   0 sivulich   (501) staff       (20)      336 2023-08-06 13:05:45.000000 mqttasgi-1.2.3/mqttasgi.egg-info/SOURCES.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)        1 2023-08-06 13:05:45.000000 mqttasgi-1.2.3/mqttasgi.egg-info/dependency_links.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)       48 2023-08-06 13:05:45.000000 mqttasgi-1.2.3/mqttasgi.egg-info/entry_points.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)       40 2023-08-06 13:05:45.000000 mqttasgi-1.2.3/mqttasgi.egg-info/requires.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)        9 2023-08-06 13:05:45.000000 mqttasgi-1.2.3/mqttasgi.egg-info/top_level.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)       38 2023-08-06 13:05:45.558751 mqttasgi-1.2.3/setup.cfg
+-rw-r--r--   0 sivulich   (501) staff       (20)     1664 2022-08-29 21:56:42.000000 mqttasgi-1.2.3/setup.py
```

### Comparing `mqttasgi-1.2.2/LICENSE` & `mqttasgi-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttasgi-1.2.2/PKG-INFO` & `mqttasgi-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttasgi
-Version: 1.2.2
+Version: 1.2.3
 Summary: MQTT ASGI Protocol Server
 Home-page: https://github.com/sivulich/mqttasgi
 Author: Santiago Ivulich
 Author-email: sivulich@itba.edu.ar
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -60,14 +60,16 @@
 | -v / --verbosity | Logging verbosity | VERBOSITY | 0 |
 | -U / --username | MQTT Username | MQTT_USERNAME |  |
 | -P / --password | MQTT Password | MQTT_PASSWORD |  |
 | -i / --id | MQTT Client ID | MQTT_CLIENT_ID |  |
 | -C / --cert | TLS Certificate | TLS_CERT |  |
 | -K / --key | TLS Key | TLS_KEY |  |
 | -S / --cacert | TLS CA Certificate | TLS_CA |  |
+| -SSL / --use-ssl | Use ssl (without certificate authentication) | MQTT_USE_SSL | False |
+| -T / --transport | Transport type (tcp or websockets) | MQTT_TRANSPORT | tcp |
 | -r / --retries | Num. retries on disconnect | MQTT_RETRIES | 3 |
 | Last argument | ASGI Apllication |  | |
 
 Environment variables are supported and can be set using a `.env` file on the root of the project, but passing a parameter overrides this value.
 
 ## Consumer
```

### Comparing `mqttasgi-1.2.2/README.md` & `mqttasgi-1.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 | -v / --verbosity | Logging verbosity | VERBOSITY | 0 |
 | -U / --username | MQTT Username | MQTT_USERNAME |  |
 | -P / --password | MQTT Password | MQTT_PASSWORD |  |
 | -i / --id | MQTT Client ID | MQTT_CLIENT_ID |  |
 | -C / --cert | TLS Certificate | TLS_CERT |  |
 | -K / --key | TLS Key | TLS_KEY |  |
 | -S / --cacert | TLS CA Certificate | TLS_CA |  |
+| -SSL / --use-ssl | Use ssl (without certificate authentication) | MQTT_USE_SSL | False |
+| -T / --transport | Transport type (tcp or websockets) | MQTT_TRANSPORT | tcp |
 | -r / --retries | Num. retries on disconnect | MQTT_RETRIES | 3 |
 | Last argument | ASGI Apllication |  | |
 
 Environment variables are supported and can be set using a `.env` file on the root of the project, but passing a parameter overrides this value.
 
 ## Consumer
```

### Comparing `mqttasgi-1.2.2/mqttasgi/cli.py` & `mqttasgi-1.2.3/mqttasgi/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,30 @@
 from .utils import get_application
 from dotenv import load_dotenv
 
 load_dotenv()
 
 logger = logging.getLogger(__name__)
 
+def bool_type_converter(arg):
+    if arg.lower() == "true":
+        return True
+    elif arg.lower() == "false":
+        return False
+    raise ValueError()
+
+
 def main():
     parser = argparse.ArgumentParser(description="MQTT ASGI Protocol Server")
     parser.add_argument("-H", "--host", help="MQTT broker host",
                         default=os.environ.get("MQTT_HOSTNAME", "localhost"))
     parser.add_argument("-p", "--port", help="MQTT broker port", type=int,
                         default=int(os.environ.get("MQTT_PORT", 1883)))
-    parser.add_argument("-c", "--cleansession", help="MQTT Clean Session", type=bool,
-                        default=os.environ.get("MQTT_CLEAN", "True").lower() == "true")
+    parser.add_argument("-c", "--cleansession", help="MQTT Clean Session", type=bool_type_converter,
+                        default=bool_type_converter(os.environ.get("MQTT_CLEAN", "True")))
     parser.add_argument("-v", "--verbosity", type=int, help="Set verbosity",
                         default=int(os.environ.get("VERBOSITY", 0)))
     parser.add_argument("-U", "--username", help="MQTT username to authorised connection",
                         default=os.environ.get("MQTT_USERNAME", None))
     parser.add_argument("-P", "--password", help="MQTT password to authorised connection",
                         default=os.environ.get("MQTT_PASSWORD", None))
     parser.add_argument("-i", "--id", dest="client_id", help="MQTT Client ID",
@@ -28,14 +36,18 @@
     # add support for certificate authentication (TLS)
     parser.add_argument("-C", "--cert", help="MQTT TLS certificate",
                         default=os.environ.get("TLS_CERT", None))
     parser.add_argument("-K", "--key", help="MQTT TLS key",
                         default=os.environ.get("TLS_KEY", None))
     parser.add_argument("-S", "--cacert", help="MQTT TLS CA certificate",
                         default=os.environ.get("TLS_CA", None))
+    parser.add_argument("-SSL", "--use-ssl", dest="use_ssl", help="Use ssl with server signed certificate",
+                        type=bool_type_converter, default=bool_type_converter(os.environ.get("MQTT_USE_SSL", "False")))
+    parser.add_argument("-T", "--transport", help="Transport type (tcp or websockets)",
+                        default=os.environ.get("MQTT_TRANSPORT", "tcp"))
     parser.add_argument("-r", "--retries", help="Maximum number of connection retries after unexpected disconnect (0 to always try to reconnect)",
                         default=os.environ.get("MQTT_RETRIES", 3), type=int)
 
     parser.add_argument("application",
                         help=("The ASGI application instance to use as "
                               "path.to.module:application"))
 
@@ -59,14 +71,16 @@
         args.password,
         args.client_id,
         logger=logger,
         clean_session=args.cleansession,
         cert=args.cert,
         key=args.key,
         ca_cert=args.cacert,
-        connect_max_retries=args.retries
+        connect_max_retries=args.retries,
+        use_ssl=args.use_ssl,
+        transport = args.transport
     )
 
     server.run()
 
 if __name__ == '__main__':
     main()
```

### Comparing `mqttasgi-1.2.2/mqttasgi/consumers.py` & `mqttasgi-1.2.3/mqttasgi/consumers.py`

 * *Files identical despite different names*

### Comparing `mqttasgi-1.2.2/mqttasgi/server.py` & `mqttasgi-1.2.3/mqttasgi/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 _logger = logging.getLogger(__name__)
 
 
 class Server(object):
     def __init__(self, application, host, port, username=None, password=None,
                  client_id=2407, mqtt_type_pub=None, mqtt_type_usub=None, mqtt_type_sub=None,
-                 mqtt_type_msg=None, connect_max_retries=3, logger=None, clean_session=True, cert=None, key=None, ca_cert=None):
+                 mqtt_type_msg=None, connect_max_retries=3, logger=None, clean_session=True, cert=None, key=None, ca_cert=None,
+                 use_ssl=False, transport ="tcp"):
 
         self.application_type = application
         self.application_data = {}
         self.base_scope = {
             'type': 'mqtt',
             'version': '2.4',
             'spec_version': '0.1'
@@ -28,27 +29,29 @@
             self.log = _logger
         else:
             self.log = logger
 
         self.host = host
         self.port = port
         self.client_id = client_id
-        self.client = mqtt.Client(client_id=self.client_id, userdata={
+        self.transport = transport
+        self.client = mqtt.Client(client_id=self.client_id, transport=self.transport, userdata={
             "server": self,
             "host": self.host,
             "port": self.port,
         }, clean_session=clean_session)
 
         self.client.enable_logger(self.log)
         self.username = username
         self.password = password
         # certificates
         self.cert = cert
         self.key = key
         self.ca_cert = ca_cert
+        self.use_ssl = use_ssl
         self.client.on_connect = self._on_connect
         self.client.on_disconnect = self._on_disconnect
         self.connect_max_retries = connect_max_retries
         self.client.on_message = lambda client, userdata, message: \
             self._mqtt_receive(-1, message.topic, message.payload, message.qos)
 
         self.topics_subscription = {}
@@ -145,15 +148,16 @@
 
         if all([self.cert, self.key, self.ca_cert]):
             self.client.tls_set(
                 ca_certs=self.ca_cert,
                 certfile=self.cert,
                 keyfile=self.key,
             )
-
+        elif self.use_ssl:
+            self.client.tls_set()
         try:
             self.client.connect(self.host, self.port)
         except Exception as e:
             try:
                 self._handle_reconnect(on_connect=True)
             except Exception as e:
                 await self.shutdown('CONNECTION_ERROR')
```

### Comparing `mqttasgi-1.2.2/mqttasgi/testing.py` & `mqttasgi-1.2.3/mqttasgi/testing.py`

 * *Files identical despite different names*

### Comparing `mqttasgi-1.2.2/mqttasgi.egg-info/PKG-INFO` & `mqttasgi-1.2.3/mqttasgi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttasgi
-Version: 1.2.2
+Version: 1.2.3
 Summary: MQTT ASGI Protocol Server
 Home-page: https://github.com/sivulich/mqttasgi
 Author: Santiago Ivulich
 Author-email: sivulich@itba.edu.ar
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -60,14 +60,16 @@
 | -v / --verbosity | Logging verbosity | VERBOSITY | 0 |
 | -U / --username | MQTT Username | MQTT_USERNAME |  |
 | -P / --password | MQTT Password | MQTT_PASSWORD |  |
 | -i / --id | MQTT Client ID | MQTT_CLIENT_ID |  |
 | -C / --cert | TLS Certificate | TLS_CERT |  |
 | -K / --key | TLS Key | TLS_KEY |  |
 | -S / --cacert | TLS CA Certificate | TLS_CA |  |
+| -SSL / --use-ssl | Use ssl (without certificate authentication) | MQTT_USE_SSL | False |
+| -T / --transport | Transport type (tcp or websockets) | MQTT_TRANSPORT | tcp |
 | -r / --retries | Num. retries on disconnect | MQTT_RETRIES | 3 |
 | Last argument | ASGI Apllication |  | |
 
 Environment variables are supported and can be set using a `.env` file on the root of the project, but passing a parameter overrides this value.
 
 ## Consumer
```

### Comparing `mqttasgi-1.2.2/setup.py` & `mqttasgi-1.2.3/setup.py`

 * *Files identical despite different names*

