# Comparing `tmp/lobsang-0.0.2.tar.gz` & `tmp/lobsang-0.0.3.tar.gz`

## Comparing `lobsang-0.0.2.tar` & `lobsang-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lobsang-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lobsang-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lobsang-0.0.2/examples/.env
--rw-r--r--   0        0        0    31185 2020-02-02 00:00:00.000000 lobsang-0.0.2/examples/1_basics.ipynb
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/__init__.py
--rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/chat.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/messages.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/directives/__init__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/directives/base.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/directives/text.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/llms/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/llms/base.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lobsang-0.0.2/lobsang/llms/fake.py
--rw-r--r--   0        0        0    18340 2020-02-02 00:00:00.000000 lobsang-0.0.2/tests/test_chat.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 lobsang-0.0.2/tests/test_directives.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lobsang-0.0.2/tests/test_messages.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lobsang-0.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lobsang-0.0.2/LICENSE
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 lobsang-0.0.2/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lobsang-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 lobsang-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 lobsang-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lobsang-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lobsang-0.0.3/examples/.env
+-rw-r--r--   0        0        0    34218 2020-02-02 00:00:00.000000 lobsang-0.0.3/examples/1_basics.ipynb
+-rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 lobsang-0.0.3/examples/2_directives.ipynb
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/__init__.py
+-rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/chat.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/messages.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/base.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/json.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/text.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/base.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/fake.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/openai.py
+-rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_chat.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_directives.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_llms.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_messages.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lobsang-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lobsang-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 lobsang-0.0.3/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lobsang-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 lobsang-0.0.3/PKG-INFO
```

### Comparing `lobsang-0.0.2/.github/workflows/python-publish.yml` & `lobsang-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/examples/1_basics.ipynb` & `lobsang-0.0.3/examples/1_basics.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9925312020325807%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2023-08-06T16:06:15.866533548Z', 'start_time': '2023-08-06T16:06:14.981240485Z'}}}, "*

 * *            '2: {\'execution_count\': 2, \'outputs\': {0: {\'data\': {\'text/plain\': \'"All set! '*

 * *            '🎉 Let\\\'s get started! 🚀 OPENAI_API_KEY=sk-PbRY4M6AH6Xh..."\'}, \'execution_count\': '*

 * *            "2}}, 'metadata': {'ExecuteTime': {'end_time': '2023-08-06T16:06:16.094116303Z', "*

 * *            "'start_time': '2023- […]*

