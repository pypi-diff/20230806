# Comparing `tmp/mutual-0.3.4.tar.gz` & `tmp/mutual-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.3.4.tar", last modified: Fri Aug  4 07:47:28 2023, max compression
+gzip compressed data, was "mutual-0.4.0.tar", last modified: Sun Aug  6 15:45:03 2023, max compression
```

## Comparing `mutual-0.3.4.tar` & `mutual-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.636569 mutual-0.3.4/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.4/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-08-04 07:47:28.636284 mutual-0.3.4/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     8420 2023-07-30 03:58:16.000000 mutual-0.3.4/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.631289 mutual-0.3.4/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)     4340 2023-08-04 07:44:12.000000 mutual-0.3.4/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.635807 mutual-0.3.4/mutual/api_resources/
--rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-08-02 06:46:48.000000 mutual-0.3.4/mutual/api_resources/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    13226 2023-08-04 07:25:46.000000 mutual-0.3.4/mutual/api_resources/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4988 2023-08-04 07:23:14.000000 mutual-0.3.4/mutual/api_resources/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.4/mutual/api_resources/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.4/mutual/api_resources/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.4/mutual/api_resources/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.4/mutual/api_resources/Material.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.3.4/mutual/api_resources/Memory.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.4/mutual/api_resources/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      358 2023-08-04 02:43:31.000000 mutual-0.3.4/mutual/api_resources/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-04 07:47:28.632469 mutual-0.3.4/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      509 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-08-04 07:47:28.000000 mutual-0.3.4/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-08-04 07:47:28.636623 mutual-0.3.4/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-08-04 07:45:56.000000 mutual-0.3.4/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.581399 mutual-0.4.0/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.4.0/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)    10128 2023-08-06 15:45:03.581136 mutual-0.4.0/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     9701 2023-08-06 15:41:03.000000 mutual-0.4.0/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.576717 mutual-0.4.0/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4365 2023-08-06 15:33:15.000000 mutual-0.4.0/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.580787 mutual-0.4.0/mutual/api_resources/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-08-02 06:46:48.000000 mutual-0.4.0/mutual/api_resources/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    14003 2023-08-06 15:33:02.000000 mutual-0.4.0/mutual/api_resources/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4988 2023-08-04 07:23:14.000000 mutual-0.4.0/mutual/api_resources/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.4.0/mutual/api_resources/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.4.0/mutual/api_resources/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.4.0/mutual/api_resources/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.4.0/mutual/api_resources/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.4.0/mutual/api_resources/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.4.0/mutual/api_resources/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      358 2023-08-04 02:43:31.000000 mutual-0.4.0/mutual/api_resources/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.577632 mutual-0.4.0/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)    10128 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      509 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-08-06 15:45:03.581450 mutual-0.4.0/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-08-06 15:45:00.000000 mutual-0.4.0/setup.py
```

### Comparing `mutual-0.3.4/LICENSE.txt` & `mutual-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/PKG-INFO` & `mutual-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mutual
-Version: 0.3.4
-Summary: A Python client for the Mutual API.
-Home-page: https://github.com/Mutu-AI
-Author: Alex Betita
-Author-email: alexbetita25@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # mutual
 
 A python package to interact with the Mutuai API.
 
 ## Installation
 
 Run `pip install mutual` in the project root directory.
@@ -30,20 +16,24 @@
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 
 ```
 ## Chat.create(parameters)
 ```python
 # bot_name --> uniquely identifies the bot tied to the api_key account holder
 # bot_id --> uniquely identifies the bot accross all bots
 # username --> uniquely identifies person interacting with bot
