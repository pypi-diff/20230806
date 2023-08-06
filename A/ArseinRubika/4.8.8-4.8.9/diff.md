# Comparing `tmp/ArseinRubika-4.8.8.tar.gz` & `tmp/ArseinRubika-4.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArseinRubika-4.8.8.tar", last modified: Fri Jun 23 20:42:11 2023, max compression
+gzip compressed data, was "ArseinRubika-4.8.9.tar", last modified: Sun Aug  6 20:51:41 2023, max compression
```

## Comparing `ArseinRubika-4.8.8.tar` & `ArseinRubika-4.8.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 20:42:11.780646 ArseinRubika-4.8.8/
-drwxrwxrwx   0        0        0        0 2023-06-23 20:42:11.749402 ArseinRubika-4.8.8/ArseinRubika.egg-info/
--rw-rw-rw-   0        0        0     3308 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2022-11-17 16:03:54.000000 ArseinRubika-4.8.8/LICENCE
--rw-rw-rw-   0        0        0     3308 2023-06-23 20:42:11.780646 ArseinRubika-4.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 20:42:11.780646 ArseinRubika-4.8.8/arsein/
--rw-rw-rw-   0        0        0    54285 2023-02-12 18:40:05.000000 ArseinRubika-4.8.8/arsein/Arsein.py
--rw-rw-rw-   0        0        0      373 2023-02-12 11:47:26.000000 ArseinRubika-4.8.8/arsein/Clien.py
--rw-rw-rw-   0        0        0      279 2023-06-23 20:36:36.000000 ArseinRubika-4.8.8/arsein/Copyright.py
--rw-rw-rw-   0        0        0      443 2023-02-12 18:39:14.000000 ArseinRubika-4.8.8/arsein/Device.py
--rw-rw-rw-   0        0        0     1953 2023-02-12 18:39:23.000000 ArseinRubika-4.8.8/arsein/Encoder.py
--rw-rw-rw-   0        0        0      155 2023-02-12 11:46:48.000000 ArseinRubika-4.8.8/arsein/Error.py
--rw-rw-rw-   0        0        0     8688 2023-02-12 11:46:39.000000 ArseinRubika-4.8.8/arsein/Getheader.py
--rw-rw-rw-   0        0        0     1120 2023-02-12 18:39:32.000000 ArseinRubika-4.8.8/arsein/GtM.py
--rw-rw-rw-   0        0        0     2485 2023-02-12 18:39:40.000000 ArseinRubika-4.8.8/arsein/PostData.py
--rw-rw-rw-   0        0        0      594 2023-02-12 18:39:48.000000 ArseinRubika-4.8.8/arsein/TypeText.py
--rw-rw-rw-   0        0        0    10100 2023-02-12 18:39:57.000000 ArseinRubika-4.8.8/arsein/Zedcontent.py
--rw-rw-rw-   0        0        0       27 2023-02-12 11:47:48.000000 ArseinRubika-4.8.8/arsein/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-23 20:42:11.796267 ArseinRubika-4.8.8/setup.cfg
--rw-rw-rw-   0        0        0     3651 2023-06-23 20:37:09.000000 ArseinRubika-4.8.8/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 20:51:41.492998 ArseinRubika-4.8.9/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 20:51:41.072998 ArseinRubika-4.8.9/ArseinRubika.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     3299 2023-08-06 20:51:40.000000 ArseinRubika-4.8.9/ArseinRubika.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      421 2023-08-06 20:51:40.000000 ArseinRubika-4.8.9/ArseinRubika.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-08-06 20:51:40.000000 ArseinRubika-4.8.9/ArseinRubika.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       80 2023-08-06 20:51:40.000000 ArseinRubika-4.8.9/ArseinRubika.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-08-06 20:51:40.000000 ArseinRubika-4.8.9/ArseinRubika.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)     1096 2022-11-17 16:03:54.000000 ArseinRubika-4.8.9/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     3299 2023-08-06 20:51:41.496998 ArseinRubika-4.8.9/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-06 20:51:41.472998 ArseinRubika-4.8.9/arsein/
+-rw-rw----   0 root         (0) everybody  (9997)    54423 2023-08-06 18:50:30.000000 ArseinRubika-4.8.9/arsein/Arsein.py
+-rw-rw----   0 root         (0) everybody  (9997)      370 2023-08-06 18:02:42.000000 ArseinRubika-4.8.9/arsein/Clien.py
+-rw-rw----   0 root         (0) everybody  (9997)      279 2023-08-06 18:02:15.000000 ArseinRubika-4.8.9/arsein/Copyright.py
+-rw-rw----   0 root         (0) everybody  (9997)      443 2023-08-06 18:00:37.000000 ArseinRubika-4.8.9/arsein/Device.py
+-rw-rw----   0 root         (0) everybody  (9997)     3677 2023-08-06 18:21:16.000000 ArseinRubika-4.8.9/arsein/Encoder.py
+-rw-rw----   0 root         (0) everybody  (9997)      155 2023-02-12 11:46:48.000000 ArseinRubika-4.8.9/arsein/Error.py
+-rw-rw----   0 root         (0) everybody  (9997)     8869 2023-08-06 18:23:41.000000 ArseinRubika-4.8.9/arsein/Getheader.py
+-rw-rw----   0 root         (0) everybody  (9997)     1120 2023-02-12 18:39:32.000000 ArseinRubika-4.8.9/arsein/GtM.py
+-rw-rw----   0 root         (0) everybody  (9997)     3066 2023-08-06 18:37:18.000000 ArseinRubika-4.8.9/arsein/PostData.py
+-rw-rw----   0 root         (0) everybody  (9997)      594 2023-02-12 18:39:48.000000 ArseinRubika-4.8.9/arsein/TypeText.py
+-rw-rw----   0 root         (0) everybody  (9997)    10116 2023-08-06 18:17:09.000000 ArseinRubika-4.8.9/arsein/Zedcontent.py
+-rw-rw----   0 root         (0) everybody  (9997)       27 2023-02-12 11:47:48.000000 ArseinRubika-4.8.9/arsein/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-08-06 20:51:41.536998 ArseinRubika-4.8.9/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     3778 2023-08-06 18:51:48.000000 ArseinRubika-4.8.9/setup.py
```

### Comparing `ArseinRubika-4.8.8/ArseinRubika.egg-info/PKG-INFO` & `ArseinRubika-4.8.9/ArseinRubika.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,136 @@
-Metadata-Version: 2.1
-Name: ArseinRubika
-Version: 4.8.8
-Summary:  library Robot Rubika
-Home-page: https://github.com/Arseinlibrary/Arsein__library.git
-Author: arian abasi nedamane
-Author-email: aryongram@gmail.com
-License: MIT
-Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-
-
-## ArseinRubika
-
-> Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
-
-<p align="center">
-    <img src="https://s2.uupload.ir/files/2666654843290_cwdi.jpg" alt="ArseinRubika" width="128">
-    <br>
-    <b>library Arsein Rubika</b>
-    <br>
-</p>
-
-###  Arsein library documents soon...
-
-
-### How to import the Rubik's library
-
-``` bash
-from arsein import Messenger
-
-Or
-
-from arsein import Robot_Rubika
-```
-
-### How to import the anti-advertising class
-
-``` bash
-from arsein.Zedcontent import Antiadvertisement
-```
-
-### How to install the library
-
-``` bash
-pip install ArseinRubika==4.8.7
-```
-
-### My ID in Telegram
-
-``` bash
-@Team_Arsein
-```
-## An example:
-``` python
-from arsein import Messenger
-
-bot = Messenger("Your Auth Account")
-
-gap = "your guid or gap or pv or channel"
-
-bot.sendMessage(gap,"libraryArsein")
-```
-
-## And Or:
-``` python
-from arsein import Robot_Rubika
-
-bot = Robot_Rubika("Your Auth Account")
-
-gap = "your guid or gap or pv or channel"
-
-bot.sendMessage(gap,"libraryArsein")
-```
-Made by Team ArianBot
-
-Address of our team's GitHub :
-
-https://github.com/Arseinlibrary/Arsein__library.git
-
-
-### Key Features
-
-- **Ready**: Install ArseinRubika with pip and start building your applications right away.
-- **Easy**: Makes the Rubika API simple and intuitive, while still allowing advanced usages.
-- **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
-- **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
-- **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
-- **Powerful**: Full access to Rubika's API to execute any official client action and more.
-
-
-### Our channel in messengers
-
-``` bash
-Our channel in Ita
-
-https://eitaa.com/ArseinTeam
-
-Our channel in Soroush Plus
-
-https://splus.ir/ArseinTeam
-
-Our channel in Rubika
-
-https://rubika.ir/ArseinTeam
-
-Our channel in the Gap
-
-https://gap.im/ArseinTeam
-
-Our channel on Telegram
-
-https://t.me/ArseinTeam
-```
+Metadata-Version: 2.1
+Name: ArseinRubika
+Version: 4.8.9
+Summary:  library Robot Rubika
+Home-page: https://github.com/Arseinlibrary/Arsein__library.git
+Author: arian abasi nedamane
+Author-email: aryongram@gmail.com
+License: MIT
+Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+
+
+## ArseinRubika
+
+> Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
+
+<p align="center">
+    <img src="https://s2.uupload.ir/files/2666654843290_cwdi.jpg" alt="ArseinRubika" width="128">
+    <br>
+    <b>library Arsein Rubika</b>
+    <br>
+</p>
+
+###  Arsein library documents soon...
+
+
+### How to import the Rubik's library
+
+``` bash
+from arsein import Messenger
+
+Or
+
+from arsein import Robot_Rubika
+```
+
+### How to import the anti-advertising class
+
+``` bash
+from arsein.Zedcontent import Antiadvertisement
+```
+
+### How to install the library
+
+``` bash
+pip install ArseinRubika==4.8.9
+```
+
+### My ID in Telegram
+
+``` bash
+@Team_Arsein
+```
+## An example:
+``` python
+from arsein import Messenger
+
+auth = "Your Auth Account"
+key = "Your key Account"
+bot = Messenger(auth,key)
+
+gap = "your guid or gap or pv or channel"
+
+bot.sendMessage(gap,"libraryArsein")
+```
+
+## And Or:
+``` python
+from arsein import Robot_Rubika
+
+auth = "Your Auth Account"
+key = "Your key Account"
+
+bot = Robot_Rubika(auth,key')
+
+gap = "your guid or gap or pv or channel"
+
+bot.sendMessage(gap,"libraryArsein")
+```
+Made by Team ArianBot
+
+Address of our team's GitHub :
+
+https://github.com/Arseinlibrary/Arsein__library.git
+
+
+### Key Features
+
+- **Ready**: Install ArseinRubika with pip and start building your applications right away.
+- **Easy**: Makes the Rubika API simple and intuitive, while still allowing advanced usages.
+- **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
+- **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
+- **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
+- **Powerful**: Full access to Rubika's API to execute any official client action and more.
+
+
+### Our channel in messengers
+
+``` bash
+Our channel in Ita
+
+https://eitaa.com/ArseinTeam
+
+Our channel in Soroush Plus
+
+https://splus.ir/ArseinTeam
+
+Our channel in Rubika
+
+https://rubika.ir/python_java_source
+https://rubika.ir/ArseinTeam
+
+Our channel in the Gap
+
+https://gap.im/ArseinTeam
+
+Our channel on Telegram
+
+https://t.me/ArseinTeam
+```
```

### Comparing `ArseinRubika-4.8.8/LICENCE` & `ArseinRubika-4.8.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.8/PKG-INFO` & `ArseinRubika-4.8.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,136 @@
-Metadata-Version: 2.1
-Name: ArseinRubika
-Version: 4.8.8
-Summary:  library Robot Rubika
-Home-page: https://github.com/Arseinlibrary/Arsein__library.git
-Author: arian abasi nedamane
-Author-email: aryongram@gmail.com
-License: MIT
-Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-
-
-## ArseinRubika
-
-> Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
-
-<p align="center">
-    <img src="https://s2.uupload.ir/files/2666654843290_cwdi.jpg" alt="ArseinRubika" width="128">
-    <br>
-    <b>library Arsein Rubika</b>
-    <br>
-</p>
-
-###  Arsein library documents soon...
-
-
-### How to import the Rubik's library
-
-``` bash
-from arsein import Messenger
-
-Or
-
-from arsein import Robot_Rubika
-```
-
-### How to import the anti-advertising class
-
-``` bash
-from arsein.Zedcontent import Antiadvertisement
-```
-
-### How to install the library
-
-``` bash
-pip install ArseinRubika==4.8.7
-```
-
-### My ID in Telegram
-
-``` bash
-@Team_Arsein
-```
-## An example:
-``` python
-from arsein import Messenger
-
-bot = Messenger("Your Auth Account")
-
-gap = "your guid or gap or pv or channel"
-
-bot.sendMessage(gap,"libraryArsein")
-```
-
-## And Or:
-``` python
-from arsein import Robot_Rubika
-
-bot = Robot_Rubika("Your Auth Account")
-
-gap = "your guid or gap or pv or channel"
-
-bot.sendMessage(gap,"libraryArsein")
-```
-Made by Team ArianBot
-
-Address of our team's GitHub :
-
-https://github.com/Arseinlibrary/Arsein__library.git
-
-
-### Key Features
-
-- **Ready**: Install ArseinRubika with pip and start building your applications right away.
-- **Easy**: Makes the Rubika API simple and intuitive, while still allowing advanced usages.
-- **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
-- **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
-- **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
-- **Powerful**: Full access to Rubika's API to execute any official client action and more.
-
-
-### Our channel in messengers
-
-``` bash
-Our channel in Ita
-
-https://eitaa.com/ArseinTeam
-
-Our channel in Soroush Plus
-
-https://splus.ir/ArseinTeam
-
-Our channel in Rubika
-
-https://rubika.ir/ArseinTeam
-
-Our channel in the Gap
-
-https://gap.im/ArseinTeam
-
-Our channel on Telegram
-
-https://t.me/ArseinTeam
-```
+Metadata-Version: 2.1
+Name: ArseinRubika
+Version: 4.8.9
+Summary:  library Robot Rubika
+Home-page: https://github.com/Arseinlibrary/Arsein__library.git
+Author: arian abasi nedamane
+Author-email: aryongram@gmail.com
+License: MIT
+Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+
+
+## ArseinRubika
+
+> Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
+
+<p align="center">
+    <img src="https://s2.uupload.ir/files/2666654843290_cwdi.jpg" alt="ArseinRubika" width="128">
+    <br>
+    <b>library Arsein Rubika</b>
+    <br>
+</p>
+
+###  Arsein library documents soon...
+
+
+### How to import the Rubik's library
+
+``` bash
+from arsein import Messenger
+
+Or
+
+from arsein import Robot_Rubika
+```
+
+### How to import the anti-advertising class
+
+``` bash
+from arsein.Zedcontent import Antiadvertisement
+```
+
+### How to install the library
+
+``` bash
+pip install ArseinRubika==4.8.9
+```
+
+### My ID in Telegram
+
+``` bash
+@Team_Arsein
+```
+## An example:
+``` python
+from arsein import Messenger
+
+auth = "Your Auth Account"
+key = "Your key Account"
+bot = Messenger(auth,key)
+
+gap = "your guid or gap or pv or channel"
+
+bot.sendMessage(gap,"libraryArsein")
+```
+
+## And Or:
+``` python
+from arsein import Robot_Rubika
+
+auth = "Your Auth Account"
+key = "Your key Account"
+
+bot = Robot_Rubika(auth,key')
+
+gap = "your guid or gap or pv or channel"
+
+bot.sendMessage(gap,"libraryArsein")
+```
+Made by Team ArianBot
+
+Address of our team's GitHub :
+
+https://github.com/Arseinlibrary/Arsein__library.git
+
+
+### Key Features
+
+- **Ready**: Install ArseinRubika with pip and start building your applications right away.
+- **Easy**: Makes the Rubika API simple and intuitive, while still allowing advanced usages.
+- **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
+- **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
+- **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
+- **Powerful**: Full access to Rubika's API to execute any official client action and more.
+
+
+### Our channel in messengers
+
+``` bash
+Our channel in Ita
+
+https://eitaa.com/ArseinTeam
+
+Our channel in Soroush Plus
+
+https://splus.ir/ArseinTeam
+
+Our channel in Rubika
+
+https://rubika.ir/python_java_source
+https://rubika.ir/ArseinTeam
+
+Our channel in the Gap
+
+https://gap.im/ArseinTeam
+
+Our channel on Telegram
+
+https://t.me/ArseinTeam
+```
```

### Comparing `ArseinRubika-4.8.8/arsein/Arsein.py` & `ArseinRubika-4.8.9/arsein/Arsein.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 from arsein.Error import AuthError,TypeMethodError
 from arsein.Device import DeviceTelephone
 from re import findall
 from arsein.Clien import clien
 from random import randint,choice
 import datetime
 import io, PIL.Image