```diff
@@ -1,17 +1,17 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 1,
             "id": "initial_id",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:10.546104763Z",
-                    "start_time": "2023-08-04T14:33:09.605860709Z"
+                    "end_time": "2023-08-06T16:06:15.866533548Z",
+                    "start_time": "2023-08-06T16:06:14.981240485Z"
                 },
                 "collapsed": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -51,29 +51,29 @@
                 "\n",
                 "In this notebook, we'll cover the basics of lobsang. As a LLM we use OpenAI's \"gpt-3.5-turbo\" model, so you'll need an [OpenAI API key](https://platform.openai.com/account/api-keys) to run this notebook (set it in the cell below).\n",
                 "This is not a free service, but all examples in this notebook should cost less than $0.01 to run. Nevertheless, you should set a [usage limit](https://platform.openai.com/account/billing/limits) to avoid any surprises."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 2,
             "id": "d435b5427783c0ff",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:10.551837136Z",
-                    "start_time": "2023-08-04T14:33:10.548380917Z"
+                    "end_time": "2023-08-06T16:06:16.094116303Z",
+                    "start_time": "2023-08-06T16:06:15.869101627Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "\"All set! \ud83c\udf89 Let's get started! \ud83d\ude80 OPENAI_API_KEY=sk-d45JqOfunEgN...\""
+                        "text/plain": "\"All set! \ud83c\udf89 Let's get started! \ud83d\ude80 OPENAI_API_KEY=sk-PbRY4M6AH6Xh...\""
                     },
-                    "execution_count": 22,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import os\n",
                 "\n",
@@ -106,20 +106,20 @@
                 "1. `SystemMessage` is a special case and is used to set the model's behavior (There should only be one `SystemMessage` per `Chat` instance at the beginning of the conversation.)\n",
                 "1. `UserMessage` is used for messages that are created by the user/developer.\n",
                 "1. `AssistantMessage` is used for messages that are sent generated by the llm."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 3,
             "id": "cfbb7d2b6aee2be7",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:10.599400867Z",
-                    "start_time": "2023-08-04T14:33:10.551911045Z"
+                    "end_time": "2023-08-06T16:06:16.099780826Z",
+                    "start_time": "2023-08-06T16:06:16.095186756Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -175,20 +175,20 @@
                 "## LLM Wrapper\n",
                 "\n",
                 "For experiments and testing, we also provide a FakeLLM which can be imported via `from lobsang.llms import FakeLLM`. However, in this notebook we'll use OpenAI's API. So before we can start chatting, we need to wrap the openai api to make it compatible with lobsang. This can be done with lobsang's `LLM` class as follows:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 4,
             "id": "9c9962d0a47c7842",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:10.600322115Z",
-                    "start_time": "2023-08-04T14:33:10.599099449Z"
+                    "end_time": "2023-08-06T16:06:16.099909218Z",
+                    "start_time": "2023-08-06T16:06:16.097688511Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "class OpenAI(LLM):\n",
                 "    \"\"\"Wrapper for OpenAI API\"\"\"\n",
@@ -220,15 +220,15 @@
         {
             "cell_type": "markdown",
             "id": "15dc69bf8e02d149",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "**Note**: In this example, we return an empty dictionary as the second return value. However, all keys added to the dictionary will end up in the `info` attribute of the corresponding `AssistantMessage` that is created by the chat instance from the response text. This can be used to store additional information about the message. "
+                "**Note**: In this example, we return an empty dictionary as the second return value. However, all keys added to the dictionary will end up in the `info` attribute of the corresponding `AssistantMessage` that is created by the chat instance from the response text. This can be used to store additional information about the message. This is implementation is also provided under `lobsang.llms.openai` and can be imported via `from lobsang import OpenAI`."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5d424b6672d5ade3",
             "metadata": {
                 "collapsed": false
@@ -238,29 +238,29 @@
                 "\n",
                 "Now, let's bring all the pieces together and create a `Chat` instance. In this example, we'll call chat directly with a string, i.e. `chat(\"Ping\")`. \n",
                 "This is equivalent to `chat.run([UserMessage(\"Ping\")])[1]` or `chat.run([\"Ping\"])[1]` (we'll get to the `run` method in a bit), but since this is verbose we provide a shortcut for this common use case with the `__call__` method, i.e. `chat(\"Ping\")`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 5,
             "id": "97382db5b7752f2f",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:11.436319909Z",
-                    "start_time": "2023-08-04T14:33:10.599240445Z"
+                    "end_time": "2023-08-06T16:06:16.787806388Z",
+                    "start_time": "2023-08-06T16:06:16.100273042Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "AssistantMessage(role=assistant, text=Pong! How can I assist you today?, info={'directive': TextDirective, 'query': UserMessage(role=user, text=Ping., info={})})"
+                        "text/plain": "AssistantMessage(role=assistant, text=Pong!, info={'original': 'Pong!', 'directive': TextDirective})"
                     },
-                    "execution_count": 25,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# We first create a chat instance with the LLM wrapper from above\n",
                 "chat = Chat(llm=OpenAI())  # \ud83d\udc48 Note that we don't pass a system message here, so the model will use its default behavior \"You are a helpful assistant.\"\n",
@@ -283,29 +283,37 @@
                 "\n",
                 "Alright, in the next example, we'll initialize the chat instance with a `SystemMessage` to set the model's behavior. \n",
                 "Let's make it a fancy wizard \ud83e\uddd9\u200d\u2642\ufe0f that speaks in a medieval style:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 6,
             "id": "4a9e0b43d1388f94",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:18.274030228Z",
