# Comparing `tmp/nonebot_plugin_kanonbot-0.0.1b1.tar.gz` & `tmp/nonebot_plugin_kanonbot-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kanonbot-0.0.1b1.tar", last modified: Sat Aug  5 09:16:54 2023, max compression
+gzip compressed data, was "nonebot_plugin_kanonbot-0.0.1b2.tar", last modified: Sat Aug  5 18:33:40 2023, max compression
```

## Comparing `nonebot_plugin_kanonbot-0.0.1b1.tar` & `nonebot_plugin_kanonbot-0.0.1b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 09:16:54.623489 nonebot_plugin_kanonbot-0.0.1b1/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_kanonbot-0.0.1b1/LICENSE
--rw-rw-rw-   0        0        0      276 2023-08-05 09:16:54.622489 nonebot_plugin_kanonbot-0.0.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     2448 2023-08-05 08:32:00.000000 nonebot_plugin_kanonbot-0.0.1b1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 09:16:54.612487 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/
--rw-rw-rw-   0        0        0    10370 2023-08-05 05:14:26.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/__init__.py
--rw-rw-rw-   0        0        0     7757 2023-08-05 09:13:37.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/bot_run.py
--rw-rw-rw-   0        0        0     8483 2023-08-05 07:48:39.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/config.py
--rw-rw-rw-   0        0        0     2550 2023-08-05 09:11:43.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/plugins.py
--rw-rw-rw-   0        0        0    10734 2023-08-05 05:14:26.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/tools.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:16:54.620489 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/
--rw-rw-rw-   0        0        0      276 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 09:16:54.623489 nonebot_plugin_kanonbot-0.0.1b1/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-08-05 09:16:52.000000 nonebot_plugin_kanonbot-0.0.1b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:33:40.270607 nonebot_plugin_kanonbot-0.0.1b2/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_kanonbot-0.0.1b2/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-08-05 18:33:40.269605 nonebot_plugin_kanonbot-0.0.1b2/PKG-INFO
+-rw-rw-rw-   0        0        0     2448 2023-08-05 08:32:00.000000 nonebot_plugin_kanonbot-0.0.1b2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 18:33:40.260607 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/
+-rw-rw-rw-   0        0        0    10813 2023-08-05 17:24:03.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/__init__.py
+-rw-rw-rw-   0        0        0     8448 2023-08-05 17:55:20.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/bot_run.py
+-rw-rw-rw-   0        0        0    10122 2023-08-05 17:56:52.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/config.py
+-rw-rw-rw-   0        0        0     2765 2023-08-05 18:30:41.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/plugins.py
+-rw-rw-rw-   0        0        0    10732 2023-08-05 18:23:03.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:33:40.268606 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-08-05 18:33:40.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-05 18:33:40.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:33:40.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-08-05 18:33:40.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-05 18:33:40.000000 nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:33:40.270607 nonebot_plugin_kanonbot-0.0.1b2/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-08-05 18:33:37.000000 nonebot_plugin_kanonbot-0.0.1b2/setup.py
```

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/LICENSE` & `nonebot_plugin_kanonbot-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/README.md` & `nonebot_plugin_kanonbot-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/__init__.py` & `nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -138,34 +138,42 @@
 
     # 判断是否响应
     commandname = ""
     commandlist = command_list()
     run = False
     if not run:
         cache_commandlist = commandlist["精准"]
-        if command in cache_commandlist:
+        if command in list(cache_commandlist):
+            commandname = cache_commandlist[command]
             run = True
     if not run:
         cache_commandlist = commandlist["模糊"]
-        for cache_command in cache_commandlist:
+        for cache_command in list(cache_commandlist):
             if cache_command in command:
+                commandname = cache_commandlist[command]
                 run = True
+                break
     if not run:
         cache_commandlist = commandlist["开头"]
-        for cache_command in cache_commandlist:
+        for cache_command in list(cache_commandlist):
             if command.startswith(cache_command):
+                commandname = cache_commandlist[cache_command]
                 run = True
+                break
     if not run:
         cache_commandlist = commandlist["结尾"]
-        for cache_command in cache_commandlist:
+        for cache_command in list(cache_commandlist):
             if command.endswith(cache_command):
+                commandname = cache_commandlist[cache_command]
                 run = True
+                break
     if not run:
         cache_commandlist = commandlist["精准2"]
-        if command in cache_commandlist:
+        if command in list(cache_commandlist):
+            commandname = cache_commandlist[command]
             run = True
 
     if not run and kn_config(""):
         conn = sqlite3.connect(await get_file_path("emoji_1.db"))
         cursor = conn.cursor()
         cursor.execute(f'select * from emoji where emoji = "{command}"')
         data = cursor.fetchone()
@@ -238,16 +246,17 @@
             "atmsgs": atmsgs,
             "info_premission": info_premission,
             "commandname": commandname,
             "groupcode": groupcode,
             "qq": qq,
             "imgmsgs": imgmsgs
         }
-        data = botrun(bot, allfriendlist, allgroupmember_data, msg_info)
-
+        print(msg_info)
+        data = await botrun(bot, allfriendlist, allgroupmember_data, msg_info)
+        print(data)
         # 获取返回信息，进行回复
         code = int(data["code"])
         if code == 0:
             pass
         elif code == 1:
             message = data["message"]
             msg = MessageSegment.text(message)
```

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/bot_run.py` & `nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/bot_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # coding=utf-8
 from .config import kn_config, _config_list
 from .tools import lockst, locked, command_cd
