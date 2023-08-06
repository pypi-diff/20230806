# Comparing `tmp/django-telethon-1.1.5a1.tar.gz` & `tmp/django-telethon-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-telethon-1.1.5a1.tar", last modified: Thu Nov  3 20:08:29 2022, max compression
+gzip compressed data, was "dist/django-telethon-1.1.6.tar", last modified: Sun Aug  6 17:55:06 2023, max compression
```

## Comparing `django-telethon-1.1.5a1.tar` & `django-telethon-1.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10939 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9711 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/management/commands/runtelegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7810 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/models/
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2055 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1438 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/sentfiles.py
--rw-rw-rw-   0 root         (0) root         (0)     1830 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      720 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/states.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/receivers.py
--rw-rw-rw-   0 root         (0) root         (0)     9016 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/signals.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4164 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2022-11-03 20:08:23.000000 django-telethon-1.1.5a1/django_telethon/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10939 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      949 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      266 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1864 2022-11-03 20:08:24.000000 django-telethon-1.1.5a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-08-06 17:54:59.000000 django-telethon-1.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-08-06 17:54:59.000000 django-telethon-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-08-06 17:55:06.000000 django-telethon-1.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9722 2023-08-06 17:54:59.000000 django-telethon-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/management/commands/runtelegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7810 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon/models/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/sentfiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/models/states.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/receivers.py
+-rw-rw-rw-   0 root         (0) root         (0)     9016 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2023-08-06 17:54:59.000000 django-telethon-1.1.6/django_telethon/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      949 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-06 17:55:06.000000 django-telethon-1.1.6/django_telethon.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-08-06 17:54:59.000000 django-telethon-1.1.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-08-06 17:55:06.000000 django-telethon-1.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1856 2023-08-06 17:54:59.000000 django-telethon-1.1.6/setup.py
```

### Comparing `django-telethon-1.1.5a1/LICENSE` & `django-telethon-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/PKG-INFO` & `django-telethon-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.1.5a1
+Version: 1.1.6
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -39,21 +39,21 @@
 # Django Telethon config
 
 
   ⭐️ Thanks **everyone** who has starred the project, it means a lot!
 
 This project is to help you use [Telethon](https://docs.telethon.dev/en/stable/index.html). 
 
-Djagno-Telethon is an asyncio Python 3 MTProto library to interact with Telegram's API as a user or through a bot account (bot API alternative).
+Django-Telethon is an asyncio Python 3 MTProto library to interact with Telegram's API as a user or through a bot account (bot API alternative).
 
 ### What is this?
 
 Telegram is a popular messaging application. This library is meant to make it easy for you to write Python programs that can interact with Telegram. Think of it as a wrapper that has already done the heavy job for you, so you can focus on developing an application.
 
-A Django-Telethon session storage implementation backed for Django ORM to use telethon in django projects.
+Django-Telethon is a session storage implementation backend for Django ORM to use telethon in Django projects.
 
 ## Compatibility
 
 * Python 3.7+
 * Django 3.0+
 
 ## Installation
@@ -112,18 +112,18 @@
 python manage.py migrate
 ```
 
 ## Signing In
 
 Before working with Telegram’s API, you need to get your own API ID and hash:
 
-[Login to your Telegram account](https://my.telegram.org/auth) with the phone number of the developer account to use.
-Click under API Development tools.
-A Create new application window will appear. Fill in your application details. There is no need to enter any URL, and only the first two fields (App title and Short name) can currently be changed later.
-Click on Create application at the end. Remember that your API hash is secret and Telegram won’t let you revoke it. Don’t post it anywhere!
+- [Login to your Telegram account](https://my.telegram.org/auth) with the phone number of the developer account to use.
+- Click under API Development tools.
+- Create new application window will appear. Fill in your application details. There is no need to enter any URL, and only the first two fields (App title and Short name) can currently be changed later.
+- Click on Create application at the end. Remember that your API hash is secret and Telegram won’t let you revoke it. Don’t post it anywhere!
 
 ***This API ID and hash is the one used by your application, not your phone number. You can use this API ID and hash with any phone number or even for bot accounts.***
 
 Read more (proxy, bot and etc) [Here](https://docs.telethon.dev/en/stable/basic/signing-in.html).
 
 ## Usage
 
@@ -170,15 +170,15 @@
         try:
             telegram_client.sign_in(phone, code)
         except SessionPasswordNeededError:
             password = input('Enter your password: ')
             telegram_client.sign_in(password=password)    
     ```
 
-#### Doing stuff
+#### Doing stuffs
 
 ```python
 print((await telegram_client.get_me()).stringify())
 
 await telegram_client.send_message('username', 'Hello! Talking to you from Telethon')
 await telegram_client.send_file('username', '/home/myself/Pictures/holidays.jpg')
 
@@ -189,29 +189,29 @@
 @telegram_client.on(telegram_client.NewMessage(pattern='(?i)hi|hello'))
 async def handler(event):
     await event.respond('Hey!')
 ```
 
 ### API
 #### User Login
-1. run the following command to start the server:
+1. Run the following command to start the server:
 
     ```shell script
     python manage.py runserver
     ```
 
-1. run the following command to start telegram client:
+1. Run the following command to start telegram client:
 
     ```shell script
     python manage.py runtelegram
     ```
    
 1. go to [admin panel](http://127.0.0.1:8000/admin/) and [telegram app section](http://127.0.0.1:8000/admin/django_telethon/app/). create a new app. get data from the [your Telegram account](https://my.telegram.org/auth).
 
-1. request code from telegram:
+1. Request code from telegram:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/send-code-request/"
    
@@ -224,15 +224,15 @@
    }
    
    response = requests.request("POST", url, headers=headers, data=payload)
    
    print(response.text)
     ```
 
-1. send this request for sign in:
+1. Send this request for sign in:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/login-user-request/"
    
@@ -249,15 +249,15 @@
    response = requests.request("POST", url, headers=headers, data=payload)
    
    print(response.text)
 
    ```
 
 #### Bot login 
-send this request for sign in:
+Send this request for sign in:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/login-bot-request/"
    
@@ -306,15 +306,15 @@
     supervisorctl status
     ```
 
 ## Listen to events
 
 After login telegram client the signal `telegram_client_registered` is emitted. 
 
-1. you can listen to this signal by using the following code for example put this code to your ```receivers.py``` file in app directory:
+1. You can listen to this signal by using the following code for example put this code to your ```receivers.py``` file in app directory:
    
    ```python
    from functools import partial
    
    from django.dispatch import receiver
    from telethon import events
```

### Comparing `django-telethon-1.1.5a1/README.md` & `django-telethon-1.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 # Django Telethon config
 
 
   ⭐️ Thanks **everyone** who has starred the project, it means a lot!
 
 This project is to help you use [Telethon](https://docs.telethon.dev/en/stable/index.html). 
 
-Djagno-Telethon is an asyncio Python 3 MTProto library to interact with Telegram's API as a user or through a bot account (bot API alternative).
+Django-Telethon is an asyncio Python 3 MTProto library to interact with Telegram's API as a user or through a bot account (bot API alternative).
 
 ### What is this?
 
 Telegram is a popular messaging application. This library is meant to make it easy for you to write Python programs that can interact with Telegram. Think of it as a wrapper that has already done the heavy job for you, so you can focus on developing an application.
 
-A Django-Telethon session storage implementation backed for Django ORM to use telethon in django projects.
+Django-Telethon is a session storage implementation backend for Django ORM to use telethon in Django projects.
 
 ## Compatibility
 
 * Python 3.7+
 * Django 3.0+
 
 ## Installation
@@ -79,18 +79,18 @@
 python manage.py migrate
 ```
 
 ## Signing In
 
 Before working with Telegram’s API, you need to get your own API ID and hash:
 
-[Login to your Telegram account](https://my.telegram.org/auth) with the phone number of the developer account to use.
-Click under API Development tools.
-A Create new application window will appear. Fill in your application details. There is no need to enter any URL, and only the first two fields (App title and Short name) can currently be changed later.
-Click on Create application at the end. Remember that your API hash is secret and Telegram won’t let you revoke it. Don’t post it anywhere!
+- [Login to your Telegram account](https://my.telegram.org/auth) with the phone number of the developer account to use.
+- Click under API Development tools.
+- Create new application window will appear. Fill in your application details. There is no need to enter any URL, and only the first two fields (App title and Short name) can currently be changed later.
+- Click on Create application at the end. Remember that your API hash is secret and Telegram won’t let you revoke it. Don’t post it anywhere!
 
 ***This API ID and hash is the one used by your application, not your phone number. You can use this API ID and hash with any phone number or even for bot accounts.***
 
 Read more (proxy, bot and etc) [Here](https://docs.telethon.dev/en/stable/basic/signing-in.html).
 
 ## Usage
 
@@ -137,15 +137,15 @@
         try:
             telegram_client.sign_in(phone, code)
         except SessionPasswordNeededError:
             password = input('Enter your password: ')
             telegram_client.sign_in(password=password)    
     ```
 
-#### Doing stuff
+#### Doing stuffs
 
 ```python
 print((await telegram_client.get_me()).stringify())
 
 await telegram_client.send_message('username', 'Hello! Talking to you from Telethon')
 await telegram_client.send_file('username', '/home/myself/Pictures/holidays.jpg')
 
@@ -156,29 +156,29 @@
 @telegram_client.on(telegram_client.NewMessage(pattern='(?i)hi|hello'))
 async def handler(event):
     await event.respond('Hey!')
 ```
 
 ### API
 #### User Login
-1. run the following command to start the server:
+1. Run the following command to start the server:
 
     ```shell script
     python manage.py runserver
     ```
 
-1. run the following command to start telegram client:
+1. Run the following command to start telegram client:
 
     ```shell script
     python manage.py runtelegram
     ```
    
 1. go to [admin panel](http://127.0.0.1:8000/admin/) and [telegram app section](http://127.0.0.1:8000/admin/django_telethon/app/). create a new app. get data from the [your Telegram account](https://my.telegram.org/auth).
 
-1. request code from telegram:
+1. Request code from telegram:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/send-code-request/"
    
@@ -191,15 +191,15 @@
    }
    
    response = requests.request("POST", url, headers=headers, data=payload)
    
    print(response.text)
     ```
 
-1. send this request for sign in:
+1. Send this request for sign in:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/login-user-request/"
    
@@ -216,15 +216,15 @@
    response = requests.request("POST", url, headers=headers, data=payload)
    
    print(response.text)
 
    ```
 
 #### Bot login 
-send this request for sign in:
+Send this request for sign in:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/login-bot-request/"
    
@@ -273,15 +273,15 @@
     supervisorctl status
     ```
 
 ## Listen to events
 
 After login telegram client the signal `telegram_client_registered` is emitted. 
 
-1. you can listen to this signal by using the following code for example put this code to your ```receivers.py``` file in app directory:
+1. You can listen to this signal by using the following code for example put this code to your ```receivers.py``` file in app directory:
    
    ```python
    from functools import partial
    
    from django.dispatch import receiver
    from telethon import events
```

### Comparing `django-telethon-1.1.5a1/django_telethon/admin.py` & `django-telethon-1.1.6/django_telethon/admin.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/management/commands/runtelegram.py` & `django-telethon-1.1.6/django_telethon/management/commands/runtelegram.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/migrations/0001_initial.py` & `django-telethon-1.1.6/django_telethon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/models/entities.py` & `django-telethon-1.1.6/django_telethon/models/entities.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/models/login.py` & `django-telethon-1.1.6/django_telethon/models/login.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/models/sentfiles.py` & `django-telethon-1.1.6/django_telethon/models/sentfiles.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/models/sessions.py` & `django-telethon-1.1.6/django_telethon/models/sessions.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/models/states.py` & `django-telethon-1.1.6/django_telethon/models/states.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/receivers.py` & `django-telethon-1.1.6/django_telethon/receivers.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/sessions.py` & `django-telethon-1.1.6/django_telethon/sessions.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/utils.py` & `django-telethon-1.1.6/django_telethon/utils.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon/views.py` & `django-telethon-1.1.6/django_telethon/views.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/django_telethon.egg-info/PKG-INFO` & `django-telethon-1.1.6/django_telethon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.1.5a1
+Version: 1.1.6
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -39,21 +39,21 @@
 # Django Telethon config
 
 
   ⭐️ Thanks **everyone** who has starred the project, it means a lot!
 
 This project is to help you use [Telethon](https://docs.telethon.dev/en/stable/index.html). 
 
-Djagno-Telethon is an asyncio Python 3 MTProto library to interact with Telegram's API as a user or through a bot account (bot API alternative).
+Django-Telethon is an asyncio Python 3 MTProto library to interact with Telegram's API as a user or through a bot account (bot API alternative).
 
 ### What is this?
 
 Telegram is a popular messaging application. This library is meant to make it easy for you to write Python programs that can interact with Telegram. Think of it as a wrapper that has already done the heavy job for you, so you can focus on developing an application.
 
-A Django-Telethon session storage implementation backed for Django ORM to use telethon in django projects.
+Django-Telethon is a session storage implementation backend for Django ORM to use telethon in Django projects.
 
 ## Compatibility
 
 * Python 3.7+
 * Django 3.0+
 
 ## Installation
@@ -112,18 +112,18 @@
 python manage.py migrate
 ```
 
 ## Signing In
 
 Before working with Telegram’s API, you need to get your own API ID and hash:
 
-[Login to your Telegram account](https://my.telegram.org/auth) with the phone number of the developer account to use.
-Click under API Development tools.
-A Create new application window will appear. Fill in your application details. There is no need to enter any URL, and only the first two fields (App title and Short name) can currently be changed later.
-Click on Create application at the end. Remember that your API hash is secret and Telegram won’t let you revoke it. Don’t post it anywhere!
+- [Login to your Telegram account](https://my.telegram.org/auth) with the phone number of the developer account to use.
+- Click under API Development tools.
+- Create new application window will appear. Fill in your application details. There is no need to enter any URL, and only the first two fields (App title and Short name) can currently be changed later.
+- Click on Create application at the end. Remember that your API hash is secret and Telegram won’t let you revoke it. Don’t post it anywhere!
 
 ***This API ID and hash is the one used by your application, not your phone number. You can use this API ID and hash with any phone number or even for bot accounts.***
 
 Read more (proxy, bot and etc) [Here](https://docs.telethon.dev/en/stable/basic/signing-in.html).
 
 ## Usage
 
@@ -170,15 +170,15 @@
         try:
             telegram_client.sign_in(phone, code)
         except SessionPasswordNeededError:
             password = input('Enter your password: ')
             telegram_client.sign_in(password=password)    
     ```
 
-#### Doing stuff
+#### Doing stuffs
 
 ```python
 print((await telegram_client.get_me()).stringify())
 
 await telegram_client.send_message('username', 'Hello! Talking to you from Telethon')
 await telegram_client.send_file('username', '/home/myself/Pictures/holidays.jpg')
 
@@ -189,29 +189,29 @@
 @telegram_client.on(telegram_client.NewMessage(pattern='(?i)hi|hello'))
 async def handler(event):
     await event.respond('Hey!')
 ```
 
 ### API
 #### User Login
-1. run the following command to start the server:
+1. Run the following command to start the server:
 
     ```shell script
     python manage.py runserver
     ```
 
-1. run the following command to start telegram client:
+1. Run the following command to start telegram client:
 
     ```shell script
     python manage.py runtelegram
     ```
    
 1. go to [admin panel](http://127.0.0.1:8000/admin/) and [telegram app section](http://127.0.0.1:8000/admin/django_telethon/app/). create a new app. get data from the [your Telegram account](https://my.telegram.org/auth).
 
-1. request code from telegram:
+1. Request code from telegram:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/send-code-request/"
    
@@ -224,15 +224,15 @@
    }
    
    response = requests.request("POST", url, headers=headers, data=payload)
    
    print(response.text)
     ```
 
-1. send this request for sign in:
+1. Send this request for sign in:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/login-user-request/"
    
@@ -249,15 +249,15 @@
    response = requests.request("POST", url, headers=headers, data=payload)
    
    print(response.text)
 
    ```
 
 #### Bot login 
-send this request for sign in:
+Send this request for sign in:
     
    ```python
    import requests
    import json
    
    url = "http://127.0.0.1:8000/telegram/login-bot-request/"
    
@@ -306,15 +306,15 @@
     supervisorctl status
     ```
 
 ## Listen to events
 
 After login telegram client the signal `telegram_client_registered` is emitted. 
 
-1. you can listen to this signal by using the following code for example put this code to your ```receivers.py``` file in app directory:
+1. You can listen to this signal by using the following code for example put this code to your ```receivers.py``` file in app directory:
    
    ```python
    from functools import partial
    
    from django.dispatch import receiver
    from telethon import events
```

### Comparing `django-telethon-1.1.5a1/django_telethon.egg-info/SOURCES.txt` & `django-telethon-1.1.6/django_telethon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5a1/setup.py` & `django-telethon-1.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-telethon',
-    version='1.1.5-alpha.1',
+    version='1.1.6',
     packages=find_packages(),
     include_package_data=True,
     license='BSD License',
     description='Telethon for django',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ali-zahedi/django-telethon',
```