-                    "start_time": "2023-08-04T14:33:11.436706809Z"
+                    "end_time": "2023-08-06T16:06:29.158058406Z",
+                    "start_time": "2023-08-06T16:06:16.784390143Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Ah, good sir/madam, thou hast asked a most difficult question! As a fancy wizard, mine heart doth hold affection for many a spell. Yet, if I must choose but one, I would humbly declare that the enchantment of Teleportation doth hold the highest place of reverence in mine arcane repertoire. 'Tis a spell that doth allow me to traverse great distances in the blink of an eye, traversing the realms with but a whispered incantation. Verily, it is a spell that grants me the power to appear in distant lands, beyond the limits of time and space, and to witness the wonders that lie there. Thus, Teleportation is a spell that fills me with joy and wonder at the possibilities that magic doth offer.\n"
+                        "Ah, dear traveler, thou hath inquired about mine favorite spell! Verily, mine heart doth rejoice at the mention of it. The spell that doth capture mine fancy and ignite the flames of enchantment within my soul is the wondrous incantation known as \"Aurora Borealis.\"\n",
+                        "\n",
+                        "With the power of this spell, I am able to summon the mesmerizing lights of the Northern Sky. Erupting in vibrant hues of azure, emerald, and amethyst, the ethereal display dances across the heavens, filling the night with its celestial majesty.\n",
+                        "\n",
+                        "As I intone the ancient words and weave my hands in intricate gestures, the very fabric of reality bends to my will. Pure magic enlivens the air, swirling and twirling with mystical energy, until the breathtaking splendor of the Aurora Borealis emerges from the mystical realm to grace ours.\n",
+                        "\n",
+                        "This spell, dear interlocutor, serves not only as a magnificent spectacle to behold but also acts as a beacon of hope and wonder to all who witness it. The Aurora Borealis fills the hearts of those who gaze upon it with awe, reminding them of the vastness and beauty of the world, and inspiring them to believe in the limitless possibilities that magic can bring.\n",
+                        "\n",
+                        "Verily, the Aurora Borealis spell is a testament to the grandeur and artistry of the arcane arts, and forever dost it hold a special place in this wizard's heart.\n"
                     ]
                 }
             ],
             "source": [
                 "# First, we need to write a system message that sets the model's behavior\n",
                 "system_message = \"You are a fancy wizard and talk in a medieval style.\"\n",
                 "\n",
@@ -333,30 +341,38 @@
                 "> **Note:** Please note that not all list operations are supported. For example, sorting is not supported. If you are missing a list operation, please open an issue on GitHub. Thanks! \ud83d\ude4f\n",
                 "\n",
                 "\ud83d\udc47 Now, let's take a look at the chat history:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 7,
             "id": "730774f9dea7820",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:18.302082821Z",
-                    "start_time": "2023-08-04T14:33:18.243028094Z"
+                    "end_time": "2023-08-06T16:06:29.171112669Z",
+                    "start_time": "2023-08-06T16:06:29.158642996Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "USER: What is you favourite spell?\n",
-                        "ASSISTANT: Ah, good sir/madam, thou hast asked a most difficult question! As a fancy wizard, mine heart doth hold affection for many a spell. Yet, if I must choose but one, I would humbly declare that the enchantment of Teleportation doth hold the highest place of reverence in mine arcane repertoire. 'Tis a spell that doth allow me to traverse great distances in the blink of an eye, traversing the realms with but a whispered incantation. Verily, it is a spell that grants me the power to appear in distant lands, beyond the limits of time and space, and to witness the wonders that lie there. Thus, Teleportation is a spell that fills me with joy and wonder at the possibilities that magic doth offer.\n"
+                        "ASSISTANT: Ah, dear traveler, thou hath inquired about mine favorite spell! Verily, mine heart doth rejoice at the mention of it. The spell that doth capture mine fancy and ignite the flames of enchantment within my soul is the wondrous incantation known as \"Aurora Borealis.\"\n",
+                        "\n",
+                        "With the power of this spell, I am able to summon the mesmerizing lights of the Northern Sky. Erupting in vibrant hues of azure, emerald, and amethyst, the ethereal display dances across the heavens, filling the night with its celestial majesty.\n",
+                        "\n",
+                        "As I intone the ancient words and weave my hands in intricate gestures, the very fabric of reality bends to my will. Pure magic enlivens the air, swirling and twirling with mystical energy, until the breathtaking splendor of the Aurora Borealis emerges from the mystical realm to grace ours.\n",
+                        "\n",
+                        "This spell, dear interlocutor, serves not only as a magnificent spectacle to behold but also acts as a beacon of hope and wonder to all who witness it. The Aurora Borealis fills the hearts of those who gaze upon it with awe, reminding them of the vastness and beauty of the world, and inspiring them to believe in the limitless possibilities that magic can bring.\n",
+                        "\n",
+                        "Verily, the Aurora Borealis spell is a testament to the grandeur and artistry of the arcane arts, and forever dost it hold a special place in this wizard's heart.\n"
                     ]
                 }
             ],
             "source": [
                 "print(chat)"
             ]
         },