-import plugins
+from .plugins import (
+    plugins_zhanbu
+)
 import time
 import nonebot
 from nonebot import logger
 import os
 import sqlite3
 
 config = nonebot.get_driver().config
@@ -24,35 +26,40 @@
         basepath = os.path.abspath('.') + basepath.removeprefix(".")
         if not basepath.endswith("/"):
             basepath += "/"
     else:
         basepath += "/"
 except Exception as e:
     basepath = os.path.abspath('.') + "/KanonBot/"
+if not os.path.exists(basepath):
+    os.makedirs(basepath)
 
 
-def botrun(bot, allfriendlist, allgroupmemberlist, msg_info):
+async def botrun(bot, allfriendlist, allgroupmemberlist, msg_info):
     # ## 初始化 ##
-    lockdb = './lock.db'
-    lockst(lockdb)
+    lockdb = f"{basepath}db/"
+    if not os.path.exists(lockdb):
+        os.makedirs(lockdb)
+    lockdb += "lock.db"
+    await lockst(lockdb)
     global image, addimage
     msg = msg_info["msg"]
     commands = msg_info["commands"]
     command = str(commands[0])
     if len(commands) >= 2:
         command2 = commands[1]
     else:
         command2 = ''
     atmsg = atmsgs = msg_info["atmsgs"]
     info_premission = msg_info["info_premission"]
     commandname = msg_info["commandname"]
     groupcode = msg_info["groupcode"]
     qq = msg_info["qq"]
     imgmsgs = msg_info["imgmsgs"]
-    botid = bot.self_id()
+    botid = bot.self_id
 
     if len(atmsg) >= 1:
         qq2 = atmsgs[0]
     else:
         if len(command2) >= 5:
             try:
                 qq2 = int(command2)
