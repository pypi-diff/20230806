# Comparing `tmp/reprim-0.1.2.tar.gz` & `tmp/reprim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprim-0.1.2.tar", last modified: Mon Jul 17 21:26:04 2023, max compression
+gzip compressed data, was "reprim-0.1.3.tar", last modified: Sun Aug  6 15:05:18 2023, max compression
```

## Comparing `reprim-0.1.2.tar` & `reprim-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.661732 reprim-0.1.2/
--rw-rw-rw-   0        0        0      683 2023-07-17 21:26:04.660734 reprim-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.573461 reprim-0.1.2/RePrIm/
--rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.1.2/RePrIm/__init__.py
--rw-rw-rw-   0        0        0    20390 2023-07-15 17:24:46.000000 reprim-0.1.2/RePrIm/reprim.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.634298 reprim-0.1.2/RePrIm/util/
--rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.1.2/RePrIm/util/hardware_monitor.py
--rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.1.2/RePrIm/util/lib.py
--rw-rw-rw-   0        0        0     3125 2023-07-15 15:22:07.000000 reprim-0.1.2/RePrIm/util/process.py
--rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.1.2/RePrIm/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-17 21:26:04.654790 reprim-0.1.2/reprim.egg-info/
--rw-rw-rw-   0        0        0      683 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 21:26:04.000000 reprim-0.1.2/reprim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 21:26:04.661732 reprim-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-17 21:25:43.000000 reprim-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:05:18.632042 reprim-0.1.3/
+-rw-rw-rw-   0        0        0      683 2023-08-06 15:05:18.631045 reprim-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 15:05:18.608106 reprim-0.1.3/RePrIm/
+-rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.1.3/RePrIm/__init__.py
+-rw-rw-rw-   0        0        0    20383 2023-08-06 14:59:58.000000 reprim-0.1.3/RePrIm/reprim.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:05:18.612096 reprim-0.1.3/RePrIm/util/
+-rw-rw-rw-   0        0        0     1759 2023-08-06 13:52:57.000000 reprim-0.1.3/RePrIm/util/hardware_monitor.py
+-rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.1.3/RePrIm/util/lib.py
+-rw-rw-rw-   0        0        0     3431 2023-08-06 15:04:00.000000 reprim-0.1.3/RePrIm/util/process.py
+-rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.1.3/RePrIm/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:05:18.630047 reprim-0.1.3/reprim.egg-info/
+-rw-rw-rw-   0        0        0      683 2023-08-06 15:05:18.000000 reprim-0.1.3/reprim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-08-06 15:05:18.000000 reprim-0.1.3/reprim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:05:18.000000 reprim-0.1.3/reprim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-08-06 15:05:18.000000 reprim-0.1.3/reprim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-06 15:05:18.000000 reprim-0.1.3/reprim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:05:18.632042 reprim-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-08-06 15:05:16.000000 reprim-0.1.3/setup.py
```

### Comparing `reprim-0.1.2/PKG-INFO` & `reprim-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.1.2
+Version: 0.1.3
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.1.2/RePrIm/reprim.py` & `reprim-0.1.3/RePrIm/reprim.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,20 +101,20 @@
     file_view_func(filename, call.message.id, call.message.chat.id)
 
 
 def file_view_func(filename, message_id, chat_id):
     only_name = os.path.split(tools.unlex(filename))[1]
     markup = types.InlineKeyboardMarkup()
     markup.row(types.InlineKeyboardButton(text='⬇️download',
-                                          callback_data=json.dumps({"handler": "download", 'data': filename})))
-    markup.row(types.InlineKeyboardButton(text='🗑️delete',
+                                          callback_data=json.dumps({"handler": "download", 'data': filename})),
+               types.InlineKeyboardButton(text='🗑️delete',
                                           callback_data=json.dumps({"handler": "?delete", "data": filename})))
     markup.row(types.InlineKeyboardButton(text='✏️rename',
-                                          callback_data=json.dumps({"handler": "rename", 'data': filename})))
-    markup.row(types.InlineKeyboardButton(text='🔄replace',
+                                          callback_data=json.dumps({"handler": "rename", 'data': filename})),
+               types.InlineKeyboardButton(text='🔄replace',
                                           callback_data=json.dumps({"handler": "replace", "data": filename})))
     if only_name.endswith('.exe') or only_name.endswith('.py'):
         markup.row(types.InlineKeyboardButton(text='▶️run',
                                               callback_data=json.dumps({"handler": "run", "data": filename})))
     markup.row(types.InlineKeyboardButton(text='🔙', callback_data=json.dumps({"handler": "explore",
                                                                               "data": os.path.dirname(filename)})),
                types.InlineKeyboardButton(text='❌', callback_data='{"handler": "close"}'))