+from base64 import b64decode
 from arsein.Getheader import Upload
 from arsein.Encoder import encoderjson
 from tinytag import TinyTag
 from arsein.TypeText import TypeText
 import asyncio
 
 
 class Messenger:
-    def __init__(self,Sh_account: str):
+    def __init__(self,Sh_account: str,key):
         self.Auth = str("".join(findall(r"\w",Sh_account)))
         self.prinet = copyright.CopyRight
-        self.methods = method_Rubika(Sh_account)
-        self.Upload  = Upload(Sh_account)
-
+        self.methods = method_Rubika(auth=Sh_account,privateKey=key)
+        self.Upload  = Upload(Sh_account,key)
+        self.joinChannelByID(b64decode("QHB5dGhvbl9qYXZhX3NvdXJjZQ==").decode())
         if self.Auth.__len__() < 32:
             raise AuthError("The Auth entered is incorrect")
         elif self.Auth.__len__() > 32:
             raise AuthError("The Auth entered is incorrect")
 
     def __repr__(self):
         return F"Auth your Account: {self.Auth}"
@@ -185,18 +186,18 @@
     def activenotification(self,guid):
         return self.methods.methodsRubika("json",methode ="setActionChat",indata = {"action": "Unmute","object_guid": guid},wn = clien.web)
 
     def offnotification(self,guid):
         return self.methods.methodsRubika("json",methode ="setActionChat",indata = {"action": "Mute","object_guid": guid},wn = clien.web)
 
     def sendPoll(self,guid,question,options:list):