@@ -130,40 +137,50 @@
         """
         db_path = dbpath + "comfig.db"
         conn = sqlite3.connect(db_path)
         cursor = conn.cursor()
         if not os.path.exists(db_path):
             # 数据库文件 如果文件不存在，会自动在当前目录中创建
             cursor.execute(f"create table {groupcode}(command VARCHAR(10) primary key, state BOOLEAN(20))")
+        cursor.execute("SELECT * FROM sqlite_master WHERE type='table'")
+        datas = cursor.fetchall()
+        tables = []
+        for data in datas:
+            if data[1] != "sqlite_sequence":
+                tables.append(data[1])
+        if groupcode not in tables:
+            cursor.execute(f"create table {groupcode}(command VARCHAR(10) primary key, state BOOLEAN(20))")
         cursor.execute(f'SELECT * FROM {groupcode} WHERE command = "{commandname}"')
         data = cursor.fetchone()
         if data is not None:
             state = data[1]
         else:
             cursor.execute("SELECT * FROM sqlite_master WHERE type='table'")
             datas = cursor.fetchall()
             # 数据库列表转为序列
             tables = []
             for data in datas:
                 if data[1] != "sqlite_sequence":
                     tables.append(data[1])
             if "list" not in tables:
-                cursor.execute(f"create table list(command VARCHAR(10) primary key, state BOOLEAN(20), "
-                               f"message VARCHAR(20), group VARCHAR(20), name VARCHAR(20))")
+                cursor.execute("create table list(command VARCHAR(10) primary key, state BOOLEAN(20), "
+                               "message VARCHAR(20), 'group' VARCHAR(20), name VARCHAR(20))")
             cursor.execute(f'SELECT * FROM list WHERE command="{commandname}"')
             data = cursor.fetchone()
             if data is not None:
                 state = data[1]
                 cursor.execute(f"replace into {groupcode} ('command','state') values('{commandname}',{state})")
                 conn.commit()
             else:
                 config_list = _config_list()
                 if commandname in list(config_list):
+                    print(1)
                     state = config_list[commandname]["state"]
                 else:
+                    print(2)
                     state = False
         cursor.close()
         conn.close()
         return state
 
     # 查询冷却
     def command_cooling() -> bool:
@@ -180,24 +197,25 @@
     # 如果需要继续运行则True
     run = True
 
     if run is True:
         # 处理消息
         if "zhanbu" == commandname:
             if getconfig("zhanbu"):
-                if getconfig("commandcd") and info_premission != "10" and qq not in adminqq:
+                if getconfig("commandcd"):
                     coolingdb = dbpath + "cooling.db"
                     cooling = command_cd(qq, groupcode, timeshort, coolingdb)
-                    if cooling != "off":
+                    if cooling != "off" and info_premission != "10" and qq not in adminqq:
                         code = 1
-                        coolingmessage = f"指令冷却中（{cooling}s)"
+                        message = f"指令冷却中（{cooling}s)"
                         logger.info("指令冷却中")
                     else:
                         at = 'on'
-                        message, returnpath = plugins.plugins_zhanbu(qq, cachepath)
+                        logger.info(f"run-{commandname}")
+                        message, returnpath = plugins_zhanbu(qq, cachepath)
                         if returnpath is not None:
                             code = 3
                         else:
                             code = 1
         elif "###" == commandname:
             pass
```

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/plugins.py` & `nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/plugins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,83 @@
-import random
+# coding=utf-8
 import random
 from nonebot import logger
 import nonebot
 import os
 import sqlite3
 from .config import kn_config, _zhanbu_datas
 from .tools import get_file_path, connect_api
 
 config = nonebot.get_driver().config
-# ÅäÖÃ2£º
+# 配置2：
 try:
     basepath = config.kanon_basepath
     if "\\" in basepath:
         basepath = basepath.replace("\\", "/")
     if basepath.startswith("./"):
         basepath = os.path.abspath('.') + basepath.removeprefix(".")
         if not basepath.endswith("/"):
             basepath += "/"
     else:
         basepath += "/"
 except Exception as e:
     basepath = os.path.abspath('.') + "/KanonBot/"
 
+
 def plugins_zhanbu(qq, cachepath):
     message = ""
     returnpath = None
 
     zhanbudb = cachepath + 'zhanbu/'
     if not os.path.exists(zhanbudb):
         os.makedirs(zhanbudb)
     zhanbudb = f"{zhanbudb}zhanbu.db"
 
     conn = sqlite3.connect(zhanbudb)
     cursor = conn.cursor()
     cursor.execute("SELECT * FROM sqlite_master WHERE type='table'")
     datas = cursor.fetchall()
-    # Êý¾Ý¿âÁÐ±í×ªÎªÐòÁÐ
+    # 数据库列表转为序列
     tables = []
     for data in datas:
         if data[1] != "sqlite_sequence":
             tables.append(data[1])
     if "zhanbu" not in tables:
         cursor.execute('create table zhanbu (userid varchar(10) primary key, id varchar(20))')
     cursor.execute(f'select * from zhanbu where userid = "{qq}"')
     data = cursor.fetchone()
     if data is None:
         # zhanbu_datas = _zhanbu_datas()
         # zhanbu_id = random.choice(list(zhanbu_datas))
         zhanbu_id = str(random.randint(0, 116))
         # zhanbu_data = zhanbu_datas[zhanbu_id]
+
+        # 写入占卜结果
+
+
+
         if kn_config("kanon_api-state"):
-            # Èç¹û¿ªÆôÁËapi£¬Ôò´Ó·þÎñÆ÷ÏÂÔØÕ¼²·Êý¾Ý
-            returnpath = f"{basepath}image/Õ¼²·1/"
+            # 如果开启了api，则从服务器下载占卜数据
+            returnpath = f"{basepath}image/占卜1/"
             if not os.path.exists(returnpath):
                 os.makedirs(returnpath)
             returnpath += f"{zhanbu_id}.png"
             if not os.path.exists(returnpath):
-                # Èç¹ûÎÄ¼þÎ´»º´æ£¬Ôò»º´æÏÂÀ´
-                url = kn_config("kanon_api-url") + f"api/image?imageid=knapi-zhanbu1-{zhanbu_id}"
+                # 如果文件未缓存，则缓存下来
+                url = f"{kn_config('kanon_api-url')}/api/image?imageid=knapi-zhanbu1-{zhanbu_id}"
                 image = connect_api("image", url)
-                image.save(f"{cachepath}Õ¼²·1/{zhanbu_id}.png")
+                returnpath = f"{basepath}image/占卜1/{zhanbu_id}.png"
+                image.save(returnpath)
+                message = "今日占卜结果是："
         else:
-            # Ê¹ÓÃ±¾µØÊý¾Ý
-            # message = f"½ñÈÕÕ¼²·½á¹û£º{zhanbu_data['title']}\n{zhanbu_data['message']}"
-            message = f"½ñÈÕÕ¼²·½á¹û£º{zhanbu_id}"
+            # 使用本地数据
+            # message = f"今日占卜结果：{zhanbu_data['title']}\n{zhanbu_data['message']}"
+            message = f"今日占卜结果：{zhanbu_id}"
         pass
     else:
-        message = "½ñÈÕÕ¼²·½á¹ûÊÇ£º"
+        message = "今日占卜结果是："
     cursor.close()
     conn.close()
 
     return message, returnpath
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/tools.py` & `nonebot_plugin_kanonbot-0.0.1b2/nonebot_plugin_kanonbot/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#coding=utf-8
+# coding=utf-8
 import httpx
 from PIL import Image
 from io import BytesIO
 import sqlite3
 import random
 import json
 from nonebot import logger
@@ -58,14 +58,15 @@
     """
     连接api以获取内容
     :param type: 下载类型。例：“json”, "image", "file"
     :param url: url。例："http://cdn.kanon.ink/json/config?name=ping"
     :param post_json: post获取时的内容。例：{"data": "data_here"}
     :param file_path: 文件保存位置。例："C:/file.zip"
     """
+    logger.info(f"connect-{url}")
     # 把api调用的代码放在一起，也许未来改为异步调取
     if type == "json":
         if post_json is None:
             return json.loads(httpx.get(url).text)
         else:
             return json.loads(httpx.post(url, json=post_json).text)
     elif type == "image":
@@ -108,26 +109,26 @@
     :return:
     """
     import time
     sleeptime = random.randint(1, 200)
     sleeptime = float(sleeptime) / 100
     time.sleep(sleeptime)
     # 读取锁定