@@ -343,31 +343,27 @@
     bot.answer_callback_query(text='send command', callback_query_id=call.id)
     bot.register_next_step_handler_by_chat_id(chat_id=call.message.chat.id, callback=console_handler,
                                               file=tools.unlex(file))
 
 
 def console_handler(message, file):
     bot.delete_message(chat_id=message.chat.id, message_id=message.id)
-    old_cwd = os.getcwd()
-    os.chdir(file)
-    os.system(message.text)
-    os.chdir(old_cwd)
+    process.Process(absfile=os.path.join(file, 'a.txt'), default_dir=os.getcwd(), handler=bot, console=message.text)
 
 
 @bot.callback_query_handler(func=lambda call: json.loads(call.data)['handler'] == 'download_dir')
 def download_dir(call):
     bot.clear_step_handler_by_chat_id(chat_id=call.message.chat.id)
     bot.answer_callback_query(callback_query_id=call.id, text='building zip file...')
     path = tools.unlex(json.loads(call.data)['data'])
     chat_id = call.message.chat.id
     archive = shutil.make_archive('buff', 'zip', path)
     with open(archive, mode='rb') as rf:
         data = BytesIO(rf.read())
         data.name = f'{path.split("//")[-1]}.zip'
-        print(data.name)
         if data.name == '..zip':
             data.name = 'source.zip'
     os.remove('buff.zip')
     markup = types.InlineKeyboardMarkup()
     markup.row(types.InlineKeyboardButton(text='❌', callback_data='{"handler": "close"}'))
     send(blob=data, chat_id=chat_id, mk=markup)
```

### Comparing `reprim-0.1.2/RePrIm/util/hardware_monitor.py` & `reprim-0.1.3/RePrIm/util/hardware_monitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import os
 import clr
 
 
-if not os.path.isfile(os.path.join(os.path.split(__file__)[0], 'lib.dll')):
-    os.renames(os.path.join(os.path.split(__file__)[0], 'lib.py'), os.path.join(os.path.split(__file__)[0], 'lib.dll'))
-
 openhardwaremonitor_hwtypes = [
     'Mainboard', 'SuperIO', 'CPU', 'RAM', 'GpuNvidia', 'GpuAti', 'TBalancer', 'Heatmaster', 'HDD'
 ]
 openhardwaremonitor_sensortypes = [
     'Voltage', 'Clock', 'Temperature', 'Load', 'Fan', 'Flow', 'Control', 'Level',
     'Factor', 'Power', 'Data', 'SmallData'
 ]
```

### Comparing `reprim-0.1.2/RePrIm/util/lib.py` & `reprim-0.1.3/RePrIm/util/lib.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.2/RePrIm/util/process.py` & `reprim-0.1.3/RePrIm/util/process.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,85 @@
+import datetime
 import json
 import os
 import sys
 import subprocess
 from threading import Thread
 from telebot.types import InlineKeyboardMarkup, InlineKeyboardButton
 from .tools import data
 
 
 pid = 0
 processes = {}
 
 
 class Process:
-    def __init__(self, absfile, default_dir, handler):
+    def __init__(self, absfile, default_dir, handler, console=None):
         global pid
         self.absfile = absfile
         self.id = pid + 1
         pid += 1
         os.chdir(os.path.dirname(absfile))
-        args = [sys.executable, absfile] if absfile.endswith('.py') else [absfile]
+        args = [sys.executable, absfile] if absfile.endswith('.py') else ([absfile] if not console else console.split())
         self.process = subprocess.Popen(args=args, stderr=subprocess.PIPE, stdout=subprocess.PIPE,
                                         stdin=subprocess.PIPE)
         os.chdir(default_dir)
         self.handler = handler
-        self.name = os.path.split(absfile)[1]
+        self.name = os.path.split(absfile)[1] if not console else 'console'
         self.alive = True
         processes[self.id] = self
         self.thread = Thread(target=self.daemon)
         self.thread.start()
-        self.alive_thread = Thread(target=self.alive_breaker)
-        self.alive_thread.start()
 
     def daemon(self):
         try:
             mk = InlineKeyboardMarkup()
             mk.row(InlineKeyboardButton('communicate',
                                         callback_data=json.dumps({"handler": "communicate", "data": self.id})))
             mk.row(InlineKeyboardButton('❌', callback_data='{"handler": "close"}'))
-            while self.alive:
+            while self.getalive():
                 self.get_out(mk)
             mk = InlineKeyboardMarkup()
             mk.row(InlineKeyboardButton('❌', callback_data='{"handler": "close"}'))
             err = self.process.stderr.read().decode()
             self.handler.send_message(chat_id=data['host'],
                                       text=f"process {self.name} was completed{' with error ' + err if err else ''}",
                                       reply_markup=mk)
             processes.pop(self.id)
-        except:
+        except Exception as e:
+            print(e)
             self.kill()
             processes.pop(self.id)
             mk = InlineKeyboardMarkup()
             mk.row(InlineKeyboardButton('❌', callback_data='{"handler": "close"}'))
             self.handler.send_message(chat_id=data['host'],
                                       text=f"process {self.name} was completed with RePrIm error",
                                       reply_markup=mk)
 
     def communicate(self, info):
         self.process.stdin.write(str(info).encode())
         self.process.stdin.close()
 
     def get_out(self, mk):
-        out = self.process.stdout.readline().decode()
-        if out:
-            self.handler.send_message(chat_id=data['host'], text=f"out from {self.name}:\n{out}",
-                                      reply_markup=mk)
-
-    def alive_breaker(self):
-        while self.alive:
-            if not self.getalive():
-                self.alive = False
+        try:
+            out = self.read_io(2)[:4096]
+            if out:
+                self.handler.send_message(chat_id=data['host'], text=f"out from {self.name}:\n{out}",
+                                          reply_markup=mk)
+        except subprocess.TimeoutExpired:
+            pass
+
+    def read_io(self, timeout):
+        endtime = datetime.datetime.now() + datetime.timedelta(seconds=timeout)
+        stdout = ''
+        while endtime > datetime.datetime.now():
+            out = self.process.stdout.readline().decode()
+            if out:
+                stdout += out
+        return stdout
 
     def kill(self):
         try:
             if self.name.endswith('.py'):
                 self.process.kill()
             else:
                 subprocess.Popen(f'taskkill /im {self.name} /f')
```

### Comparing `reprim-0.1.2/RePrIm/util/tools.py` & `reprim-0.1.3/RePrIm/util/tools.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.2/reprim.egg-info/PKG-INFO` & `reprim-0.1.3/reprim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.1.2
+Version: 0.1.3
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.1.2/setup.py` & `reprim-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 requirements = ["pytelegrambotapi", "pythonnet"]
 
 
 setup(
     name="reprim",
-    version="0.1.2",
+    version="0.1.3",
     author="GGergy",
     author_email="gergy2k07@gmail.com",
     description="for questions write me in Telegram (@IDieLast)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/GGergy/RePrIm/",
     packages=['RePrIm', 'RePrIm/util'],
```

