# Comparing `tmp/agixt-1.3.8.tar.gz` & `tmp/agixt-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.3.8.tar", last modified: Tue Jul  4 19:46:50 2023, max compression
+gzip compressed data, was "agixt-1.3.9.tar", last modified: Tue Jul  4 20:33:08 2023, max compression
```

## Comparing `agixt-1.3.8.tar` & `agixt-1.3.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.743451 agixt-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 19:46:38.000000 agixt-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 19:46:38.000000 agixt-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-04 19:46:50.743451 agixt-1.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.731451 agixt-1.3.8/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/DBConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/History.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.731451 agixt-1.3.8/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/Websearch.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.727451 agixt-1.3.8/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.731451 agixt-1.3.8/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/launch-backend.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.735451 agixt-1.3.8/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/agixt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/poe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 19:46:38.000000 agixt-1.3.8/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.731451 agixt-1.3.8/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-04 19:46:50.000000 agixt-1.3.8/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-04 19:46:50.000000 agixt-1.3.8/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:46:50.000000 agixt-1.3.8/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 19:46:50.000000 agixt-1.3.8/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 19:46:50.000000 agixt-1.3.8/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.735451 agixt-1.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.735451 agixt-1.3.8/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/1-Getting started/Screenshots.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.739451 agixt-1.3.8/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Smart Task Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/2-Concepts/Task Chains.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.739451 agixt-1.3.8/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Custom OpenAI Style Provider.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/Poe.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.743451 agixt-1.3.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-04 19:46:38.000000 agixt-1.3.8/docs/images/db.dbdiagram
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 19:46:38.000000 agixt-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 19:46:38.000000 agixt-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:46:50.743451 agixt-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-04 19:46:38.000000 agixt-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:46:50.743451 agixt-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-04 19:46:38.000000 agixt-1.3.8/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 19:46:38.000000 agixt-1.3.8/tests/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)    45872 2023-07-04 19:46:38.000000 agixt-1.3.8/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.670179 agixt-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-04 20:32:51.000000 agixt-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 20:32:51.000000 agixt-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-04 20:33:08.670179 agixt-1.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.658179 agixt-1.3.9/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15071 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/DBConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.658179 agixt-1.3.9/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/Websearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.654179 agixt-1.3.9/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.658179 agixt-1.3.9/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/launch-backend.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.662179 agixt-1.3.9/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/agixt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 20:32:51.000000 agixt-1.3.9/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.658179 agixt-1.3.9/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-04 20:33:08.000000 agixt-1.3.9/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-04 20:33:08.000000 agixt-1.3.9/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:33:08.000000 agixt-1.3.9/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 20:33:08.000000 agixt-1.3.9/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 20:33:08.000000 agixt-1.3.9/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.662179 agixt-1.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.662179 agixt-1.3.9/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.666179 agixt-1.3.9/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Smart Task Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/2-Concepts/Task Chains.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.666179 agixt-1.3.9/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Custom OpenAI Style Provider.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/Poe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.670179 agixt-1.3.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-04 20:32:51.000000 agixt-1.3.9/docs/images/db.dbdiagram
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 20:32:51.000000 agixt-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 20:32:51.000000 agixt-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 20:33:08.670179 agixt-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-04 20:32:51.000000 agixt-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:33:08.670179 agixt-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-04 20:32:51.000000 agixt-1.3.9/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 20:32:51.000000 agixt-1.3.9/tests/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    45872 2023-07-04 20:32:51.000000 agixt-1.3.9/tests/tests.ipynb
```

### Comparing `agixt-1.3.8/LICENSE` & `agixt-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/PKG-INFO` & `agixt-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.3.8
+Version: 1.3.9
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.3.8/agixt/Agent.py` & `agixt-1.3.9/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Chain.py` & `agixt-1.3.9/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/DBConnection.py` & `agixt-1.3.9/agixt/DBConnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             try:
                 engine = create_engine(
                     f"postgresql://{self.username}:{self.password}@{self.server}:{self.port}/{self.database_name}"
                 )
                 engine.execute(f"CREATE DATABASE {self.database_name}")
             except Exception as e:
                 print(f"Error creating database: {e}")
-                raise e
         return engine
 
 
 db = DBConnection()
 
 Base = db.Base
 engine = db.engine