-    try:
-        # 数据库文件 如果文件不存在，会自动在当前目录中创建
-        conn = sqlite3.connect(lockdb)
-        cursor = conn.cursor()
-        cursor.execute('create table lock (name VARCHAR(10) primary key, lock VARCHAR(20))')
-        cursor.close()
-        conn.close()
-    except:
-        print('已存在锁定数据库，开始读取数据')
-    # 查询数据
+
     conn = sqlite3.connect(lockdb)
     cursor = conn.cursor()
+    cursor.execute("SELECT * FROM sqlite_master WHERE type='table'")
+    datas = cursor.fetchall()
+    tables = []
+    for data in datas:
+        if data[1] != "sqlite_sequence":
+            tables.append(data[1])
+    if "lock" not in tables:
+        cursor.execute('create table lock (name VARCHAR(10) primary key, lock VARCHAR(20))')
+    # 查询数据
     cursor.execute('select * from lock where name = "lock"')
     locking = cursor.fetchone()
     cursor.close()
     conn.close()
 
     # 判断锁定
     if locking == 'on':
```

### Comparing `nonebot_plugin_kanonbot-0.0.1b1/setup.py` & `nonebot_plugin_kanonbot-0.0.1b2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_kanonbot',
-      version='0.0.1-beta1',
+      version='0.0.1-beta2',
       description='nonebot plugin kanonbot',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_kanonbot',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