@@ -370,109 +386,125 @@
                 "\u261d\ufe0f As you can see, the chat history contains our previous message and the response from the model.\n",
                 "\n",
                 "\ud83d\udc47 The following shows a selection of supported list operations:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 8,
             "id": "6a031f836fa44b19",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:18.302257220Z",
-                    "start_time": "2023-08-04T14:33:18.243143081Z"
+                    "end_time": "2023-08-06T16:06:29.171373309Z",
+                    "start_time": "2023-08-06T16:06:29.160304612Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "USER: What is you favourite spell?\n",
-                        "ASSISTANT: Ah, good sir/madam, thou hast asked a most difficult question! As a fancy wizard, mine heart doth hold affection for many a spell. Yet, if I must choose but one, I would humbly declare that the enchantment of Teleportation doth hold the highest place of reverence in mine arcane repertoire. 'Tis a spell that doth allow me to traverse great distances in the blink of an eye, traversing the realms with but a whispered incantation. Verily, it is a spell that grants me the power to appear in distant lands, beyond the limits of time and space, and to witness the wonders that lie there. Thus, Teleportation is a spell that fills me with joy and wonder at the possibilities that magic doth offer.\n"
+                        "ASSISTANT: Ah, dear traveler, thou hath inquired about mine favorite spell! Verily, mine heart doth rejoice at the mention of it. The spell that doth capture mine fancy and ignite the flames of enchantment within my soul is the wondrous incantation known as \"Aurora Borealis.\"\n",
+                        "\n",
+                        "With the power of this spell, I am able to summon the mesmerizing lights of the Northern Sky. Erupting in vibrant hues of azure, emerald, and amethyst, the ethereal display dances across the heavens, filling the night with its celestial majesty.\n",
+                        "\n",
+                        "As I intone the ancient words and weave my hands in intricate gestures, the very fabric of reality bends to my will. Pure magic enlivens the air, swirling and twirling with mystical energy, until the breathtaking splendor of the Aurora Borealis emerges from the mystical realm to grace ours.\n",
+                        "\n",
+                        "This spell, dear interlocutor, serves not only as a magnificent spectacle to behold but also acts as a beacon of hope and wonder to all who witness it. The Aurora Borealis fills the hearts of those who gaze upon it with awe, reminding them of the vastness and beauty of the world, and inspiring them to believe in the limitless possibilities that magic can bring.\n",
+                        "\n",
+                        "Verily, the Aurora Borealis spell is a testament to the grandeur and artistry of the arcane arts, and forever dost it hold a special place in this wizard's heart.\n"
                     ]
                 }
             ],
             "source": [
                 "# We can iterate over the chat history\n",
                 "for message in chat:\n",
                 "    print(message)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 9,
             "id": "7506d83894599dff",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:18.302429114Z",
-                    "start_time": "2023-08-04T14:33:18.243204356Z"
+                    "end_time": "2023-08-06T16:06:29.236823923Z",
+                    "start_time": "2023-08-06T16:06:29.162819782Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "2"
                     },
-                    "execution_count": 29,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# We can also get the length of the chat history\n",
                 "len(chat)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 10,
             "id": "e9f94c9839034b92",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:18.302591992Z",
-                    "start_time": "2023-08-04T14:33:18.243278466Z"
+                    "end_time": "2023-08-06T16:06:29.237143684Z",
+                    "start_time": "2023-08-06T16:06:29.209325662Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "UserMessage(role=user, text=What is you favourite spell?, info={})"
+                        "text/plain": "UserMessage(role=user, text=What is you favourite spell?, info={'original': 'What is you favourite spell?', 'directive': TextDirective})"
                     },