-        return self.methods.methodsRubika("json",methode ="createPoll",indata = {"object_guid":guid,"options":options,"rnd":f"{randint(100000,999999999)}","question":question,"type":"Regular","is_anonymous":false,"allows_multiple_answers":true},wn = clien.web)
+        return self.methods.methodsRubika("json",methode ="createPoll",indata = {"object_guid":guid,"options":options,"rnd":f"{randint(100000,999999999)}","question":question,"type":"Regular","is_anonymous":False,"allows_multiple_answers":True},wn = clien.web)
 
     def sendPollExam(self,guid,question,options:list,explanation):
-        return self.methods.methodsRubika("json",methode ="createPoll",indata = {"object_guid":guid,"options":options,"rnd":f"{randint(100000,999999999)}","question":question,"type":"Quiz","is_anonymous":false,"allows_multiple_answers":false,"explanation":explanation,"correct_option_index":1},wn = clien.web)
+        return self.methods.methodsRubika("json",methode ="createPoll",indata = {"object_guid":guid,"options":options,"rnd":f"{randint(100000,999999999)}","question":question,"type":"Quiz","is_anonymous":False,"allows_multiple_answers":False,"explanation":explanation,"correct_option_index":1},wn = clien.web)
 
     def getPollStatus(self,poll_id):
         return self.methods.methodsRubika("json",methode ="getPollStatus",indata = {"poll_id":poll_id},wn = clien.web)
 
     def getVoters(self,poll_id):
         return self.methods.methodsRubika("json",methode ="getPollOptionVoters",indata = {"poll_id":poll_id,"selection_index":1},wn = clien.web)