```

### Comparing `agixt-1.3.8/agixt/Embedding.py` & `agixt-1.3.9/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Extensions.py` & `agixt-1.3.9/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/History.py` & `agixt-1.3.9/agixt/History.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Hub.py` & `agixt-1.3.9/agixt/Hub.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Interactions.py` & `agixt-1.3.9/agixt/Interactions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Memories.py` & `agixt-1.3.9/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Prompts.py` & `agixt-1.3.9/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/Websearch.py` & `agixt-1.3.9/agixt/Websearch.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/app.py` & `agixt-1.3.9/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/__init__.py` & `agixt-1.3.9/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/agixt.py` & `agixt-1.3.9/agixt/provider/agixt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/azure.py` & `agixt-1.3.9/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/chatgpt.py` & `agixt-1.3.9/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/claude.py` & `agixt-1.3.9/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/custom.py` & `agixt-1.3.9/agixt/provider/custom.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/fastchat.py` & `agixt-1.3.9/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/gpt4all.py` & `agixt-1.3.9/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/gpt4free.py` & `agixt-1.3.9/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/gpugpt4all.py` & `agixt-1.3.9/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/huggingchat.py` & `agixt-1.3.9/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/huggingface.py` & `agixt-1.3.9/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/kobold.py` & `agixt-1.3.9/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/llamacpp.py` & `agixt-1.3.9/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/llamacppapi.py` & `agixt-1.3.9/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/oobabooga.py` & `agixt-1.3.9/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/openai.py` & `agixt-1.3.9/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/palm.py` & `agixt-1.3.9/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/poe.py` & `agixt-1.3.9/agixt/provider/poe.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/runpod.py` & `agixt-1.3.9/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt/provider/transformer.py` & `agixt-1.3.9/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/agixt.egg-info/PKG-INFO` & `agixt-1.3.9/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.3.8
+Version: 1.3.9
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.3.8/agixt.egg-info/SOURCES.txt` & `agixt-1.3.9/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/1-Getting started/Quick Start.md` & `agixt-1.3.9/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/1-Getting started/Screenshots.md` & `agixt-1.3.9/docs/1-Getting started/Screenshots.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/1-Getting started/Support.md` & `agixt-1.3.9/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.3.9/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Agents.md` & `agixt-1.3.9/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Chains.md` & `agixt-1.3.9/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Chat.md` & `agixt-1.3.9/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Commands.md` & `agixt-1.3.9/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Instructions.md` & `agixt-1.3.9/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Prompts.md` & `agixt-1.3.9/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Smart Chat.md` & `agixt-1.3.9/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Smart Instruct.md` & `agixt-1.3.9/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Smart Task Chains.md` & `agixt-1.3.9/docs/2-Concepts/Smart Task Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/2-Concepts/Task Chains.md` & `agixt-1.3.9/docs/2-Concepts/Task Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Anthropic Claude.md` & `agixt-1.3.9/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Azure OpenAI.md` & `agixt-1.3.9/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/ChatGPT.md` & `agixt-1.3.9/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Custom OpenAI Style Provider.md` & `agixt-1.3.9/docs/3-Providers/Custom OpenAI Style Provider.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/FastChat.md` & `agixt-1.3.9/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.3.9/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/GPT4ALL.md` & `agixt-1.3.9/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/GPT4Free.md` & `agixt-1.3.9/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Google Bard.md` & `agixt-1.3.9/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.3.9/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/HuggingChat.md` & `agixt-1.3.9/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Microsoft Bing.md` & `agixt-1.3.9/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.3.9/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/OpenAI.md` & `agixt-1.3.9/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/Poe.md` & `agixt-1.3.9/docs/3-Providers/Poe.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/llamacpp API.md` & `agixt-1.3.9/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/3-Providers/llamacpp.md` & `agixt-1.3.9/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/README.md` & `agixt-1.3.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.3.9/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/AGiXT-gradient-light.svg` & `agixt-1.3.9/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/AGiXT.png` & `agixt-1.3.9/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/AGiXT.svg` & `agixt-1.3.9/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.3.9/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/AGiXTwhiteborder.svg` & `agixt-1.3.9/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.3.9/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/Smart Instruct.drawio` & `agixt-1.3.9/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/Smart Instruct.drawio.svg` & `agixt-1.3.9/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/Smart Tasks.drawio` & `agixt-1.3.9/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/Smart Tasks.drawio.svg` & `agixt-1.3.9/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/Untitled Diagram.drawio` & `agixt-1.3.9/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/docs/images/db.dbdiagram` & `agixt-1.3.9/docs/images/db.dbdiagram`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/setup.py` & `agixt-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/tests/test-commands.ipynb` & `agixt-1.3.9/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.3.8/tests/tests.ipynb` & `agixt-1.3.9/tests/tests.ipynb`

 * *Files identical despite different names*