@@ -58,33 +48,42 @@
 # multiplayer_memory (bool) --> True by default, allows mulitplayer 
 # context_window (int) --> determines context, default 2
 ```
 
 ```python
 # CHAT DEMO
 for message in mutual.Chat.create_demo("Hello"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 
 # BOT Instance
 
 # uses bot name
 alexbot = mutual.create_bot("bot_name") # THIS WILL CREATE A NEW BOT AND IF BOT WITH BOT NAME EXIST WILL RETURN THAT BOT
 for message in alexbot.chat("Hey there", "username"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 
 # can create bot instance passing in these values
 alexbot = mutual.create_bot(bot_name="alexbot", prompt="You are a customer assistant for mutual that provides helpful information") 
 
+# creating a bot with infoboat template
+alexbot = mutual.create_bot(bot_name="alexbot", template="infoboat")
+
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 
 # update using bot instance
 alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # feed bot data
 response = alexbot.feed(source="file_path")
 print(response)
@@ -198,42 +197,50 @@
 # you can import the functions directly like so
 from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey, Memory, Material
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
-for message in mutual.Chat.create_demo("Hello"):
-    json_data = json.loads(message)
-    if index == 0:
-        print(json_data['data']['bot_data']['bot_id'], end='', flush=True)
-        print(json_data['data']['user_data']['username'], end='', flush=True)
-        print(json_data['data']['bot_data']['bot_name'], end='', flush=True)
-    index += 1
-    print(json_data['content'], end='', flush=True)
+for message in mutual.Chat.create_demo("Hello", error_logs=True):
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if index == 0:
+            print(json_data['data']['bot_data']['bot_id'], end='', flush=True)
+            print(json_data['data']['user_data']['username'], end='', flush=True)
+            print(json_data['data']['bot_data']['bot_name'], end='', flush=True)
+        index += 1
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
 for message in mutual.Chat.create_demo("Hello"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 
 alexbot = mutual.create_bot("AlexBot")
 for message in alexbot.chat("hello", username="Alex"):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 ```
 
 # FLOW EXAMPLE
 ```py
 alexbot = mutual.create_bot("AlexbBot2",prompt="You are a customer assistant for mutual that provides helpful information")
 for message in alexbot.chat("hello", username="Alex", flow=True):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 ```
 
 # FEED MEMORY EXAMPLE
 ```py
 alexbot = mutual.fetch_bot("mutual-bot-1")
 
 feed_response = alexbot.feed(source=f"/Users/alexbetita/Documents/Programming/api-agent-package/api-agent/package/agent_info_2_copy.txt")
@@ -243,22 +250,38 @@
 feed_response = alexbot.feed(source=["Alex Betita is a full stack software engineer for Mutual.", "He is also full stack teacher for App Academy"])
 
 print(feed_response)
 
 response = alexbot.view()
 for memory in response['memories']:
     print(memory)
+
+# PDF
+# MAKE SURE TO SET THE TEMPLATE AS infoboat
+alexbot = mutual.create_bot("package_info_boat", template="infoboat")
+alexbot.feed(source='comp_202_syllabus-1.pdf')
 ```
 
 # STREAM OFF EXAMPLE
 ```py
 
 response = alexbot.chat("Hi!", username="Alex", stream=False)
 json_data = json.loads(response)
 print(json_data['content'])
 
 
 for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
-    json_data = json.loads(message)
-    print(json_data['content'], end='', flush=True)
+    if(len(message)>1):
+        json_data = json.loads(message)
+        if json_data['content'] != '[close]':
+            print(json_data['content'], end='', flush=True)
 
 ```
+
+# CLEAR CONVERSATIONS
+```py
+
+alexbot = mutual.fetch_bot("alex_bot")
+response = alexbot.clear_conversations(username='Alex')
+print(response)
+
+```
```

### Comparing `mutual-0.3.4/mutual/__init__.py` & `mutual-0.4.0/mutual/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,20 +47,20 @@
                      mistake, try rephrasing it.
 unnatural_lang_message = Sorry, I'm not sure how to answer that.\nIf you think this is a mistake, try rephrasing it.
 manipulation_message = I'm afraid you might be trying to manipulate me. I can't answer that!\n"
                           If you think this is a mistake, try rephrasing it.
 """
 
 
-def create_bot(bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None):
+def create_bot(bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None, template=None):
     # create new bot instance
     global api_key
     global bot_id
 
-    response = Bot.create_bot(bot_name, prompt, prompt_id, judge_id, judge_message_id, material_id)
+    response = Bot.create_bot(bot_name, prompt, prompt_id, judge_id, judge_message_id, material_id, template)
     if not response['bot_id']:
         print('Failed in creating a bot.')
         raise Exception(f"Something went wrong. Error Message: {response['details']}")
     
     new_bot_instance = Bot.Bot(api_key, response['bot_id'], response['bot_name'], 
                                prompt_id or response['prompt_id'],
                                judge_id or response['judge_id'],
```

### Comparing `mutual-0.3.4/mutual/api_resources/APIKey.py` & `mutual-0.4.0/mutual/api_resources/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/Bot.py` & `mutual-0.4.0/mutual/api_resources/Bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,29 @@
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
 def create_bot(bot_name=None, prompt=None, prompt_id = "default", judge_id="default", 
-            judge_message_id="default", materiald_id="default"):
+            judge_message_id="default", materiald_id="default", template=None):
     
     url = f"{mutual.endpoint}/bots"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "prompt": prompt,
         "prompt_id": prompt_id or "default",
         "judge_id": judge_id or "default",
         "judge_message_id": judge_message_id or "default",
-        "material_id": materiald_id or "default"
+        "material_id": materiald_id or "default",
+        "template": template
     }
     response = requests.post(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
@@ -298,8 +299,26 @@
         else:
             return "The source type is not supported"
 
         # Check the response status code and return the appropriate message
         if response.status_code < 300:
             return response.json()
         else:
-            return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
+            return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
+        
+    def clear_conversations(self, username=None):
+        url = f"{mutual.endpoint}/bots_user/{str(self.bot_id)}"
+
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.api_key}"
+        }
+        data = {
+            "username": username
+        }
+        
+        response = requests.delete(url, data=json.dumps(data), headers=headers)
+        if response.status_code < 300:
+            return response.json()
+        else:
+            self.default_stream_response["content"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+            return self.default_stream_response
```

### Comparing `mutual-0.3.4/mutual/api_resources/Chat.py` & `mutual-0.4.0/mutual/api_resources/Chat.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/Dev.py` & `mutual-0.4.0/mutual/api_resources/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/Judge.py` & `mutual-0.4.0/mutual/api_resources/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/JudgeMessage.py` & `mutual-0.4.0/mutual/api_resources/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/Material.py` & `mutual-0.4.0/mutual/api_resources/Material.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/Memory.py` & `mutual-0.4.0/mutual/api_resources/Memory.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/mutual/api_resources/Prompt.py` & `mutual-0.4.0/mutual/api_resources/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.4/setup.py` & `mutual-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.3.4',  # beta
+    version='0.4.0',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