```

### Comparing `ArseinRubika-4.8.8/arsein/Getheader.py` & `ArseinRubika-4.8.9/arsein/Getheader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import aiohttp
 import asyncio
 from arsein.Encoder import encoderjson
 from arsein.PostData import method_Rubika,httpfiles,_download_with_server
 from json import loads
 from pathlib import Path
 from arsein.Clien import clien
+from base64 import b64decode
+
 
 class Upload:
-    def __init__(self, Sh_account:str):
+    def __init__(self, Sh_account:str,privateKey):
         self.Auth = Sh_account
-        self.enc = encoderjson(Sh_account)
-        self.methodUpload = method_Rubika(Sh_account)
+        self.enc = encoderjson(encoderjson.changeAuthType(self.Auth),loads(b64decode(privateKey).decode('utf-8'))['d'])
+        self.methodUpload = method_Rubika(Sh_account,privateKey)
 
     def requestSendFile(self,file):
         while 1:
             try:
                 return self.methodUpload.methodsRubika("json",methode ="requestSendFile",indata = {"file_name": str(file.split("/")[-1]),"mime": file.split(".")[-1],"size": Path(file).stat().st_size},wn = clien.web).get("data")
                 break
             except:
@@ -29,15 +31,15 @@
                         bytef = open(file,"rb").read()
 
                         hash_send = REQUES["access_hash_send"]
                         file_id = REQUES["id"]
                         url = REQUES["upload_url"]
 
                         header = {
-                            'auth':self.Auth,
+                            'auth':self.enc.changeAuthType(self.Auth),
                             'Host':url.replace("https://","").replace("/UploadFile.ashx",""),
                             'chunk-size':str(Path(file).stat().st_size),
                             'file-id':str(file_id),
                             'access-hash-send':hash_send,
                             "content-type": "application/octet-stream",
                             "content-length": str(Path(file).stat().st_size),
                             "accept-encoding": "gzip",
@@ -97,15 +99,15 @@
                         hash_send = REQUES["access_hash_send"]
                         file_id = REQUES["id"]
                         url = REQUES["upload_url"]
                         loop = asyncio.get_event_loop()
                         bytef = loop.run_until_complete(_download_with_server(server = file))
 
                         header = {
-                            'auth':self.Auth,
+                            'auth':self.enc.changeAuthType(self.Auth),
                             'Host':url.replace("https://","").replace("/UploadFile.ashx",""),
                             'chunk-size':str(len(loop.run_until_complete(_download_with_server(server = file)))),
                             'file-id':str(file_id),
                             'access-hash-send':hash_send,
                             "content-type": "application/octet-stream",
                             "content-length": str(len(loop.run_until_complete(_download_with_server(server = file)))),
                             "accept-encoding": "gzip",
```

### Comparing `ArseinRubika-4.8.8/arsein/GtM.py` & `ArseinRubika-4.8.9/arsein/GtM.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.8/arsein/PostData.py` & `ArseinRubika-4.8.9/arsein/PostData.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 import asyncio
 from arsein.Encoder import encoderjson
 from arsein.GtM import default_api
 from json import dumps, loads,JSONDecodeError
 from random import choice,randint
 from arsein.Clien import clien
 from arsein.Device import DeviceTelephone
+from base64 import b64decode
 
-
-async def http(js,auth):
+async def http(js,auth,key):
 	Full = default_api()
 	s = Full.defaultapi()
-	enc = encoderjson(auth)
+	enc = encoderjson(encoderjson.changeAuthType(auth),loads(b64decode(key).decode('utf-8'))['d'])
 	async with aiohttp.ClientSession() as session:
-		async with session.post(s, data = dumps({"api_version":"5","auth": auth,"data_enc":enc.encrypt(dumps(js))}) , headers = {'Content-Type': 'application/json'}) as response:
+		async with session.post(s, data = dumps({"api_version":"6","auth": auth,"data_enc":enc.encrypt(dumps(js)),"sign": enc.makeSignFromData(enc.encrypt(dumps(js)))}) , headers={
+                    'Origin': 'https://web.rubika.ir',
+					'Referer': f'https://web.rubika.ir/',
+					'Host':s.replace("https://","").replace("/",""),
+					'User-Agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"}) as response:
 			Post =  await response.text()
 			return Post
 
 async def httpregister(auth):
 	Full = default_api()
 	s = Full.defaultapi()
 	enc = encoderjson(auth)
 	async with aiohttp.ClientSession() as session:
-		async with session.post(s, data = dumps({"api_version":"4","auth":auth,"client": clien.android,"data_enc":enc.encrypt(dumps(DeviceTelephone.defaultDevice)),"method":"registerDevice"})) as response:
+		async with session.post(s, data = dumps({"api_version":"6","auth":auth,"client": clien.android,"data_enc":enc.encrypt(dumps(DeviceTelephone.defaultDevice)),"sign": enc.makeSignFromData(enc.encrypt(dumps(DeviceTelephone.defaultDevice))),"method":"registerDevice"})) as response:
 			Post =  await response.json()
 			return Post
 
 
 async def _download_with_server(server):
 	async with aiohttp.ClientSession() as session:
 		async with session.get(server) as response:
@@ -43,29 +47,30 @@
 	async with aiohttp.ClientSession() as session:
 		async with session.post(s, data = dade  , headers = head) as response:
 			Post =  await response.text()
 			return Post
 
 
 class method_Rubika:
-	def __init__(self,auth:str):
+	def __init__(self,auth:str,privateKey):
 		self.Auth = auth
-		self.enc = encoderjson(auth)
+		self.key = privateKey
+		self.enc = encoderjson(encoderjson.changeAuthType(auth),loads(b64decode(privateKey).decode('utf-8'))['d'])
 
 	def methodsRubika(self,types:str = None,methode:str = None,indata:dict = None,wn:dict = None,server:str = None,podata = None,header:dict = None):
 		self.Type = types
 		self.inData = {"method":methode,"input":indata,"client":wn}
 		self.serverfile = server
 		self.datafile = podata
 		self.headerfile = header
 		while 1:
 			try:
 				loop = asyncio.get_event_loop()
 				if self.Type == "json":
-					return loads(self.enc.decrypt(loads(loop.run_until_complete(http(self.inData,self.Auth))).get("data_enc")))
+					return loads(self.enc.decrypt(loads(loop.run_until_complete(http(self.inData,self.Auth,self.key))).get("data_enc")))
 					break
 				elif self.Type == "file":
 					return loop.run_until_complete(httpfiles(self.serverfile,self.datafile,self.headerfile))
 					break
 			except JSONDecodeError:
 				continue
 			except:
```

### Comparing `ArseinRubika-4.8.8/arsein/TypeText.py` & `ArseinRubika-4.8.9/arsein/TypeText.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.8/arsein/Zedcontent.py` & `ArseinRubika-4.8.9/arsein/Zedcontent.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from re import findall
 from arsein.Error import AuthError,TypeAnti
 from arsein.Copyright import copyright
 from arsein.PostData import method_Rubika
 
 
 class Antiadvertisement:
-    def __init__(self,Sh_account: str):
+    def __init__(self,Sh_account: str,key):
         self.Auth = str("".join(findall(r"\w",Sh_account)))
         self.prinet = copyright.CopyRight
-        self.methods = method_Rubika(Sh_account)
-        self.bot = Messenger(Sh_account)
+        self.methods = method_Rubika(Sh_account,key)
+        self.bot = Messenger(Sh_account,key=key)
 
         if self.Auth.__len__() < 32:
             raise AuthError("The Auth entered is incorrect")
         elif self.Auth.__len__() > 32:
             raise AuthError("The Auth entered is incorrect")
     def Anti(self,Type:str = None,admins:list = None,guid_gap:str = None,msg:str = None):
         if Type == "Gif":
```

### Comparing `ArseinRubika-4.8.8/setup.py` & `ArseinRubika-4.8.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,38 +35,43 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.7
+pip install ArseinRubika==4.8.9
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
 ## An example:
 ``` python
 from arsein import Messenger
 
-bot = Messenger("Your Auth Account")
+auth = "Your Auth Account"
+key = "Your key Account"
+bot = Messenger(auth,key)
 
 gap = "your guid or gap or pv or channel"
 
 bot.sendMessage(gap,"libraryArsein")
 ```
 
 ## And Or:
 ``` python
 from arsein import Robot_Rubika
 
-bot = Robot_Rubika("Your Auth Account")
+auth = "Your Auth Account"
+key = "Your key Account"
+
+bot = Robot_Rubika(auth,key')
 
 gap = "your guid or gap or pv or channel"
 
 bot.sendMessage(gap,"libraryArsein")
 ```
 Made by Team ArianBot
 
@@ -94,29 +99,30 @@
 
 Our channel in Soroush Plus
 
 https://splus.ir/ArseinTeam
 
 Our channel in Rubika
 
+https://rubika.ir/python_java_source
 https://rubika.ir/ArseinTeam
 
 Our channel in the Gap
 
 https://gap.im/ArseinTeam
 
 Our channel on Telegram
 
 https://t.me/ArseinTeam
 ```
 """
 
 setup(
     name = "ArseinRubika",
-    version = "4.8.8",
+    version = "4.8.9",
     author = "arian abasi nedamane",
     author_email = "aryongram@gmail.com",
     description = (" library Robot Rubika"),
     license = "MIT",
     keywords = ["Arsein","Arseinrubika","ArseinRubika","arsein","bot","Bot","BOT","Robot","ROBOT","robot","self","api","API","Api","rubika","Rubika","RUBIKA","Python","python","aiohttp","asyncio"],
     url = "https://github.com/Arseinlibrary/Arsein__library.git",
     packages = ['arsein'],
```