-                    "execution_count": 30,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# We can index into it (or slice it, i.e chat[i:j])\n",
                 "chat[0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 11,
             "id": "9a76ed24d38fbe9d",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:18.302730523Z",
-                    "start_time": "2023-08-04T14:33:18.243373866Z"
+                    "end_time": "2023-08-06T16:06:29.237359801Z",
+                    "start_time": "2023-08-06T16:06:29.209530758Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "USER: I'm a new message\n",
-                        "ASSISTANT: Ah, good sir/madam, thou hast asked a most difficult question! As a fancy wizard, mine heart doth hold affection for many a spell. Yet, if I must choose but one, I would humbly declare that the enchantment of Teleportation doth hold the highest place of reverence in mine arcane repertoire. 'Tis a spell that doth allow me to traverse great distances in the blink of an eye, traversing the realms with but a whispered incantation. Verily, it is a spell that grants me the power to appear in distant lands, beyond the limits of time and space, and to witness the wonders that lie there. Thus, Teleportation is a spell that fills me with joy and wonder at the possibilities that magic doth offer.\n"
+                        "ASSISTANT: Ah, dear traveler, thou hath inquired about mine favorite spell! Verily, mine heart doth rejoice at the mention of it. The spell that doth capture mine fancy and ignite the flames of enchantment within my soul is the wondrous incantation known as \"Aurora Borealis.\"\n",
+                        "\n",
+                        "With the power of this spell, I am able to summon the mesmerizing lights of the Northern Sky. Erupting in vibrant hues of azure, emerald, and amethyst, the ethereal display dances across the heavens, filling the night with its celestial majesty.\n",
+                        "\n",
+                        "As I intone the ancient words and weave my hands in intricate gestures, the very fabric of reality bends to my will. Pure magic enlivens the air, swirling and twirling with mystical energy, until the breathtaking splendor of the Aurora Borealis emerges from the mystical realm to grace ours.\n",
+                        "\n",
+                        "This spell, dear interlocutor, serves not only as a magnificent spectacle to behold but also acts as a beacon of hope and wonder to all who witness it. The Aurora Borealis fills the hearts of those who gaze upon it with awe, reminding them of the vastness and beauty of the world, and inspiring them to believe in the limitless possibilities that magic can bring.\n",
+                        "\n",
+                        "Verily, the Aurora Borealis spell is a testament to the grandeur and artistry of the arcane arts, and forever dost it hold a special place in this wizard's heart.\n"
                     ]
                 }
             ],
             "source": [
                 "# and replace messages\n",
                 "chat[0] = UserMessage(\"I'm a new message\")\n",
                 "print(chat)"
@@ -489,29 +521,29 @@
                 "\n",
                 "\ud83d\udc47 Now that we know how to call chat and how to access the chat history, we'll take a look at one more useful feature.\n",
                 "Most of the time you want your message as well as the response automatically added to the chat history. So this is the default behavior of the `Chat` class. However, sometimes you might want to call the model without adding the message to the chat history. For example, if you want to explore variations of a message. For this purpose you can set the `append` flag/parameter to `False` when calling chat: `chat(\"Ping\", append=False)`. This will return the response message without adding anything to the chat history."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 12,
             "id": "7ec7adcb2dd5cd77",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:19.236018648Z",
-                    "start_time": "2023-08-04T14:33:18.243431184Z"
+                    "end_time": "2023-08-06T16:06:30.028440355Z",
+                    "start_time": "2023-08-06T16:06:29.209730534Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Response: The sum of 1+1 is 2.\n",
+                        "Response: 1+1 equals 2.\n",
                         "0\n"
                     ]
                 }
             ],
             "source": [
                 "chat = Chat(llm=OpenAI())\n",
                 "\n",
@@ -519,30 +551,30 @@
                 "\n",
                 "print(\"Response:\", res.text)  \n",
                 "print(len(chat))  # \ud83d\udc48 Will be 0 as we didn't append the message"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 13,
             "id": "16a2ca680d8195",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:19.879085744Z",
-                    "start_time": "2023-08-04T14:33:19.235289753Z"
+                    "end_time": "2023-08-06T16:06:30.807981196Z",
+                    "start_time": "2023-08-06T16:06:30.028103712Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "USER: What is 1+1?\n",
-                        "ASSISTANT: 1+1 equals 2.\n",
+                        "ASSISTANT: 1 + 1 equals 2.\n",
                         "2\n"
                     ]
                 }
             ],
             "source": [
                 "# Now, let's append the message and check the length again\n",
                 "chat(\"What is 1+1?\")\n",
@@ -564,20 +596,20 @@
                 "**Note:** This is a very strict validation, it is therefore not used internally but, for example, can be useful for debugging. Also, invalid chat history can still be used with the `Chat` class. However, it might lead to unexpected behavior.\n",
                 "\n",
                 "Let's check out an example:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 14,
             "id": "91a474621d792966",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:19.890879819Z",
-                    "start_time": "2023-08-04T14:33:19.880753830Z"
+                    "end_time": "2023-08-06T16:06:30.814870754Z",
+                    "start_time": "2023-08-06T16:06:30.810271564Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -599,20 +631,20 @@
                 "    chat.validate()  # \ud83d\udc48 Will raise an error\n",
                 "except Exception as e:\n",
                 "    print(\"Error:\", e)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 15,
             "id": "3696f42af8c4079e",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:19.891030824Z",
-                    "start_time": "2023-08-04T14:33:19.883303679Z"
+                    "end_time": "2023-08-06T16:06:30.815050301Z",
+                    "start_time": "2023-08-06T16:06:30.811815568Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -626,20 +658,20 @@
             "source": [
                 "# Let's take a look at the current chat history (before we fix it)\n",
                 "print(chat)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 16,
             "id": "bd167d1e41e5aace",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:19.891156541Z",
-                    "start_time": "2023-08-04T14:33:19.885304022Z"
+                    "end_time": "2023-08-06T16:06:30.816705053Z",
+                    "start_time": "2023-08-06T16:06:30.813890700Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -674,20 +706,20 @@
                 "In addition, to passing a single message to the `Chat` class, you can also pass a list of messages. For each unanswered message (we'll explain what this means in a second), the `Chat` class will call the model and append the message as well as the response to the conversation which is returned in the end. If the `append` flag/parameter is set to `True` (default), the messages and responses will also be appended to the chat history. \n",
                 "\n",
                 "For this, we can use the `run` method which takes a list of messages and returns the conversation with the messages and responses from the model. Let's take a look:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 17,
             "id": "4cb9752c6b437944",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:21.331545838Z",
-                    "start_time": "2023-08-04T14:33:19.887621613Z"
+                    "end_time": "2023-08-06T16:06:32.880483904Z",
+                    "start_time": "2023-08-06T16:06:30.816083364Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -725,20 +757,20 @@
                 "\u261d\ufe0f As you can see the conversation is a list of messages. The first message is the first user message, followed by our predefined response from the model. The second message is the second user message, followed by the response from the model and so on. \n",
                 "\n",
                 "\ud83d\udc47 If you do not want the example to be part of the conversation you can do the following:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 18,
             "id": "40b34fe4ceeb0f96",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:22.578330622Z",
-                    "start_time": "2023-08-04T14:33:21.332961498Z"
+                    "end_time": "2023-08-06T16:06:34.675824362Z",
+                    "start_time": "2023-08-06T16:06:32.882284671Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -772,20 +804,20 @@
                 "\u261d\ufe0f Now, the example is not part of the conversation anymore. \n",
                 "\n",
                 "\ud83d\udc47 Note that it is part of the chat history though:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 19,
             "id": "82611403a831a802",
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2023-08-04T14:33:22.583577348Z",
-                    "start_time": "2023-08-04T14:33:22.578805628Z"
+                    "end_time": "2023-08-06T16:06:34.685786460Z",
+                    "start_time": "2023-08-06T16:06:34.676446412Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
```

### Comparing `lobsang-0.0.2/lobsang/chat.py` & `lobsang-0.0.3/lobsang/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         system_message = system_message or self.system_message
         response, llm_info = self.llm.chat([system_message, *context])
 
         # Parse response
         parsed_response, directive_info = directive.parse(response)
 
         # Create and return assistant message
-        assistant_info = llm_info | directive_info | {'directive': directive, 'query': query}
+        assistant_info = llm_info | directive_info
         assistant_message = AssistantMessage(parsed_response, info=assistant_info)
         return assistant_message
 
     def __setitem__(self, idx: SupportsIndex, item) -> None:
         """
         Sets an item at a given index in the chat.
```

### Comparing `lobsang-0.0.2/lobsang/messages.py` & `lobsang-0.0.3/lobsang/messages.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/lobsang/directives/__init__.py` & `lobsang-0.0.3/lobsang/directives/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This package contains the directives used to instruct the LLM.
 
-A directive's scope is one user message and it's corresponding response from the LLM.
+A directive's scope is one user message, and it's corresponding response from the LLM.
 The directive embeds a user message with instructions for the LLM to follow.
 Once the LLM generated a response, the directive will parse the response according to the directive's context.
 
 For example, a JSONDirective will embed specific instructions for the LLM to follow and to return a JSON response.
 Since, the LLM only returns text, the JSONDirective will try to parse the response as JSON and return the result.
 """
 
 from lobsang.directives.base import Directive
 from lobsang.directives.text import TextDirective
+from lobsang.directives.json import JSONDirective
```

### Comparing `lobsang-0.0.2/lobsang/directives/text.py` & `lobsang-0.0.3/lobsang/directives/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,25 +5,17 @@
     """
     The text directive. Neither changes the message nor the response but is required to comply with the directive
     interface of lobsang.
 
     This is the default directive in lobsang. Use it if you want a plain text response from the LLM.
     It does not change the corresponding user message (i.e. the message just before the directive in the chat).
     """
+    instructions = "{message}"
 
-    def embed(self, message: str) -> (str, dict):
-        """
-        No embedding is required for the text directive.
-
-        :param message: The message. Will not be changed by the text directive.
-        :return: Tuple (str, dict). The message as-is and an empty info dict.
-        """
-        return message, {}
-
-    def parse(self, response: str) -> (str, dict):
+    def parse(self, response: str, **kwargs) -> (str, dict):
         """
         No parsing is required for the text directive.
 
         :param response: The response from the LLM. Will not be changed by the text directive.
-        :return: Tuple (str, dict). The response as-is and an empty info dict.
+        :return: Tuple (str, dict). The response as-is and dict with additional info.
         """
-        return response, {}
+        return response, self._info(response, **kwargs)
```

### Comparing `lobsang-0.0.2/lobsang/llms/base.py` & `lobsang-0.0.3/lobsang/llms/base.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/lobsang/llms/fake.py` & `lobsang-0.0.3/lobsang/llms/fake.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/tests/test_chat.py` & `lobsang-0.0.3/tests/test_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 from lobsang.llms.fake import FakeLLM
 
 
 class TestDirective(Directive):
     """
     Dummy directive for testing.
     """
+    instructions = "embed {message}"
 
-    def embed(self, message: str) -> (str, dict):
-        return f"embed {message}", {'original': message}
-
-    def parse(self, response: str) -> (str, dict):
-        return f"parse {response}", {'original': response}
+    def parse(self, response: str, **kwargs) -> (str, dict):
+        return f"parse {response}", self._info(response, **kwargs)
 
 
 class TestLLM(FakeLLM):
     """
     Intercepts messages and stores them in a list.
     """
     messages = None
```

### Comparing `lobsang-0.0.2/tests/test_messages.py` & `lobsang-0.0.3/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/LICENSE` & `lobsang-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/README.md` & `lobsang-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.2/pyproject.toml` & `lobsang-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="lobsang"
 description="A simple framework to interact with conversational LLMs"
 keywords =['llm', 'chat', 'framework']
-version="0.0.2"
+version="0.0.3"
 authors = []
 readme="README.md"
 requires-python=">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `lobsang-0.0.2/PKG-INFO` & `lobsang-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobsang
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple framework to interact with conversational LLMs
 Project-URL: Homepage, https://github.com/cereisen/lobsang
 License-File: LICENSE
 Keywords: chat,framework,llm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

