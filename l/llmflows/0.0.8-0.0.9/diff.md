# Comparing `tmp/llmflows-0.0.8.tar.gz` & `tmp/llmflows-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.8.tar", last modified: Sat Jul 22 23:42:06 2023, max compression
+gzip compressed data, was "llmflows-0.0.9.tar", last modified: Sun Jul 23 16:10:09 2023, max compression
```

## Comparing `llmflows-0.0.8.tar` & `llmflows-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.741030 llmflows-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-22 23:41:55.000000 llmflows-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-07-22 23:42:06.741030 llmflows-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-22 23:41:55.000000 llmflows-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.733029 llmflows-0.0.8/llmflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.737029 llmflows-0.0.8/llmflows/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/callbacks/async_base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/callbacks/async_functional_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/callbacks/base_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/callbacks/functional_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.737029 llmflows-0.0.8/llmflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/async_base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/async_base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/async_chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/async_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/async_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/base_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/chat_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/functional_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/flows/vectorstore_flowstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.737029 llmflows-0.0.8/llmflows/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/message_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/llms/openai_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.737029 llmflows-0.0.8/llmflows/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/prompts/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.737029 llmflows-0.0.8/llmflows/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/vectorstores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/vectorstores/vector_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-22 23:41:55.000000 llmflows-0.0.8/llmflows/vectorstores/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 23:42:06.733029 llmflows-0.0.8/llmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-07-22 23:42:06.000000 llmflows-0.0.8/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-22 23:42:06.000000 llmflows-0.0.8/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 23:42:06.000000 llmflows-0.0.8/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-22 23:42:06.000000 llmflows-0.0.8/llmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 23:42:06.000000 llmflows-0.0.8/llmflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-22 23:41:55.000000 llmflows-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 23:42:06.741030 llmflows-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.228916 llmflows-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-23 16:09:57.000000 llmflows-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-23 16:10:09.228916 llmflows-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-07-23 16:09:57.000000 llmflows-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.224916 llmflows-0.0.9/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.224916 llmflows-0.0.9/llmflows/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/callbacks/async_base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/callbacks/async_functional_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/callbacks/base_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/callbacks/functional_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.224916 llmflows-0.0.9/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/async_base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/async_base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/async_chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/base_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/chat_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/functional_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/flows/vectorstore_flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.228916 llmflows-0.0.9/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/message_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.228916 llmflows-0.0.9/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.228916 llmflows-0.0.9/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/vectorstores/vector_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-23 16:09:57.000000 llmflows-0.0.9/llmflows/vectorstores/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:10:09.224916 llmflows-0.0.9/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-23 16:10:09.000000 llmflows-0.0.9/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-23 16:10:09.000000 llmflows-0.0.9/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 16:10:09.000000 llmflows-0.0.9/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-23 16:10:09.000000 llmflows-0.0.9/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 16:10:09.000000 llmflows-0.0.9/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-23 16:09:57.000000 llmflows-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 16:10:09.228916 llmflows-0.0.9/setup.cfg
```

### Comparing `llmflows-0.0.8/LICENSE` & `llmflows-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/PKG-INFO` & `llmflows-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c6c 6d66  : 2.1.Name: llmf
 00000020: 6c6f 7773 0a56 6572 7369 6f6e 3a20 302e  lows.Version: 0.
-00000030: 302e 380a 5375 6d6d 6172 793a 204c 4c4d  0.8.Summary: LLM
+00000030: 302e 390a 5375 6d6d 6172 793a 204c 4c4d  0.9.Summary: LLM
 00000040: 466c 6f77 7320 2d20 5369 6d70 6c65 2c20  Flows - Simple, 
 00000050: 4578 706c 6963 6974 2061 6e64 2054 7261  Explicit and Tra
 00000060: 6e73 7061 7265 6e74 204c 4c4d 2041 7070  nsparent LLM App
 00000070: 730a 4175 7468 6f72 3a20 5374 6f79 616e  s.Author: Stoyan
 00000080: 2053 746f 7961 6e6f 760a 5072 6f6a 6563   Stoyanov.Projec
 00000090: 742d 5552 4c3a 2048 6f6d 6570 6167 652c  t-URL: Homepage,
 000000a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
@@ -28,604 +28,621 @@
 000001b0: 203e 3d33 2e39 0a44 6573 6372 6970 7469   >=3.9.Descripti
 000001c0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 000001d0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
 000001e0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
 000001f0: 454e 5345 0a0a 2320 4c4c 4d46 6c6f 7773  ENSE..# LLMFlows
 00000200: 202d 2053 696d 706c 652c 2045 7870 6c69   - Simple, Expli
 00000210: 6369 742c 2061 6e64 2054 7261 6e73 7061  cit, and Transpa
-00000220: 7265 6e74 204c 4c4d 2041 7070 730a 0a3c  rent LLM Apps..<
-00000230: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000240: 3e0a 2020 3c69 6d67 2073 7479 6c65 3d22  >.  <img style="
-00000250: 7769 6474 683a 2038 3025 2220 7372 633d  width: 80%" src=
-00000260: 2264 6f63 732f 6c6c 6d66 6c6f 7773 5f6c  "docs/llmflows_l
-00000270: 6173 745f 6c6f 676f 2e70 6e67 2220 2f3e  ast_logo.png" />
-00000280: 0a3c 2f70 3e0a 0a5b 215b 5477 6974 7465  .</p>..[![Twitte
-00000290: 725d 2868 7474 7073 3a2f 2f69 6d67 2e73  r](https://img.s
-000002a0: 6869 656c 6473 2e69 6f2f 7477 6974 7465  hields.io/twitte
-000002b0: 722f 666f 6c6c 6f77 2f4c 4c4d 466c 6f77  r/follow/LLMFlow
-000002c0: 733f 7374 796c 653d 736f 6369 616c 295d  s?style=social)]
-000002d0: 2868 7474 7073 3a2f 2f74 7769 7474 6572  (https://twitter
-000002e0: 2e63 6f6d 2f4c 4c4d 466c 6f77 7329 0a21  .com/LLMFlows).!
-000002f0: 5b50 796c 696e 7420 776f 726b 666c 6f77  [Pylint workflow
-00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000310: 2e63 6f6d 2f73 746f 7961 6e2d 7374 6f79  .com/stoyan-stoy
-00000320: 616e 6f76 2f6c 6c6d 666c 6f77 2f61 6374  anov/llmflow/act
-00000330: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00000340: 796c 696e 742e 796d 6c2f 6261 6467 652e  ylint.yml/badge.
-00000350: 7376 6729 0a21 5b4c 6963 656e 7365 5d28  svg).![License](
-00000360: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000370: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
-00000380: 6365 6e73 652f 7374 6f79 616e 2d73 746f  cense/stoyan-sto
-00000390: 7961 6e6f 762f 6c6c 6d66 6c6f 7729 0a21  yanov/llmflow).!
-000003a0: 5b50 7950 695d 2868 7474 7073 3a2f 2f69  [PyPi](https://i
-000003b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000003c0: 7069 2f76 2f6c 6c6d 666c 6f77 7329 0a21  pi/v/llmflows).!
-000003d0: 5b53 7461 7273 5d28 6874 7470 733a 2f2f  [Stars](https://
-000003e0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-000003f0: 6974 6875 622f 7374 6172 732f 7374 6f79  ithub/stars/stoy
-00000400: 616e 2d73 746f 7961 6e6f 762f 6c6c 6d66  an-stoyanov/llmf
-00000410: 6c6f 773f 7374 796c 653d 736f 6369 616c  low?style=social
-00000420: 290a 215b 5265 6c65 6173 6520 6461 7465  ).![Release date
+00000220: 7265 6e74 204c 4c4d 2041 7070 730a 3c62  rent LLM Apps.<b
+00000230: 722f 3e0a 3c62 722f 3e0a 3c62 722f 3e0a  r/>.<br/>.<br/>.
+00000240: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000250: 223e 0a20 203c 696d 6720 7374 796c 653d  ">.  <img style=
+00000260: 2277 6964 7468 3a20 3830 2522 2073 7263  "width: 80%" src
+00000270: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000280: 2e63 6f6d 2f73 746f 7961 6e2d 7374 6f79  .com/stoyan-stoy
+00000290: 616e 6f76 2f6c 6c6d 666c 6f77 732f 626c  anov/llmflows/bl
+000002a0: 6f62 2f6d 6169 6e2f 646f 6373 2f6c 6c6d  ob/main/docs/llm
+000002b0: 666c 6f77 735f 6c61 7374 5f6c 6f67 6f2e  flows_last_logo.
+000002c0: 706e 6722 2f3e 0a3c 2f70 3e0a 3c62 722f  png"/>.</p>.<br/
+000002d0: 3e0a 3c62 722f 3e0a 3c62 722f 3e0a 0a5b  >.<br/>.<br/>..[
+000002e0: 215b 5477 6974 7465 725d 2868 7474 7073  ![Twitter](https
+000002f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000300: 6f2f 7477 6974 7465 722f 666f 6c6c 6f77  o/twitter/follow
+00000310: 2f4c 4c4d 466c 6f77 733f 7374 796c 653d  /LLMFlows?style=
+00000320: 736f 6369 616c 295d 2868 7474 7073 3a2f  social)](https:/
+00000330: 2f74 7769 7474 6572 2e63 6f6d 2f4c 4c4d  /twitter.com/LLM
+00000340: 466c 6f77 7329 0a21 5b50 796c 696e 7420  Flows).![Pylint 
+00000350: 776f 726b 666c 6f77 5d28 6874 7470 733a  workflow](https:
+00000360: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746f  //github.com/sto
+00000370: 7961 6e2d 7374 6f79 616e 6f76 2f6c 6c6d  yan-stoyanov/llm
+00000380: 666c 6f77 732f 6163 7469 6f6e 732f 776f  flows/actions/wo
+00000390: 726b 666c 6f77 732f 7079 6c69 6e74 2e79  rkflows/pylint.y
+000003a0: 6d6c 2f62 6164 6765 2e73 7667 290a 215b  ml/badge.svg).![
+000003b0: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+000003c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000003d0: 6769 7468 7562 2f6c 6963 656e 7365 2f73  github/license/s
+000003e0: 746f 7961 6e2d 7374 6f79 616e 6f76 2f6c  toyan-stoyanov/l
+000003f0: 6c6d 666c 6f77 7329 0a21 5b50 7950 695d  lmflows).![PyPi]
+00000400: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000410: 656c 6473 2e69 6f2f 7079 7069 2f76 2f6c  elds.io/pypi/v/l
+00000420: 6c6d 666c 6f77 7329 0a21 5b53 7461 7273  lmflows).![Stars
 00000430: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 00000440: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000450: 7265 6c65 6173 652d 6461 7465 2f73 746f  release-date/sto
-00000460: 7961 6e2d 7374 6f79 616e 6f76 2f6c 6c6d  yan-stoyanov/llm
-00000470: 666c 6f77 3f73 7479 6c65 3d73 6f63 6961  flow?style=socia
-00000480: 6c29 0a0a 446f 6375 6d65 6e74 6174 696f  l)..Documentatio
-00000490: 6e3a 205b 6874 7470 733a 2f2f 7265 6164  n: [https://read
-000004a0: 7468 6564 6f63 732e 6f72 675d 2868 7474  thedocs.org](htt
-000004b0: 7073 3a2f 2f72 6561 6474 6865 646f 6373  ps://readthedocs
-000004c0: 2e6f 7267 2f29 3c62 722f 3e0a 5079 5049  .org/)<br/>.PyPI
-000004d0: 3a20 5b68 7474 7073 3a2f 2f70 7970 692e  : [https://pypi.
-000004e0: 6f72 672f 7072 6f6a 6563 742f 6c6c 6d66  org/project/llmf
-000004f0: 6c6f 7773 5d28 6874 7470 733a 2f2f 7079  lows](https://py
-00000500: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
-00000510: 6c6d 666c 6f77 732f 293c 2f62 723e 0a54  lmflows/)</br>.T
-00000520: 7769 7474 6572 3a20 5b68 7474 7073 3a2f  witter: [https:/
-00000530: 2f74 7769 7474 6572 2e63 6f6d 2f4c 4c4d  /twitter.com/LLM
-00000540: 466c 6f77 735d 2868 7474 7073 3a2f 2f74  Flows](https://t
-00000550: 7769 7474 6572 2e63 6f6d 2f4c 4c4d 466c  witter.com/LLMFl
-00000560: 6f77 7329 3c62 722f 3e0a 5375 6273 7461  ows)<br/>.Substa
-00000570: 636b 3a20 5b68 7474 7073 3a2f 2f6c 6c6d  ck: [https://llm
-00000580: 666c 6f77 732e 7375 6273 7461 636b 2e63  flows.substack.c
-00000590: 6f6d 5d28 6874 7470 733a 2f2f 6c6c 6d66  om](https://llmf
-000005a0: 6c6f 7773 2e73 7562 7374 6163 6b2e 636f  lows.substack.co
-000005b0: 6d2f 293c 6272 2f3e 0a0a 2323 2041 626f  m/)<br/>..## Abo
-000005c0: 7574 0a4c 4c4d 466c 6f77 7320 6973 2061  ut.LLMFlows is a
-000005d0: 2066 7261 6d65 776f 726b 2066 6f72 2062   framework for b
-000005e0: 7569 6c64 696e 6720 7369 6d70 6c65 2c20  uilding simple, 
-000005f0: 6578 706c 6963 6974 2c20 616e 6420 7472  explicit, and tr
-00000600: 616e 7370 6172 656e 7420 4c4c 4d28 4c61  ansparent LLM(La
-00000610: 7267 6520 0a4c 616e 6775 6167 6520 4d6f  rge .Language Mo
-00000620: 6465 6c29 2061 7070 6c69 6361 7469 6f6e  del) application
-00000630: 732e 0a0a 2323 2049 6e73 7461 6c6c 6174  s...## Installat
-00000640: 696f 6e0a 6060 600a 7069 7020 696e 7374  ion.```.pip inst
-00000650: 616c 6c20 6c6c 6d66 6c6f 7773 0a60 6060  all llmflows.```
-00000660: 0a0a 2323 2050 6869 6c6f 736f 7068 790a  ..## Philosophy.
-00000670: 0a23 2323 202a 2a53 696d 706c 652a 2a0a  .### **Simple**.
-00000680: 4f75 7220 676f 616c 2069 7320 746f 2062  Our goal is to b
-00000690: 7569 6c64 2061 2073 696d 706c 652c 2077  uild a simple, w
-000006a0: 656c 6c2d 646f 6375 6d65 6e74 6564 2066  ell-documented f
-000006b0: 7261 6d65 776f 726b 2077 6974 6820 6d69  ramework with mi
-000006c0: 6e69 6d61 6c20 6162 7374 7261 6374 696f  nimal abstractio
-000006d0: 6e73 2074 6861 7420 0a61 6c6c 6f77 2075  ns that .allow u
-000006e0: 7365 7273 2074 6f20 6275 696c 6420 666c  sers to build fl
-000006f0: 6578 6962 6c65 204c 4c4d 2d70 6f77 6572  exible LLM-power
-00000700: 6564 2061 7070 7320 7769 7468 6f75 7420  ed apps without 
-00000710: 636f 6d70 726f 6d69 7369 6e67 206f 6e20  compromising on 
-00000720: 6361 7061 6269 6c69 7469 6573 2e0a 0a23  capabilities...#
-00000730: 2323 202a 2a45 7870 6c69 6369 742a 2a0a  ## **Explicit**.
-00000740: 5765 2077 616e 7420 746f 2063 7265 6174  We want to creat
-00000750: 6520 616e 2065 7870 6c69 6369 7420 4150  e an explicit AP
-00000760: 4920 656e 6162 6c69 6e67 2075 7365 7273  I enabling users
-00000770: 2074 6f20 7772 6974 6520 636c 6561 6e20   to write clean 
-00000780: 616e 6420 7265 6164 6162 6c65 2063 6f64  and readable cod
-00000790: 6520 7768 696c 6520 0a65 6173 696c 7920  e while .easily 
-000007a0: 6372 6561 7469 6e67 2063 6f6d 706c 6578  creating complex
-000007b0: 2066 6c6f 7773 206f 6620 4c4c 4d73 2069   flows of LLMs i
-000007c0: 6e74 6572 6163 7469 6e67 2077 6974 6820  nteracting with 
-000007d0: 6561 6368 206f 7468 6572 2e20 4c4c 4d46  each other. LLMF
-000007e0: 6c6f 7773 2720 636c 6173 7365 7320 0a67  lows' classes .g
-000007f0: 6976 6520 7573 6572 7320 6675 6c6c 2063  ive users full c
-00000800: 6f6e 7472 6f6c 2061 6e64 2064 6f20 6e6f  ontrol and do no
-00000810: 7420 6861 7665 2061 6e79 2068 6964 6465  t have any hidde
-00000820: 6e20 7072 6f6d 7074 7320 6f72 204c 4c4d  n prompts or LLM
-00000830: 2063 616c 6c73 2e20 0a0a 2323 2320 2a2a   calls. ..### **
-00000840: 5472 616e 7370 6172 656e 742a 2a0a 5765  Transparent**.We
-00000850: 2061 696d 2074 6f20 6865 6c70 2075 7365   aim to help use
-00000860: 7273 2068 6176 6520 6675 6c6c 2074 7261  rs have full tra
-00000870: 6e73 7061 7265 6e63 7920 6f6e 2074 6865  nsparency on the
-00000880: 6972 204c 4c4d 2d70 6f77 6572 6564 2061  ir LLM-powered a
-00000890: 7070 7320 6279 2070 726f 7669 6469 6e67  pps by providing
-000008a0: 200a 7472 6163 6561 626c 6520 666c 6f77   .traceable flow
-000008b0: 7320 616e 6420 636f 6d70 6c65 7465 2069  s and complete i
-000008c0: 6e66 6f72 6d61 7469 6f6e 2066 6f72 2065  nformation for e
-000008d0: 6163 6820 6170 7020 636f 6d70 6f6e 656e  ach app componen
-000008e0: 742c 206d 616b 696e 6720 6974 2065 6173  t, making it eas
-000008f0: 7920 746f 200a 6d6f 6e69 746f 722c 206d  y to .monitor, m
-00000900: 6169 6e74 6169 6e2c 2061 6e64 2064 6562  aintain, and deb
-00000910: 7567 2e0a 0a23 2320 4765 7474 696e 6720  ug...## Getting 
-00000920: 5374 6172 7465 640a 2323 2320 4c4c 4d73  Started.### LLMs
-00000930: 0a4c 4c4d 7320 6172 6520 6f6e 6520 6f66  .LLMs are one of
-00000940: 2074 6865 206d 6169 6e20 6162 7374 7261   the main abstra
-00000950: 6374 696f 6e73 2069 6e20 4c4c 4d46 6c6f  ctions in LLMFlo
-00000960: 7773 2e20 4c4c 4d20 636c 6173 7365 7320  ws. LLM classes 
-00000970: 6172 6520 7772 6170 7065 7273 2061 726f  are wrappers aro
-00000980: 756e 6420 4c4c 4d20 0a41 5049 7320 7375  und LLM .APIs su
-00000990: 6368 2061 7320 4f70 656e 4149 2773 2041  ch as OpenAI's A
-000009a0: 5049 732e 2054 6865 7920 7072 6f76 6964  PIs. They provid
-000009b0: 6520 6d65 7468 6f64 7320 666f 7220 636f  e methods for co
-000009c0: 6e66 6967 7572 696e 6720 616e 6420 6361  nfiguring and ca
-000009d0: 6c6c 696e 6720 7468 6573 6520 4150 4973  lling these APIs
-000009e0: 2c20 0a72 6574 7279 696e 6720 6661 696c  , .retrying fail
-000009f0: 6564 2063 616c 6c73 2c20 616e 6420 666f  ed calls, and fo
-00000a00: 726d 6174 7469 6e67 2074 6865 2072 6573  rmatting the res
-00000a10: 706f 6e73 6573 2e0a 0a60 6060 7079 7468  ponses...```pyth
-00000a20: 6f6e 0a66 726f 6d20 6c6c 6d66 6c6f 7773  on.from llmflows
-00000a30: 2e6c 6c6d 7320 696d 706f 7274 204f 7065  .llms import Ope
-00000a40: 6e41 490a 0a6c 6c6d 203d 204f 7065 6e41  nAI..llm = OpenA
-00000a50: 4928 6170 695f 6b65 793d 223c 796f 7572  I(api_key="<your
-00000a60: 2d6f 7065 6e61 692d 6170 692d 6b65 793e  -openai-api-key>
-00000a70: 2229 0a0a 7265 7375 6c74 2c20 6361 6c6c  ")..result, call
-00000a80: 5f64 6174 612c 206d 6f64 656c 5f63 6f6e  _data, model_con
-00000a90: 6669 6720 3d20 6c6c 6d2e 6765 6e65 7261  fig = llm.genera
-00000aa0: 7465 280a 2020 2070 726f 6d70 743d 2247  te(.   prompt="G
-00000ab0: 656e 6572 6174 6520 6120 636f 6f6c 2074  enerate a cool t
-00000ac0: 6974 6c65 2066 6f72 2061 6e20 3830 7320  itle for an 80s 
-00000ad0: 726f 636b 2073 6f6e 6722 0a29 0a60 6060  rock song".).```
-00000ae0: 0a0a 0a23 2323 2050 726f 6d70 7454 656d  ...### PromptTem
-00000af0: 706c 6174 6573 0a54 6865 2060 5072 6f6d  plates.The `Prom
-00000b00: 7074 5465 6d70 6c61 7465 6020 636c 6173  ptTemplate` clas
-00000b10: 7320 616c 6c6f 7773 2075 7320 746f 2063  s allows us to c
-00000b20: 7265 6174 6520 7374 7269 6e67 7320 7769  reate strings wi
-00000b30: 7468 2076 6172 6961 626c 6573 2074 6861  th variables tha
-00000b40: 7420 7765 2063 616e 2066 696c 6c20 0a69  t we can fill .i
-00000b50: 6e20 6479 6e61 6d69 6361 6c6c 7920 6c61  n dynamically la
-00000b60: 7465 7220 6f6e 2e20 4f6e 6365 2061 2070  ter on. Once a p
-00000b70: 726f 6d70 7420 7465 6d70 6c61 7465 206f  rompt template o
-00000b80: 626a 6563 7420 6973 2063 7265 6174 6564  bject is created
-00000b90: 2061 6e20 6163 7475 616c 2070 726f 6d70   an actual promp
-00000ba0: 7420 6361 6e20 0a62 6520 6765 6e65 7261  t can .be genera
-00000bb0: 7465 6420 6279 2070 726f 7669 6469 6e67  ted by providing
-00000bc0: 2074 6865 2072 6571 7569 7265 6420 7661   the required va
-00000bd0: 7269 6162 6c65 732e 0a0a 6060 6070 7974  riables...```pyt
-00000be0: 686f 6e0a 6672 6f6d 206c 6c6d 666c 6f77  hon.from llmflow
-00000bf0: 732e 6c6c 6d73 2069 6d70 6f72 7420 4f70  s.llms import Op
-00000c00: 656e 4149 0a66 726f 6d20 6c6c 6d66 6c6f  enAI.from llmflo
-00000c10: 7773 2e70 726f 6d70 7473 2069 6d70 6f72  ws.prompts impor
-00000c20: 7420 5072 6f6d 7074 5465 6d70 6c61 7465  t PromptTemplate
-00000c30: 0a0a 0a70 726f 6d70 745f 7465 6d70 6c61  ...prompt_templa
-00000c40: 7465 203d 2050 726f 6d70 7454 656d 706c  te = PromptTempl
-00000c50: 6174 6528 0a20 2020 2070 726f 6d70 743d  ate(.    prompt=
-00000c60: 2247 656e 6572 6174 6520 6120 7469 746c  "Generate a titl
-00000c70: 6520 666f 7220 6120 3930 7320 6869 702d  e for a 90s hip-
-00000c80: 686f 7020 736f 6e67 2061 626f 7574 207b  hop song about {
-00000c90: 746f 7069 637d 2e22 0a29 0a6c 6c6d 5f70  topic}.".).llm_p
-00000ca0: 726f 6d70 7420 3d20 7072 6f6d 7074 5f74  rompt = prompt_t
-00000cb0: 656d 706c 6174 652e 6765 745f 7072 6f6d  emplate.get_prom
-00000cc0: 7074 2874 6f70 6963 3d22 6672 6965 6e64  pt(topic="friend
-00000cd0: 7368 6970 2229 0a0a 7072 696e 7428 6c6c  ship")..print(ll
-00000ce0: 6d5f 7072 6f6d 7074 290a 0a6c 6c6d 203d  m_prompt)..llm =
-00000cf0: 204f 7065 6e41 4928 6170 695f 6b65 793d   OpenAI(api_key=
-00000d00: 223c 796f 7572 2d6f 7065 6e61 692d 6170  "<your-openai-ap
-00000d10: 692d 6b65 793e 2229 0a73 6f6e 675f 7469  i-key>").song_ti
-00000d20: 746c 6520 3d20 6c6c 6d2e 6765 6e65 7261  tle = llm.genera
-00000d30: 7465 286c 6c6d 5f70 726f 6d70 7429 0a0a  te(llm_prompt)..
-00000d40: 7072 696e 7428 736f 6e67 5f74 6974 6c65  print(song_title
-00000d50: 290a 6060 600a 0a23 2323 2043 6861 7420  ).```..### Chat 
-00000d60: 4c4c 4d73 0a55 6e6c 696b 6520 7265 6775  LLMs.Unlike regu
-00000d70: 6c61 7220 4c4c 4d73 2074 6861 7420 6f6e  lar LLMs that on
-00000d80: 6c79 2072 6571 7569 7265 2061 2070 726f  ly require a pro
-00000d90: 6d70 7420 746f 2067 656e 6572 6174 6520  mpt to generate 
-00000da0: 7465 7874 2c20 6368 6174 204c 4c4d 7320  text, chat LLMs 
-00000db0: 7265 7175 6972 6520 6120 0a63 6f6e 7665  require a .conve
-00000dc0: 7273 6174 696f 6e20 6869 7374 6f72 792e  rsation history.
-00000dd0: 2054 6865 2063 6f6e 7665 7273 6174 696f   The conversatio
-00000de0: 6e20 6869 7374 6f72 7920 6973 2072 6570  n history is rep
-00000df0: 7265 7365 6e74 6564 200a 6173 2061 206c  resented .as a l
-00000e00: 6973 7420 6f66 206d 6573 7361 6765 7320  ist of messages 
-00000e10: 6265 7477 6565 6e20 6120 7573 6572 2061  between a user a
-00000e20: 6e64 2061 6e20 6173 7369 7374 616e 742e  nd an assistant.
-00000e30: 2054 6869 7320 636f 6e76 6572 7361 7469   This conversati
-00000e40: 6f6e 2068 6973 746f 7279 2069 7320 0a73  on history is .s
-00000e50: 656e 7420 746f 2074 6865 206d 6f64 656c  ent to the model
-00000e60: 2c20 616e 6420 6120 6e65 7720 6d65 7373  , and a new mess
-00000e70: 6167 6520 6973 2067 656e 6572 6174 6564  age is generated
-00000e80: 2062 6173 6564 206f 6e20 6974 2e0a 0a4c   based on it...L
-00000e90: 4c4d 466c 6f77 7320 7072 6f76 6964 6573  LMFlows provides
-00000ea0: 2061 2060 4d65 7373 6167 6548 6973 746f   a `MessageHisto
-00000eb0: 7279 6020 636c 6173 7320 746f 206d 616e  ry` class to man
-00000ec0: 6167 6520 7468 6520 7265 7175 6972 6564  age the required
-00000ed0: 2063 6f6e 7665 7273 6174 696f 6e20 6869   conversation hi
-00000ee0: 7374 6f72 7920 0a66 6f72 2063 6861 7420  story .for chat 
-00000ef0: 4c4c 4d73 2e0a 0a59 6f75 2063 616e 2062  LLMs...You can b
-00000f00: 7569 6c64 2061 2073 696d 706c 6520 6368  uild a simple ch
-00000f10: 6174 626f 7420 6279 2075 7369 6e67 2074  atbot by using t
-00000f20: 6865 2060 4f70 656e 4149 4368 6174 6020  he `OpenAIChat` 
-00000f30: 616e 6420 604d 6573 7361 6765 4869 7374  and `MessageHist
-00000f40: 6f72 7960 2063 6c61 7373 6573 3a0a 0a60  ory` classes:..`
-00000f50: 6060 7079 7468 6f6e 0a66 726f 6d20 6c6c  ``python.from ll
-00000f60: 6d66 6c6f 7773 2e6c 6c6d 7320 696d 706f  mflows.llms impo
-00000f70: 7274 204f 7065 6e41 4943 6861 742c 204d  rt OpenAIChat, M
-00000f80: 6573 7361 6765 4869 7374 6f72 790a 0a6c  essageHistory..l
-00000f90: 6c6d 203d 204f 7065 6e41 4943 6861 7428  lm = OpenAIChat(
-00000fa0: 6170 695f 6b65 793d 223c 796f 7572 2d6f  api_key="<your-o
-00000fb0: 7065 6e61 692d 6170 692d 6b65 793e 2229  penai-api-key>")
-00000fc0: 0a6d 6573 7361 6765 5f68 6973 746f 7279  .message_history
-00000fd0: 203d 204d 6573 7361 6765 4869 7374 6f72   = MessageHistor
-00000fe0: 7928 290a 0a77 6869 6c65 2054 7275 653a  y()..while True:
-00000ff0: 0a20 2020 2075 7365 725f 6d65 7373 6167  .    user_messag
-00001000: 6520 3d20 696e 7075 7428 2259 6f75 3a22  e = input("You:"
-00001010: 290a 2020 2020 6d65 7373 6167 655f 6869  ).    message_hi
-00001020: 7374 6f72 792e 6164 645f 7573 6572 5f6d  story.add_user_m
-00001030: 6573 7361 6765 2875 7365 725f 6d65 7373  essage(user_mess
-00001040: 6167 6529 0a0a 2020 2020 6c6c 6d5f 7265  age)..    llm_re
-00001050: 7370 6f6e 7365 2c20 6361 6c6c 5f64 6174  sponse, call_dat
-00001060: 612c 206d 6f64 656c 5f63 6f6e 6669 6720  a, model_config 
-00001070: 3d20 6c6c 6d2e 6765 6e65 7261 7465 286d  = llm.generate(m
-00001080: 6573 7361 6765 5f68 6973 746f 7279 290a  essage_history).
-00001090: 2020 2020 6d65 7373 6167 655f 6869 7374      message_hist
-000010a0: 6f72 792e 6164 645f 6169 5f6d 6573 7361  ory.add_ai_messa
-000010b0: 6765 286c 6c6d 5f72 6573 706f 6e73 6529  ge(llm_response)
-000010c0: 0a0a 2020 2020 7072 696e 7428 6622 4c4c  ..    print(f"LL
-000010d0: 4d3a 207b 6c6c 6d5f 7265 7370 6f6e 7365  M: {llm_response
-000010e0: 7d22 290a 6060 600a 0a23 2323 204c 4c4d  }").```..### LLM
-000010f0: 2046 6c6f 7773 0a4f 6674 656e 2074 696d   Flows.Often tim
-00001100: 6573 2c20 7265 616c 2d77 6f72 6c64 2061  es, real-world a
-00001110: 7070 6c69 6361 7469 6f6e 7320 6361 6e20  pplications can 
-00001120: 6265 206d 6f72 6520 636f 6d70 6c65 7820  be more complex 
-00001130: 616e 6420 6361 6e20 6861 7665 2064 6570  and can have dep
-00001140: 656e 6465 6e63 6965 7320 0a62 6574 7765  endencies .betwe
-00001150: 656e 2070 726f 6d70 7473 2061 6e64 204c  en prompts and L
-00001160: 4c4d 2063 616c 6c73 2e20 466f 7220 6578  LM calls. For ex
-00001170: 616d 706c 653a 0a0a 215b 436f 6d70 6c65  ample:..![Comple
-00001180: 7820 666c 6f77 5d28 646f 6373 2f63 6f6d  x flow](docs/com
-00001190: 706c 6578 5f66 6c6f 772e 706e 6729 0a0a  plex_flow.png)..
-000011a0: 5768 656e 2079 6f75 2077 616e 7420 746f  When you want to
-000011b0: 2062 7569 6c64 2061 7070 7320 7769 7468   build apps with
-000011c0: 2063 6f6d 706c 6578 2064 6570 656e 6465   complex depende
-000011d0: 6e63 6965 7320 796f 7520 6361 6e20 7573  ncies you can us
-000011e0: 6520 7468 6520 6046 6c6f 7760 2061 6e64  e the `Flow` and
-000011f0: 200a 6046 6c6f 7773 7465 7060 2063 6c61   .`Flowstep` cla
-00001200: 7373 6573 2e20 4c4c 4d46 6c6f 7773 2077  sses. LLMFlows w
-00001210: 696c 6c20 6669 6775 7265 206f 7574 2074  ill figure out t
-00001220: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
-00001230: 616e 6420 6d61 6b65 2073 7572 6520 6561  and make sure ea
-00001240: 6368 200a 666c 6f77 7374 6570 2072 756e  ch .flowstep run
-00001250: 7320 6f6e 6c79 2077 6865 6e20 616c 6c20  s only when all 
-00001260: 6974 7320 6465 7065 6e64 656e 6369 6573  its dependencies
-00001270: 2061 7265 206d 6574 3a0a 0a60 6060 7079   are met:..```py
-00001280: 7468 6f6e 0a66 726f 6d20 6c6c 6d66 6c6f  thon.from llmflo
-00001290: 7773 2e66 6c6f 7773 2069 6d70 6f72 7420  ws.flows import 
-000012a0: 466c 6f77 2c20 466c 6f77 5374 6570 0a66  Flow, FlowStep.f
-000012b0: 726f 6d20 6c6c 6d66 6c6f 7773 2e6c 6c6d  rom llmflows.llm
-000012c0: 7320 696d 706f 7274 204f 7065 6e41 490a  s import OpenAI.
-000012d0: 6672 6f6d 206c 6c6d 666c 6f77 732e 7072  from llmflows.pr
-000012e0: 6f6d 7074 7320 696d 706f 7274 2050 726f  ompts import Pro
-000012f0: 6d70 7454 656d 706c 6174 650a 0a6f 7065  mptTemplate..ope
-00001300: 6e61 695f 6c6c 6d20 3d20 4f70 656e 4149  nai_llm = OpenAI
-00001310: 2861 7069 5f6b 6579 3d22 3c79 6f75 722d  (api_key="<your-
-00001320: 6f70 656e 6169 2d61 7069 2d6b 6579 3e22  openai-api-key>"
-00001330: 290a 0a23 2043 7265 6174 6520 7072 6f6d  )..# Create prom
-00001340: 7074 2074 656d 706c 6174 6573 0a74 6974  pt templates.tit
-00001350: 6c65 5f74 656d 706c 6174 6520 3d20 5072  le_template = Pr
-00001360: 6f6d 7074 5465 6d70 6c61 7465 2822 5768  omptTemplate("Wh
-00001370: 6174 2069 7320 6120 676f 6f64 2074 6974  at is a good tit
-00001380: 6c65 206f 6620 6120 6d6f 7669 6520 6162  le of a movie ab
-00001390: 6f75 7420 7b74 6f70 6963 7d3f 2229 0a73  out {topic}?").s
-000013a0: 6f6e 675f 7465 6d70 6c61 7465 203d 2050  ong_template = P
-000013b0: 726f 6d70 7454 656d 706c 6174 6528 0a20  romptTemplate(. 
-000013c0: 2020 2022 5768 6174 2069 7320 6120 676f     "What is a go
-000013d0: 6f64 2073 6f6e 6720 7469 746c 6520 6f66  od song title of
-000013e0: 2061 2073 6f75 6e64 7472 6163 6b20 666f   a soundtrack fo
-000013f0: 7220 6120 6d6f 7669 6520 6361 6c6c 6564  r a movie called
-00001400: 207b 6d6f 7669 655f 7469 746c 657d 3f22   {movie_title}?"
-00001410: 0a29 0a63 6861 7261 6374 6572 735f 7465  .).characters_te
-00001420: 6d70 6c61 7465 203d 2050 726f 6d70 7454  mplate = PromptT
-00001430: 656d 706c 6174 6528 0a20 2020 2022 5768  emplate(.    "Wh
-00001440: 6174 2061 7265 2074 776f 206d 6169 6e20  at are two main 
-00001450: 6368 6172 6163 7465 7273 2066 6f72 2061  characters for a
-00001460: 206d 6f76 6965 2063 616c 6c65 6420 7b6d   movie called {m
-00001470: 6f76 6965 5f74 6974 6c65 7d3f 220a 290a  ovie_title}?".).
-00001480: 6c79 7269 6373 5f74 656d 706c 6174 6520  lyrics_template 
-00001490: 3d20 5072 6f6d 7074 5465 6d70 6c61 7465  = PromptTemplate
-000014a0: 280a 2020 2020 2257 7269 7465 206c 7972  (.    "Write lyr
-000014b0: 6963 7320 6f66 2061 206d 6f76 6965 2073  ics of a movie s
-000014c0: 6f6e 6720 6361 6c6c 6564 207b 736f 6e67  ong called {song
-000014d0: 5f74 6974 6c65 7d2e 2054 6865 206d 6169  _title}. The mai
-000014e0: 6e20 6368 6172 6163 7465 7273 2061 7265  n characters are
-000014f0: 2022 0a20 2020 2022 7b6d 6169 6e5f 6368   ".    "{main_ch
-00001500: 6172 6163 7465 7273 7d22 0a29 0a0a 2320  aracters}".)..# 
-00001510: 4372 6561 7465 2066 6c6f 7773 7465 7073  Create flowsteps
-00001520: 0a6d 6f76 6965 5f74 6974 6c65 5f66 6c6f  .movie_title_flo
-00001530: 7773 7465 7020 3d20 466c 6f77 5374 6570  wstep = FlowStep
-00001540: 280a 2020 2020 6e61 6d65 3d22 4d6f 7669  (.    name="Movi
-00001550: 6520 5469 746c 6520 466c 6f77 7374 6570  e Title Flowstep
-00001560: 222c 0a20 2020 206c 6c6d 3d6f 7065 6e61  ",.    llm=opena
-00001570: 695f 6c6c 6d2c 0a20 2020 2070 726f 6d70  i_llm,.    promp
-00001580: 745f 7465 6d70 6c61 7465 3d74 6974 6c65  t_template=title
-00001590: 5f74 656d 706c 6174 652c 0a20 2020 206f  _template,.    o
-000015a0: 7574 7075 745f 6b65 793d 226d 6f76 6965  utput_key="movie
-000015b0: 5f74 6974 6c65 222c 0a29 0a0a 736f 6e67  _title",.)..song
-000015c0: 5f74 6974 6c65 5f66 6c6f 7773 7465 7020  _title_flowstep 
-000015d0: 3d20 466c 6f77 5374 6570 280a 2020 2020  = FlowStep(.    
-000015e0: 6e61 6d65 3d22 536f 6e67 2054 6974 6c65  name="Song Title
-000015f0: 2046 6c6f 7773 7465 7022 2c0a 2020 2020   Flowstep",.    
-00001600: 6c6c 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a  llm=openai_llm,.
-00001610: 2020 2020 7072 6f6d 7074 5f74 656d 706c      prompt_templ
-00001620: 6174 653d 736f 6e67 5f74 656d 706c 6174  ate=song_templat
-00001630: 652c 0a20 2020 206f 7574 7075 745f 6b65  e,.    output_ke
-00001640: 793d 2273 6f6e 675f 7469 746c 6522 2c0a  y="song_title",.
-00001650: 290a 0a63 6861 7261 6374 6572 735f 666c  )..characters_fl
-00001660: 6f77 7374 6570 203d 2046 6c6f 7753 7465  owstep = FlowSte
-00001670: 7028 0a20 2020 206e 616d 653d 2243 6861  p(.    name="Cha
-00001680: 7261 6374 6572 7320 466c 6f77 7374 6570  racters Flowstep
-00001690: 222c 0a20 2020 206c 6c6d 3d6f 7065 6e61  ",.    llm=opena
-000016a0: 695f 6c6c 6d2c 0a20 2020 2070 726f 6d70  i_llm,.    promp
-000016b0: 745f 7465 6d70 6c61 7465 3d63 6861 7261  t_template=chara
-000016c0: 6374 6572 735f 7465 6d70 6c61 7465 2c0a  cters_template,.
-000016d0: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
-000016e0: 6d61 696e 5f63 6861 7261 6374 6572 7322  main_characters"
-000016f0: 2c0a 290a 0a73 6f6e 675f 6c79 7269 6373  ,.)..song_lyrics
-00001700: 5f66 6c6f 7773 7465 7020 3d20 466c 6f77  _flowstep = Flow
-00001710: 5374 6570 280a 2020 2020 6e61 6d65 3d22  Step(.    name="
-00001720: 536f 6e67 204c 7972 6963 7320 466c 6f77  Song Lyrics Flow
-00001730: 7374 6570 222c 0a20 2020 206c 6c6d 3d6f  step",.    llm=o
-00001740: 7065 6e61 695f 6c6c 6d2c 0a20 2020 2070  penai_llm,.    p
-00001750: 726f 6d70 745f 7465 6d70 6c61 7465 3d6c  rompt_template=l
-00001760: 7972 6963 735f 7465 6d70 6c61 7465 2c0a  yrics_template,.
-00001770: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
-00001780: 736f 6e67 5f6c 7972 6963 7322 2c0a 290a  song_lyrics",.).
-00001790: 0a23 2043 6f6e 6e65 6374 2066 6c6f 7773  .# Connect flows
-000017a0: 7465 7073 0a6d 6f76 6965 5f74 6974 6c65  teps.movie_title
-000017b0: 5f66 6c6f 7773 7465 702e 636f 6e6e 6563  _flowstep.connec
-000017c0: 7428 736f 6e67 5f74 6974 6c65 5f66 6c6f  t(song_title_flo
-000017d0: 7773 7465 702c 2063 6861 7261 6374 6572  wstep, character
-000017e0: 735f 666c 6f77 7374 6570 2c20 736f 6e67  s_flowstep, song
-000017f0: 5f6c 7972 6963 735f 666c 6f77 7374 6570  _lyrics_flowstep
-00001800: 290a 736f 6e67 5f74 6974 6c65 5f66 6c6f  ).song_title_flo
-00001810: 7773 7465 702e 636f 6e6e 6563 7428 736f  wstep.connect(so
-00001820: 6e67 5f6c 7972 6963 735f 666c 6f77 7374  ng_lyrics_flowst
-00001830: 6570 290a 6368 6172 6163 7465 7273 5f66  ep).characters_f
-00001840: 6c6f 7773 7465 702e 636f 6e6e 6563 7428  lowstep.connect(
-00001850: 736f 6e67 5f6c 7972 6963 735f 666c 6f77  song_lyrics_flow
-00001860: 7374 6570 290a 0a23 2043 7265 6174 6520  step)..# Create 
-00001870: 616e 6420 7275 6e20 466c 6f77 0a73 6f75  and run Flow.sou
-00001880: 6e64 7472 6163 6b5f 666c 6f77 203d 2046  ndtrack_flow = F
-00001890: 6c6f 7728 7469 746c 655f 666c 6f77 7374  low(title_flowst
-000018a0: 6570 290a 7265 7375 6c74 7320 3d20 736f  ep).results = so
-000018b0: 756e 6474 7261 636b 5f66 6c6f 772e 7374  undtrack_flow.st
-000018c0: 6172 7428 746f 7069 633d 2266 7269 656e  art(topic="frien
-000018d0: 6473 6869 7022 2c20 7665 7262 6f73 653d  dship", verbose=
-000018e0: 5472 7565 290a 6060 600a 0a23 2323 2041  True).```..### A
-000018f0: 7379 6e63 2046 6c6f 7773 0a53 6f6d 6574  sync Flows.Somet
-00001900: 696d 6573 206d 756c 7469 706c 6520 666c  imes multiple fl
-00001910: 6f77 2073 7465 7073 2063 616e 2072 756e  ow steps can run
-00001920: 2069 6e20 7061 7261 6c6c 656c 2069 6620   in parallel if 
-00001930: 616c 6c20 7468 6569 7220 6465 7065 6e64  all their depend
-00001940: 656e 6369 6573 2061 7265 206d 6574 2e20  encies are met. 
-00001950: 0a46 6f72 2063 6173 6573 206c 696b 6520  .For cases like 
-00001960: 7468 6973 2c20 4c4c 4d46 6c6f 7773 2070  this, LLMFlows p
-00001970: 726f 7669 6465 7320 6173 796e 6320 636c  rovides async cl
-00001980: 6173 7365 7320 746f 2069 6d70 726f 7665  asses to improve
-00001990: 2074 6865 2072 756e 7469 6d65 206f 6620   the runtime of 
-000019a0: 616e 7920 0a63 6f6d 706c 6578 2066 6c6f  any .complex flo
-000019b0: 7720 6279 2072 756e 6e69 6e67 2066 6c6f  w by running flo
-000019c0: 7720 7374 6570 7320 7468 6174 2061 6c72  w steps that alr
-000019d0: 6561 6479 2068 6176 6520 616c 6c20 7468  eady have all th
-000019e0: 6569 7220 7265 7175 6972 6564 2069 6e70  eir required inp
-000019f0: 7574 7320 696e 200a 7061 7261 6c6c 656c  uts in .parallel
-00001a00: 2e0a 0a60 6060 7079 7468 6f6e 0a0a 2e2e  ...```python....
-00001a10: 2e0a 0a6d 6f76 6965 5f74 6974 6c65 5f66  ...movie_title_f
-00001a20: 6c6f 7773 7465 7020 3d20 4173 796e 6346  lowstep = AsyncF
-00001a30: 6c6f 7753 7465 7028 0a20 2020 206e 616d  lowStep(.    nam
-00001a40: 653d 2246 6c6f 7773 7465 7020 3122 2c0a  e="Flowstep 1",.
-00001a50: 2020 2020 6c6c 6d3d 6f70 656e 6169 5f6c      llm=openai_l
-00001a60: 6c6d 2c0a 2020 2020 7072 6f6d 7074 5f74  lm,.    prompt_t
-00001a70: 656d 706c 6174 653d 7469 746c 655f 7465  emplate=title_te
-00001a80: 6d70 6c61 7465 2c0a 2020 2020 6f75 7470  mplate,.    outp
-00001a90: 7574 5f6b 6579 3d22 6d6f 7669 655f 7469  ut_key="movie_ti
-00001aa0: 746c 6522 2c0a 290a 0a73 6f6e 675f 7469  tle",.)..song_ti
-00001ab0: 746c 655f 666c 6f77 7374 6570 203d 2046  tle_flowstep = F
-00001ac0: 6c6f 7753 7465 7028 0a20 2020 206e 616d  lowStep(.    nam
-00001ad0: 653d 2246 6c6f 7773 7465 7020 3222 2c0a  e="Flowstep 2",.
-00001ae0: 2020 2020 6c6c 6d3d 6f70 656e 6169 5f6c      llm=openai_l
-00001af0: 6c6d 2c0a 2020 2020 7072 6f6d 7074 5f74  lm,.    prompt_t
-00001b00: 656d 706c 6174 653d 736f 6e67 5f74 656d  emplate=song_tem
-00001b10: 706c 6174 652c 0a20 2020 206f 7574 7075  plate,.    outpu
-00001b20: 745f 6b65 793d 2273 6f6e 675f 7469 746c  t_key="song_titl
-00001b30: 6522 2c0a 290a 0a63 6861 7261 6374 6572  e",.)..character
-00001b40: 735f 666c 6f77 7374 6570 203d 2041 7379  s_flowstep = Asy
-00001b50: 6e63 466c 6f77 5374 6570 280a 2020 2020  ncFlowStep(.    
-00001b60: 6e61 6d65 3d22 466c 6f77 7374 6570 2033  name="Flowstep 3
-00001b70: 222c 0a20 2020 206c 6c6d 3d6f 7065 6e61  ",.    llm=opena
-00001b80: 695f 6c6c 6d2c 0a20 2020 2070 726f 6d70  i_llm,.    promp
-00001b90: 745f 7465 6d70 6c61 7465 3d63 6861 7261  t_template=chara
-00001ba0: 6374 6572 735f 7465 6d70 6c61 7465 2c0a  cters_template,.
-00001bb0: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
-00001bc0: 6d61 696e 5f63 6861 7261 6374 6572 7322  main_characters"
-00001bd0: 2c0a 290a 0a73 6f6e 675f 6c79 7269 6373  ,.)..song_lyrics
-00001be0: 5f66 6c6f 7773 7465 7020 3d20 4173 796e  _flowstep = Asyn
-00001bf0: 6346 6c6f 7753 7465 7028 0a20 2020 206e  cFlowStep(.    n
-00001c00: 616d 653d 2246 6c6f 7773 7465 7020 3422  ame="Flowstep 4"
-00001c10: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
-00001c20: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
-00001c30: 5f74 656d 706c 6174 653d 6c79 7269 6373  _template=lyrics
-00001c40: 5f74 656d 706c 6174 652c 0a20 2020 206f  _template,.    o
-00001c50: 7574 7075 745f 6b65 793d 2273 6f6e 675f  utput_key="song_
-00001c60: 6c79 7269 6373 222c 0a29 0a0a 2e2e 2e0a  lyrics",.)......
-00001c70: 0a60 6060 0a0a 4368 6563 6b20 6f75 7220  .```..Check our 
-00001c80: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00001c90: 7220 6d6f 7265 2065 7861 6d70 6c65 732c  r more examples,
-00001ca0: 2073 7563 6820 6173 2069 6e74 6567 7261   such as integra
-00001cb0: 7469 6e67 2076 6563 746f 7220 6461 7461  ting vector data
-00001cc0: 6261 7365 732c 200a 6372 6561 7469 6e67  bases, .creating
-00001cd0: 2071 7565 7374 696f 6e2d 616e 7377 6572   question-answer
-00001ce0: 696e 6720 6170 7073 2061 6e64 2077 6562  ing apps and web
-00001cf0: 2061 7070 6c69 6361 7469 6f6e 7320 7769   applications wi
-00001d00: 7468 2046 6c61 736b 2061 6e64 2046 6173  th Flask and Fas
-00001d10: 7441 5049 2e0a 0a23 2320 4665 6174 7572  tAPI...## Featur
-00001d20: 6573 0a0a 2323 2320 2a2a 4c4c 4d73 2a2a  es..### **LLMs**
-00001d30: 0a2d 2055 7469 6c69 7a65 204c 4c4d 7320  .- Utilize LLMs 
-00001d40: 7375 6368 2061 7320 4f70 656e 4149 2773  such as OpenAI's
-00001d50: 2043 6861 7447 5054 2074 6f20 6765 6e65   ChatGPT to gene
-00001d60: 7261 7465 206e 6174 7572 616c 206c 616e  rate natural lan
-00001d70: 6775 6167 6520 7465 7874 2e0a 2d20 436f  guage text..- Co
-00001d80: 6e66 6967 7572 6520 4c4c 4d20 636c 6173  nfigure LLM clas
-00001d90: 7365 7320 6561 7369 6c79 2c20 6368 6f6f  ses easily, choo
-00001da0: 7369 6e67 2073 7065 6369 6669 6320 6d6f  sing specific mo
-00001db0: 6465 6c73 2c20 7061 7261 6d65 7465 7273  dels, parameters
-00001dc0: 2c20 616e 6420 7365 7474 696e 6773 2e0a  , and settings..
-00001dd0: 2d20 4265 6e65 6669 7420 6672 6f6d 2061  - Benefit from a
-00001de0: 7574 6f6d 6174 6963 2072 6574 7269 6573  utomatic retries
-00001df0: 2077 6865 6e20 6d6f 6465 6c20 6361 6c6c   when model call
-00001e00: 7320 6661 696c 2c20 656e 7375 7269 6e67  s fail, ensuring
-00001e10: 2072 656c 6961 626c 6520 4c4c 4d20 0a20   reliable LLM . 
-00001e20: 2069 6e74 6572 6163 7469 6f6e 732e 0a0a   interactions...
-00001e30: 2323 2320 2a2a 5072 6f6d 7074 2054 656d  ### **Prompt Tem
-00001e40: 706c 6174 6573 2a2a 0a2d 2043 7265 6174  plates**.- Creat
-00001e50: 6520 6479 6e61 6d69 6320 7072 6f6d 7074  e dynamic prompt
-00001e60: 7320 7573 696e 6720 5072 6f6d 7074 2054  s using Prompt T
-00001e70: 656d 706c 6174 6573 2c20 7072 6f76 6964  emplates, provid
-00001e80: 696e 6720 666c 6578 6962 6c65 2061 6e64  ing flexible and
-00001e90: 2063 7573 746f 6d69 7a61 626c 6520 0a20   customizable . 
-00001ea0: 2074 6578 7420 6765 6e65 7261 7469 6f6e   text generation
-00001eb0: 2e0a 2d20 4465 6669 6e65 2076 6172 6961  ..- Define varia
-00001ec0: 626c 6573 2077 6974 6869 6e20 7072 6f6d  bles within prom
-00001ed0: 7074 7320 746f 2067 656e 6572 6174 6520  pts to generate 
-00001ee0: 7072 6f6d 7074 2073 7472 696e 6773 2074  prompt strings t
-00001ef0: 6169 6c6f 7265 6420 746f 2073 7065 6369  ailored to speci
-00001f00: 6669 6320 0a20 2069 6e70 7574 732e 0a0a  fic .  inputs...
-00001f10: 2323 2320 2a2a 466c 6f77 7320 616e 6420  ### **Flows and 
-00001f20: 466c 6f77 5374 6570 732a 2a0a 2d20 5374  FlowSteps**.- St
-00001f30: 7275 6374 7572 6520 4c4c 4d20 6170 706c  ructure LLM appl
-00001f40: 6963 6174 696f 6e73 2075 7369 6e67 2046  ications using F
-00001f50: 6c6f 7773 2061 6e64 2046 6c6f 7753 7465  lows and FlowSte
-00001f60: 7073 2c20 7072 6f76 6964 696e 6720 6120  ps, providing a 
-00001f70: 636c 6561 7220 616e 6420 6f72 6761 6e69  clear and organi
-00001f80: 7a65 6420 6672 616d 6577 6f72 6b20 666f  zed framework fo
-00001f90: 7220 6578 6563 7574 696e 6720 4c4c 4d20  r executing LLM 
-00001fa0: 696e 7465 7261 6374 696f 6e73 2e0a 2d20  interactions..- 
-00001fb0: 436f 6e6e 6563 7420 666c 6f77 2073 7465  Connect flow ste
-00001fc0: 7073 2074 6f20 7061 7373 206f 7574 7075  ps to pass outpu
-00001fd0: 7473 2061 7320 696e 7075 7473 2c20 6661  ts as inputs, fa
-00001fe0: 6369 6c69 7461 7469 6e67 2073 6561 6d6c  cilitating seaml
-00001ff0: 6573 7320 6461 7461 2066 6c6f 7720 616e  ess data flow an
-00002000: 640a 2020 2020 6d61 696e 7461 696e 696e  d.    maintainin
-00002010: 6720 6120 7472 616e 7370 6172 656e 7420  g a transparent 
-00002020: 4c4c 4d20 7069 7065 6c69 6e65 2e0a 2d20  LLM pipeline..- 
-00002030: 4c65 7665 7261 6765 2041 7379 6e63 2046  Leverage Async F
-00002040: 6c6f 7773 2074 6f20 7275 6e20 4c4c 4d73  lows to run LLMs
-00002050: 2069 6e20 7061 7261 6c6c 656c 2077 6865   in parallel whe
-00002060: 6e20 616c 6c20 7468 6569 7220 696e 7075  n all their inpu
-00002070: 7473 2061 7265 2061 7661 696c 6162 6c65  ts are available
-00002080: 2c20 0a20 206f 7074 696d 697a 696e 6720  , .  optimizing 
-00002090: 7065 7266 6f72 6d61 6e63 6520 616e 6420  performance and 
-000020a0: 6566 6669 6369 656e 6379 2e0a 2d20 496e  efficiency..- In
-000020b0: 636f 7270 6f72 6174 6520 6375 7374 6f6d  corporate custom
-000020c0: 2073 7472 696e 6720 6d61 6e69 7075 6c61   string manipula
-000020d0: 7469 6f6e 2066 756e 6374 696f 6e73 2064  tion functions d
-000020e0: 6972 6563 746c 7920 696e 746f 2066 6c6f  irectly into flo
-000020f0: 7773 2c20 616c 6c6f 7769 6e67 200a 2020  ws, allowing .  
-00002100: 7370 6563 6961 6c69 7a65 6420 7465 7874  specialized text
-00002110: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
-00002120: 2077 6974 686f 7574 2072 656c 7969 6e67   without relying
-00002130: 2073 6f6c 656c 7920 6f6e 204c 4c4d 2063   solely on LLM c
-00002140: 616c 6c73 2e0a 0a23 2323 202a 2a56 6563  alls...### **Vec
-00002150: 746f 7253 746f 7265 2049 6e74 6567 7261  torStore Integra
-00002160: 7469 6f6e 732a 2a0a 2d20 496e 7465 6772  tions**.- Integr
-00002170: 6174 6520 7769 7468 2076 6563 746f 7220  ate with vector 
-00002180: 6461 7461 6261 7365 7320 6c69 6b65 2050  databases like P
-00002190: 696e 6563 6f6e 6520 7573 696e 6720 7468  inecone using th
-000021a0: 6520 5665 6374 6f72 5374 6f72 6546 6c6f  e VectorStoreFlo
-000021b0: 7753 7465 702c 200a 2020 656d 706f 7765  wStep, .  empowe
-000021c0: 7269 6e67 2065 6666 6963 6965 6e74 2061  ring efficient a
-000021d0: 6e64 2073 6361 6c61 626c 6520 7374 6f72  nd scalable stor
-000021e0: 6167 6520 616e 6420 7265 7472 6965 7661  age and retrieva
-000021f0: 6c20 6f66 2076 6563 746f 7220 656d 6265  l of vector embe
-00002200: 6464 696e 6773 2e0a 2d20 4c65 7665 7261  ddings..- Levera
-00002210: 6765 2076 6563 746f 7220 6461 7461 6261  ge vector databa
-00002220: 7365 7320 666f 7220 7365 616d 6c65 7373  ses for seamless
-00002230: 2073 746f 7261 6765 2061 6e64 2071 7565   storage and que
-00002240: 7279 696e 6720 6f66 2076 6563 746f 7273  rying of vectors
-00002250: 2c20 656e 6162 6c69 6e67 2073 7472 6169  , enabling strai
-00002260: 6768 7466 6f72 7761 7264 2069 6e74 6567  ghtforward integ
-00002270: 7261 7469 6f6e 2077 6974 6820 4c4c 4d2d  ration with LLM-
-00002280: 706f 7765 7265 6420 6170 706c 6963 6174  powered applicat
-00002290: 696f 6e73 2e0a 0a23 2323 202a 2a43 616c  ions...### **Cal
-000022a0: 6c62 6163 6b73 2a2a 0a2d 2045 7865 6375  lbacks**.- Execu
-000022b0: 7465 2063 616c 6c62 6163 6b20 6675 6e63  te callback func
-000022c0: 7469 6f6e 7320 6174 2064 6966 6665 7265  tions at differe
-000022d0: 6e74 2073 7461 6765 7320 7769 7468 696e  nt stages within
-000022e0: 2066 6c6f 7720 7374 6570 732c 2065 6e61   flow steps, ena
-000022f0: 626c 696e 6720 656e 6861 6e63 6564 2063  bling enhanced c
-00002300: 7573 746f 6d69 7a61 7469 6f6e 2c20 6c6f  ustomization, lo
-00002310: 6767 696e 672c 2074 7261 6369 6e67 2c20  gging, tracing, 
-00002320: 6f72 206f 7468 6572 2073 7065 6369 6669  or other specifi
-00002330: 6320 696e 7465 6772 6174 696f 6e73 2e0a  c integrations..
-00002340: 2d20 5574 696c 697a 6520 6361 6c6c 6261  - Utilize callba
-00002350: 636b 7320 746f 2063 6f6d 7072 6568 656e  cks to comprehen
-00002360: 7369 7665 6c79 2063 6f6e 7472 6f6c 2061  sively control a
-00002370: 6e64 206d 6f6e 6974 6f72 204c 4c4d 2d70  nd monitor LLM-p
-00002380: 6f77 6572 6564 2061 7070 732c 2065 6e73  owered apps, ens
-00002390: 7572 696e 6720 0a20 2063 6c65 6172 2076  uring .  clear v
-000023a0: 6973 6962 696c 6974 7920 696e 746f 2074  isibility into t
-000023b0: 6865 2065 7865 6375 7469 6f6e 2070 726f  he execution pro
-000023c0: 6365 7373 2e0a 0a23 2323 202a 2a45 7870  cess...### **Exp
-000023d0: 6c69 6369 7420 4150 4920 616e 6420 4675  licit API and Fu
-000023e0: 6c6c 2054 7261 6e73 7061 7265 6e63 792a  ll Transparency*
-000023f0: 2a0a 5769 7468 204c 4c4d 466c 6f77 7320  *.With LLMFlows 
-00002400: 796f 7520 6861 7665 2074 6865 2066 756c  you have the ful
-00002410: 6c20 636f 6e74 726f 6c20 746f 2063 7265  l control to cre
-00002420: 6174 6520 6578 706c 6963 6974 2061 7070  ate explicit app
-00002430: 6c69 6361 7469 6f6e 7320 7769 7468 6f75  lications withou
-00002440: 7420 616e 7920 6869 6464 656e 2070 726f  t any hidden pro
-00002450: 6d70 7473 206f 7220 7072 6564 6566 696e  mpts or predefin
-00002460: 6564 2062 6568 6176 696f 7273 2e0a 0a49  ed behaviors...I
-00002470: 6e20 6164 6469 7469 6f6e 204c 4c4d 466c  n addition LLMFl
-00002480: 6f77 7320 616c 6c6f 7773 2079 6f75 2074  ows allows you t
-00002490: 6f20 616e 7377 6572 2071 7565 7374 696f  o answer questio
-000024a0: 6e73 2073 7563 6820 6173 3a0a 0a2d 2057  ns such as:..- W
-000024b0: 6865 6e20 7761 7320 6120 7061 7274 6963  hen was a partic
-000024c0: 756c 6172 2066 6c6f 7773 7465 7020 7275  ular flowstep ru
-000024d0: 6e3f 0a2d 2048 6f77 206d 7563 6820 7469  n?.- How much ti
-000024e0: 6d65 2064 6964 2069 7420 7461 6b65 3f0a  me did it take?.
-000024f0: 2d20 5768 6174 2077 6572 6520 7468 6520  - What were the 
-00002500: 696e 7075 7420 7661 7269 6162 6c65 733f  input variables?
-00002510: 0a2d 2057 6861 7420 7761 7320 7468 6520  .- What was the 
-00002520: 7072 6f6d 7074 2074 656d 706c 6174 653f  prompt template?
-00002530: 0a2d 2057 6861 7420 6469 6420 7468 6520  .- What did the 
-00002540: 7072 6f6d 7074 206c 6f6f 6b20 6c69 6b65  prompt look like
-00002550: 3f0a 2d20 5768 6174 2077 6173 2074 6865  ?.- What was the
-00002560: 2065 7861 6374 2063 6f6e 6669 6775 7261   exact configura
-00002570: 7469 6f6e 206f 6620 7468 6520 6d6f 6465  tion of the mode
-00002580: 6c3f 0a2d 2048 6f77 206d 616e 7920 7469  l?.- How many ti
-00002590: 6d65 7320 6469 6420 7765 2072 6574 7279  mes did we retry
-000025a0: 2074 6865 2072 6571 7565 7374 3f0a 2d20   the request?.- 
-000025b0: 5768 6174 2077 6173 2074 6865 2072 6177  What was the raw
-000025c0: 2064 6174 6120 7468 6520 4150 4920 7265   data the API re
-000025d0: 7475 726e 6564 3f0a 2d20 486f 7720 6d61  turned?.- How ma
-000025e0: 6e79 2074 6f6b 656e 7320 7765 7265 2075  ny tokens were u
-000025f0: 7365 643f 0a2d 2057 6861 7420 7761 7320  sed?.- What was 
-00002600: 7468 6520 6669 6e61 6c20 7265 7375 6c74  the final result
-00002610: 3f0a 0a23 2320 4c69 6365 6e73 650a 4c4c  ?..## License.LL
-00002620: 4d46 6c6f 7773 2069 7320 636f 7665 7265  MFlows is covere
-00002630: 6420 6279 2074 6865 204d 4954 206c 6963  d by the MIT lic
-00002640: 656e 7365 2e20 466f 7220 6d6f 7265 2069  ense. For more i
-00002650: 6e66 6f72 6d61 7469 6f6e 2c20 6368 6563  nformation, chec
-00002660: 6b20 604c 4943 454e 4345 2e6d 6460 2e0a  k `LICENCE.md`..
-00002670: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
-00002680: 0a54 6861 6e6b 2079 6f75 2066 6f72 2073  .Thank you for s
-00002690: 7065 6e64 696e 6720 7469 6d65 2067 6f69  pending time goi
-000026a0: 6e67 206f 7665 7220 6f75 7220 5245 4144  ng over our READ
-000026b0: 4d45 2120 4966 2079 6f75 2066 696e 6420  ME! If you find 
-000026c0: 4c4c 4d46 6c6f 7773 2065 7863 6974 696e  LLMFlows excitin
-000026d0: 6720 616e 6420 0a79 6f75 2061 7265 2063  g and .you are c
-000026e0: 6f6e 7369 6465 7269 6e67 2063 6f6e 7472  onsidering contr
-000026f0: 6962 7574 696e 672c 2070 6c65 6173 6520  ibuting, please 
-00002700: 6368 6563 6b20 5b60 434f 4e54 5249 4255  check [`CONTRIBU
-00002710: 5449 4e47 2e6d 6460 5d28 6874 7470 733a  TING.md`](https:
-00002720: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746f  //github.com/sto
-00002730: 7961 6e2d 7374 6f79 616e 6f76 2f6c 6c6d  yan-stoyanov/llm
-00002740: 666c 6f77 732f 626c 6f62 2f6d 6169 6e2f  flows/blob/main/
-00002750: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00002760: 2e0a                                     ..
+00000450: 7374 6172 732f 7374 6f79 616e 2d73 746f  stars/stoyan-sto
+00000460: 7961 6e6f 762f 6c6c 6d66 6c6f 7773 3f73  yanov/llmflows?s
+00000470: 7479 6c65 3d73 6f63 6961 6c29 0a21 5b52  tyle=social).![R
+00000480: 656c 6561 7365 2064 6174 655d 2868 7474  elease date](htt
+00000490: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000004a0: 2e69 6f2f 6769 7468 7562 2f72 656c 6561  .io/github/relea
+000004b0: 7365 2d64 6174 652f 7374 6f79 616e 2d73  se-date/stoyan-s
+000004c0: 746f 7961 6e6f 762f 6c6c 6d66 6c6f 7773  toyanov/llmflows
+000004d0: 3f73 7479 6c65 3d73 6f63 6961 6c29 0a0a  ?style=social)..
+000004e0: 446f 6375 6d65 6e74 6174 696f 6e3a 203c  Documentation: <
+000004f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000500: 6c6c 6d66 6c6f 7773 2e72 6561 6474 6865  llmflows.readthe
+00000510: 646f 6373 2e69 6f2f 2220 7461 7267 6574  docs.io/" target
+00000520: 3d22 5f62 6c61 6e6b 223e 6874 7470 733a  ="_blank">https:
+00000530: 2f2f 6c6c 6d66 6c6f 7773 2e72 6561 6474  //llmflows.readt
+00000540: 6865 646f 6373 2e69 6f3c 2f61 3e3c 2f62  hedocs.io</a></b
+00000550: 723e 0a50 7950 493a 203c 6120 6872 6566  r>.PyPI: <a href
+00000560: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000570: 7267 2f70 726f 6a65 6374 2f6c 6c6d 666c  rg/project/llmfl
+00000580: 6f77 732f 2220 7461 7267 6574 3d22 5f62  ows/" target="_b
+00000590: 6c61 6e6b 223e 6874 7470 733a 2f2f 7079  lank">https://py
+000005a0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
+000005b0: 6c6d 666c 6f77 733c 2f61 3e3c 2f62 723e  lmflows</a></br>
+000005c0: 0a54 7769 7474 6572 3a20 3c61 2068 7265  .Twitter: <a hre
+000005d0: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
+000005e0: 6572 2e63 6f6d 2f4c 4c4d 466c 6f77 732f  er.com/LLMFlows/
+000005f0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000600: 223e 6874 7470 733a 2f2f 7477 6974 7465  ">https://twitte
+00000610: 722e 636f 6d2f 4c4c 4d46 6c6f 7773 3c2f  r.com/LLMFlows</
+00000620: 613e 3c2f 6272 3e0a 5375 6273 7461 636b  a></br>.Substack
+00000630: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
+00000640: 3a2f 2f6c 6c6d 666c 6f77 732e 7375 6273  ://llmflows.subs
+00000650: 7461 636b 2e63 6f6d 2f22 2074 6172 6765  tack.com/" targe
+00000660: 743d 225f 626c 616e 6b22 3e68 7474 7073  t="_blank">https
+00000670: 3a2f 2f6c 6c6d 666c 6f77 732e 7375 6273  ://llmflows.subs
+00000680: 7461 636b 2e63 6f6d 3c2f 613e 3c2f 6272  tack.com</a></br
+00000690: 3e0a 0a23 2320 4162 6f75 740a 4c4c 4d46  >..## About.LLMF
+000006a0: 6c6f 7773 2069 7320 6120 6672 616d 6577  lows is a framew
+000006b0: 6f72 6b20 666f 7220 6275 696c 6469 6e67  ork for building
+000006c0: 2073 696d 706c 652c 2065 7870 6c69 6369   simple, explici
+000006d0: 742c 2061 6e64 2074 7261 6e73 7061 7265  t, and transpare
+000006e0: 6e74 204c 4c4d 284c 6172 6765 200a 4c61  nt LLM(Large .La
+000006f0: 6e67 7561 6765 204d 6f64 656c 2920 6170  nguage Model) ap
+00000700: 706c 6963 6174 696f 6e73 2e0a 0a23 2320  plications...## 
+00000710: 496e 7374 616c 6c61 7469 6f6e 0a60 6060  Installation.```
+00000720: 0a70 6970 2069 6e73 7461 6c6c 206c 6c6d  .pip install llm
+00000730: 666c 6f77 730a 6060 600a 0a23 2320 5068  flows.```..## Ph
+00000740: 696c 6f73 6f70 6879 0a0a 2323 2320 2a2a  ilosophy..### **
+00000750: 5369 6d70 6c65 2a2a 0a4f 7572 2067 6f61  Simple**.Our goa
+00000760: 6c20 6973 2074 6f20 6275 696c 6420 6120  l is to build a 
+00000770: 7369 6d70 6c65 2c20 7765 6c6c 2d64 6f63  simple, well-doc
+00000780: 756d 656e 7465 6420 6672 616d 6577 6f72  umented framewor
+00000790: 6b20 7769 7468 206d 696e 696d 616c 2061  k with minimal a
+000007a0: 6273 7472 6163 7469 6f6e 7320 7468 6174  bstractions that
+000007b0: 200a 616c 6c6f 7720 7573 6572 7320 746f   .allow users to
+000007c0: 2062 7569 6c64 2066 6c65 7869 626c 6520   build flexible 
+000007d0: 4c4c 4d2d 706f 7765 7265 6420 6170 7073  LLM-powered apps
+000007e0: 2077 6974 686f 7574 2063 6f6d 7072 6f6d   without comprom
+000007f0: 6973 696e 6720 6f6e 2063 6170 6162 696c  ising on capabil
+00000800: 6974 6965 732e 0a0a 2323 2320 2a2a 4578  ities...### **Ex
+00000810: 706c 6963 6974 2a2a 0a57 6520 7761 6e74  plicit**.We want
+00000820: 2074 6f20 6372 6561 7465 2061 6e20 6578   to create an ex
+00000830: 706c 6963 6974 2041 5049 2065 6e61 626c  plicit API enabl
+00000840: 696e 6720 7573 6572 7320 746f 2077 7269  ing users to wri
+00000850: 7465 2063 6c65 616e 2061 6e64 2072 6561  te clean and rea
+00000860: 6461 626c 6520 636f 6465 2077 6869 6c65  dable code while
+00000870: 200a 6561 7369 6c79 2063 7265 6174 696e   .easily creatin
+00000880: 6720 636f 6d70 6c65 7820 666c 6f77 7320  g complex flows 
+00000890: 6f66 204c 4c4d 7320 696e 7465 7261 6374  of LLMs interact
+000008a0: 696e 6720 7769 7468 2065 6163 6820 6f74  ing with each ot
+000008b0: 6865 722e 204c 4c4d 466c 6f77 7327 2063  her. LLMFlows' c
+000008c0: 6c61 7373 6573 200a 6769 7665 2075 7365  lasses .give use
+000008d0: 7273 2066 756c 6c20 636f 6e74 726f 6c20  rs full control 
+000008e0: 616e 6420 646f 206e 6f74 2068 6176 6520  and do not have 
+000008f0: 616e 7920 6869 6464 656e 2070 726f 6d70  any hidden promp
+00000900: 7473 206f 7220 4c4c 4d20 6361 6c6c 732e  ts or LLM calls.
+00000910: 200a 0a23 2323 202a 2a54 7261 6e73 7061   ..### **Transpa
+00000920: 7265 6e74 2a2a 0a57 6520 6169 6d20 746f  rent**.We aim to
+00000930: 2068 656c 7020 7573 6572 7320 6861 7665   help users have
+00000940: 2066 756c 6c20 7472 616e 7370 6172 656e   full transparen
+00000950: 6379 206f 6e20 7468 6569 7220 4c4c 4d2d  cy on their LLM-
+00000960: 706f 7765 7265 6420 6170 7073 2062 7920  powered apps by 
+00000970: 7072 6f76 6964 696e 6720 0a74 7261 6365  providing .trace
+00000980: 6162 6c65 2066 6c6f 7773 2061 6e64 2063  able flows and c
+00000990: 6f6d 706c 6574 6520 696e 666f 726d 6174  omplete informat
+000009a0: 696f 6e20 666f 7220 6561 6368 2061 7070  ion for each app
+000009b0: 2063 6f6d 706f 6e65 6e74 2c20 6d61 6b69   component, maki
+000009c0: 6e67 2069 7420 6561 7379 2074 6f20 0a6d  ng it easy to .m
+000009d0: 6f6e 6974 6f72 2c20 6d61 696e 7461 696e  onitor, maintain
+000009e0: 2c20 616e 6420 6465 6275 672e 0a0a 2323  , and debug...##
+000009f0: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
+00000a00: 0a23 2323 204c 4c4d 730a 4c4c 4d73 2061  .### LLMs.LLMs a
+00000a10: 7265 206f 6e65 206f 6620 7468 6520 6d61  re one of the ma
+00000a20: 696e 2061 6273 7472 6163 7469 6f6e 7320  in abstractions 
+00000a30: 696e 204c 4c4d 466c 6f77 732e 204c 4c4d  in LLMFlows. LLM
+00000a40: 2063 6c61 7373 6573 2061 7265 2077 7261   classes are wra
+00000a50: 7070 6572 7320 6172 6f75 6e64 204c 4c4d  ppers around LLM
+00000a60: 200a 4150 4973 2073 7563 6820 6173 204f   .APIs such as O
+00000a70: 7065 6e41 4927 7320 4150 4973 2e20 5468  penAI's APIs. Th
+00000a80: 6579 2070 726f 7669 6465 206d 6574 686f  ey provide metho
+00000a90: 6473 2066 6f72 2063 6f6e 6669 6775 7269  ds for configuri
+00000aa0: 6e67 2061 6e64 2063 616c 6c69 6e67 2074  ng and calling t
+00000ab0: 6865 7365 2041 5049 732c 200a 7265 7472  hese APIs, .retr
+00000ac0: 7969 6e67 2066 6169 6c65 6420 6361 6c6c  ying failed call
+00000ad0: 732c 2061 6e64 2066 6f72 6d61 7474 696e  s, and formattin
+00000ae0: 6720 7468 6520 7265 7370 6f6e 7365 732e  g the responses.
+00000af0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000b00: 206c 6c6d 666c 6f77 732e 6c6c 6d73 2069   llmflows.llms i
+00000b10: 6d70 6f72 7420 4f70 656e 4149 0a0a 6c6c  mport OpenAI..ll
+00000b20: 6d20 3d20 4f70 656e 4149 2861 7069 5f6b  m = OpenAI(api_k
+00000b30: 6579 3d22 3c79 6f75 722d 6f70 656e 6169  ey="<your-openai
+00000b40: 2d61 7069 2d6b 6579 3e22 290a 0a72 6573  -api-key>")..res
+00000b50: 756c 742c 2063 616c 6c5f 6461 7461 2c20  ult, call_data, 
+00000b60: 6d6f 6465 6c5f 636f 6e66 6967 203d 206c  model_config = l
+00000b70: 6c6d 2e67 656e 6572 6174 6528 0a20 2020  lm.generate(.   
+00000b80: 7072 6f6d 7074 3d22 4765 6e65 7261 7465  prompt="Generate
+00000b90: 2061 2063 6f6f 6c20 7469 746c 6520 666f   a cool title fo
+00000ba0: 7220 616e 2038 3073 2072 6f63 6b20 736f  r an 80s rock so
+00000bb0: 6e67 220a 290a 6060 600a 0a0a 2323 2320  ng".).```...### 
+00000bc0: 5072 6f6d 7074 5465 6d70 6c61 7465 730a  PromptTemplates.
+00000bd0: 5468 6520 6050 726f 6d70 7454 656d 706c  The `PromptTempl
+00000be0: 6174 6560 2063 6c61 7373 2061 6c6c 6f77  ate` class allow
+00000bf0: 7320 7573 2074 6f20 6372 6561 7465 2073  s us to create s
+00000c00: 7472 696e 6773 2077 6974 6820 7661 7269  trings with vari
+00000c10: 6162 6c65 7320 7468 6174 2077 6520 6361  ables that we ca
+00000c20: 6e20 6669 6c6c 200a 696e 2064 796e 616d  n fill .in dynam
+00000c30: 6963 616c 6c79 206c 6174 6572 206f 6e2e  ically later on.
+00000c40: 204f 6e63 6520 6120 7072 6f6d 7074 2074   Once a prompt t
+00000c50: 656d 706c 6174 6520 6f62 6a65 6374 2069  emplate object i
+00000c60: 7320 6372 6561 7465 6420 616e 2061 6374  s created an act
+00000c70: 7561 6c20 7072 6f6d 7074 2063 616e 200a  ual prompt can .
+00000c80: 6265 2067 656e 6572 6174 6564 2062 7920  be generated by 
+00000c90: 7072 6f76 6964 696e 6720 7468 6520 7265  providing the re
+00000ca0: 7175 6972 6564 2076 6172 6961 626c 6573  quired variables
+00000cb0: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+00000cc0: 6d20 6c6c 6d66 6c6f 7773 2e6c 6c6d 7320  m llmflows.llms 
+00000cd0: 696d 706f 7274 204f 7065 6e41 490a 6672  import OpenAI.fr
+00000ce0: 6f6d 206c 6c6d 666c 6f77 732e 7072 6f6d  om llmflows.prom
+00000cf0: 7074 7320 696d 706f 7274 2050 726f 6d70  pts import Promp
+00000d00: 7454 656d 706c 6174 650a 0a0a 7072 6f6d  tTemplate...prom
+00000d10: 7074 5f74 656d 706c 6174 6520 3d20 5072  pt_template = Pr
+00000d20: 6f6d 7074 5465 6d70 6c61 7465 280a 2020  omptTemplate(.  
+00000d30: 2020 7072 6f6d 7074 3d22 4765 6e65 7261    prompt="Genera
+00000d40: 7465 2061 2074 6974 6c65 2066 6f72 2061  te a title for a
+00000d50: 2039 3073 2068 6970 2d68 6f70 2073 6f6e   90s hip-hop son
+00000d60: 6720 6162 6f75 7420 7b74 6f70 6963 7d2e  g about {topic}.
+00000d70: 220a 290a 6c6c 6d5f 7072 6f6d 7074 203d  ".).llm_prompt =
+00000d80: 2070 726f 6d70 745f 7465 6d70 6c61 7465   prompt_template
+00000d90: 2e67 6574 5f70 726f 6d70 7428 746f 7069  .get_prompt(topi
+00000da0: 633d 2266 7269 656e 6473 6869 7022 290a  c="friendship").
+00000db0: 0a70 7269 6e74 286c 6c6d 5f70 726f 6d70  .print(llm_promp
+00000dc0: 7429 0a0a 6c6c 6d20 3d20 4f70 656e 4149  t)..llm = OpenAI
+00000dd0: 2861 7069 5f6b 6579 3d22 3c79 6f75 722d  (api_key="<your-
+00000de0: 6f70 656e 6169 2d61 7069 2d6b 6579 3e22  openai-api-key>"
+00000df0: 290a 736f 6e67 5f74 6974 6c65 203d 206c  ).song_title = l
+00000e00: 6c6d 2e67 656e 6572 6174 6528 6c6c 6d5f  lm.generate(llm_
+00000e10: 7072 6f6d 7074 290a 0a70 7269 6e74 2873  prompt)..print(s
+00000e20: 6f6e 675f 7469 746c 6529 0a60 6060 0a0a  ong_title).```..
+00000e30: 2323 2320 4368 6174 204c 4c4d 730a 556e  ### Chat LLMs.Un
+00000e40: 6c69 6b65 2072 6567 756c 6172 204c 4c4d  like regular LLM
+00000e50: 7320 7468 6174 206f 6e6c 7920 7265 7175  s that only requ
+00000e60: 6972 6520 6120 7072 6f6d 7074 2074 6f20  ire a prompt to 
+00000e70: 6765 6e65 7261 7465 2074 6578 742c 2063  generate text, c
+00000e80: 6861 7420 4c4c 4d73 2072 6571 7569 7265  hat LLMs require
+00000e90: 2061 200a 636f 6e76 6572 7361 7469 6f6e   a .conversation
+00000ea0: 2068 6973 746f 7279 2e20 5468 6520 636f   history. The co
+00000eb0: 6e76 6572 7361 7469 6f6e 2068 6973 746f  nversation histo
+00000ec0: 7279 2069 7320 7265 7072 6573 656e 7465  ry is represente
+00000ed0: 6420 0a61 7320 6120 6c69 7374 206f 6620  d .as a list of 
+00000ee0: 6d65 7373 6167 6573 2062 6574 7765 656e  messages between
+00000ef0: 2061 2075 7365 7220 616e 6420 616e 2061   a user and an a
+00000f00: 7373 6973 7461 6e74 2e20 5468 6973 2063  ssistant. This c
+00000f10: 6f6e 7665 7273 6174 696f 6e20 6869 7374  onversation hist
+00000f20: 6f72 7920 6973 200a 7365 6e74 2074 6f20  ory is .sent to 
+00000f30: 7468 6520 6d6f 6465 6c2c 2061 6e64 2061  the model, and a
+00000f40: 206e 6577 206d 6573 7361 6765 2069 7320   new message is 
+00000f50: 6765 6e65 7261 7465 6420 6261 7365 6420  generated based 
+00000f60: 6f6e 2069 742e 0a0a 4c4c 4d46 6c6f 7773  on it...LLMFlows
+00000f70: 2070 726f 7669 6465 7320 6120 604d 6573   provides a `Mes
+00000f80: 7361 6765 4869 7374 6f72 7960 2063 6c61  sageHistory` cla
+00000f90: 7373 2074 6f20 6d61 6e61 6765 2074 6865  ss to manage the
+00000fa0: 2072 6571 7569 7265 6420 636f 6e76 6572   required conver
+00000fb0: 7361 7469 6f6e 2068 6973 746f 7279 200a  sation history .
+00000fc0: 666f 7220 6368 6174 204c 4c4d 732e 0a0a  for chat LLMs...
+00000fd0: 596f 7520 6361 6e20 6275 696c 6420 6120  You can build a 
+00000fe0: 7369 6d70 6c65 2063 6861 7462 6f74 2062  simple chatbot b
+00000ff0: 7920 7573 696e 6720 7468 6520 604f 7065  y using the `Ope
+00001000: 6e41 4943 6861 7460 2061 6e64 2060 4d65  nAIChat` and `Me
+00001010: 7373 6167 6548 6973 746f 7279 6020 636c  ssageHistory` cl
+00001020: 6173 7365 733a 0a0a 6060 6070 7974 686f  asses:..```pytho
+00001030: 6e0a 6672 6f6d 206c 6c6d 666c 6f77 732e  n.from llmflows.
+00001040: 6c6c 6d73 2069 6d70 6f72 7420 4f70 656e  llms import Open
+00001050: 4149 4368 6174 2c20 4d65 7373 6167 6548  AIChat, MessageH
+00001060: 6973 746f 7279 0a0a 6c6c 6d20 3d20 4f70  istory..llm = Op
+00001070: 656e 4149 4368 6174 2861 7069 5f6b 6579  enAIChat(api_key
+00001080: 3d22 3c79 6f75 722d 6f70 656e 6169 2d61  ="<your-openai-a
+00001090: 7069 2d6b 6579 3e22 290a 6d65 7373 6167  pi-key>").messag
+000010a0: 655f 6869 7374 6f72 7920 3d20 4d65 7373  e_history = Mess
+000010b0: 6167 6548 6973 746f 7279 2829 0a0a 7768  ageHistory()..wh
+000010c0: 696c 6520 5472 7565 3a0a 2020 2020 7573  ile True:.    us
+000010d0: 6572 5f6d 6573 7361 6765 203d 2069 6e70  er_message = inp
+000010e0: 7574 2822 596f 753a 2229 0a20 2020 206d  ut("You:").    m
+000010f0: 6573 7361 6765 5f68 6973 746f 7279 2e61  essage_history.a
+00001100: 6464 5f75 7365 725f 6d65 7373 6167 6528  dd_user_message(
+00001110: 7573 6572 5f6d 6573 7361 6765 290a 0a20  user_message).. 
+00001120: 2020 206c 6c6d 5f72 6573 706f 6e73 652c     llm_response,
+00001130: 2063 616c 6c5f 6461 7461 2c20 6d6f 6465   call_data, mode
+00001140: 6c5f 636f 6e66 6967 203d 206c 6c6d 2e67  l_config = llm.g
+00001150: 656e 6572 6174 6528 6d65 7373 6167 655f  enerate(message_
+00001160: 6869 7374 6f72 7929 0a20 2020 206d 6573  history).    mes
+00001170: 7361 6765 5f68 6973 746f 7279 2e61 6464  sage_history.add
+00001180: 5f61 695f 6d65 7373 6167 6528 6c6c 6d5f  _ai_message(llm_
+00001190: 7265 7370 6f6e 7365 290a 0a20 2020 2070  response)..    p
+000011a0: 7269 6e74 2866 224c 4c4d 3a20 7b6c 6c6d  rint(f"LLM: {llm
+000011b0: 5f72 6573 706f 6e73 657d 2229 0a60 6060  _response}").```
+000011c0: 0a0a 2323 2320 4c4c 4d20 466c 6f77 730a  ..### LLM Flows.
+000011d0: 4f66 7465 6e20 7469 6d65 732c 2072 6561  Often times, rea
+000011e0: 6c2d 776f 726c 6420 6170 706c 6963 6174  l-world applicat
+000011f0: 696f 6e73 2063 616e 2062 6520 6d6f 7265  ions can be more
+00001200: 2063 6f6d 706c 6578 2061 6e64 2063 616e   complex and can
+00001210: 2068 6176 6520 6465 7065 6e64 656e 6369   have dependenci
+00001220: 6573 200a 6265 7477 6565 6e20 7072 6f6d  es .between prom
+00001230: 7074 7320 616e 6420 4c4c 4d20 6361 6c6c  pts and LLM call
+00001240: 732e 2046 6f72 2065 7861 6d70 6c65 3a0a  s. For example:.
+00001250: 0a21 5b43 6f6d 706c 6578 2066 6c6f 775d  .![Complex flow]
+00001260: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001270: 636f 6d2f 7374 6f79 616e 2d73 746f 7961  com/stoyan-stoya
+00001280: 6e6f 762f 6c6c 6d66 6c6f 7773 2f62 6c6f  nov/llmflows/blo
+00001290: 622f 6d61 696e 2f64 6f63 732f 636f 6d70  b/main/docs/comp
+000012a0: 6c65 785f 666c 6f77 2e70 6e67 290a 0a57  lex_flow.png)..W
+000012b0: 6865 6e20 796f 7520 7761 6e74 2074 6f20  hen you want to 
+000012c0: 6275 696c 6420 6170 7073 2077 6974 6820  build apps with 
+000012d0: 636f 6d70 6c65 7820 6465 7065 6e64 656e  complex dependen
+000012e0: 6369 6573 2079 6f75 2063 616e 2075 7365  cies you can use
+000012f0: 2074 6865 2060 466c 6f77 6020 616e 6420   the `Flow` and 
+00001300: 0a60 466c 6f77 7374 6570 6020 636c 6173  .`Flowstep` clas
+00001310: 7365 732e 204c 4c4d 466c 6f77 7320 7769  ses. LLMFlows wi
+00001320: 6c6c 2066 6967 7572 6520 6f75 7420 7468  ll figure out th
+00001330: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
+00001340: 6e64 206d 616b 6520 7375 7265 2065 6163  nd make sure eac
+00001350: 6820 0a66 6c6f 7773 7465 7020 7275 6e73  h .flowstep runs
+00001360: 206f 6e6c 7920 7768 656e 2061 6c6c 2069   only when all i
+00001370: 7473 2064 6570 656e 6465 6e63 6965 7320  ts dependencies 
+00001380: 6172 6520 6d65 743a 0a0a 6060 6070 7974  are met:..```pyt
+00001390: 686f 6e0a 6672 6f6d 206c 6c6d 666c 6f77  hon.from llmflow
+000013a0: 732e 666c 6f77 7320 696d 706f 7274 2046  s.flows import F
+000013b0: 6c6f 772c 2046 6c6f 7753 7465 700a 6672  low, FlowStep.fr
+000013c0: 6f6d 206c 6c6d 666c 6f77 732e 6c6c 6d73  om llmflows.llms
+000013d0: 2069 6d70 6f72 7420 4f70 656e 4149 0a66   import OpenAI.f
+000013e0: 726f 6d20 6c6c 6d66 6c6f 7773 2e70 726f  rom llmflows.pro
+000013f0: 6d70 7473 2069 6d70 6f72 7420 5072 6f6d  mpts import Prom
+00001400: 7074 5465 6d70 6c61 7465 0a0a 6f70 656e  ptTemplate..open
+00001410: 6169 5f6c 6c6d 203d 204f 7065 6e41 4928  ai_llm = OpenAI(
+00001420: 6170 695f 6b65 793d 223c 796f 7572 2d6f  api_key="<your-o
+00001430: 7065 6e61 692d 6170 692d 6b65 793e 2229  penai-api-key>")
+00001440: 0a0a 2320 4372 6561 7465 2070 726f 6d70  ..# Create promp
+00001450: 7420 7465 6d70 6c61 7465 730a 7469 746c  t templates.titl
+00001460: 655f 7465 6d70 6c61 7465 203d 2050 726f  e_template = Pro
+00001470: 6d70 7454 656d 706c 6174 6528 2257 6861  mptTemplate("Wha
+00001480: 7420 6973 2061 2067 6f6f 6420 7469 746c  t is a good titl
+00001490: 6520 6f66 2061 206d 6f76 6965 2061 626f  e of a movie abo
+000014a0: 7574 207b 746f 7069 637d 3f22 290a 736f  ut {topic}?").so
+000014b0: 6e67 5f74 656d 706c 6174 6520 3d20 5072  ng_template = Pr
+000014c0: 6f6d 7074 5465 6d70 6c61 7465 280a 2020  omptTemplate(.  
+000014d0: 2020 2257 6861 7420 6973 2061 2067 6f6f    "What is a goo
+000014e0: 6420 736f 6e67 2074 6974 6c65 206f 6620  d song title of 
+000014f0: 6120 736f 756e 6474 7261 636b 2066 6f72  a soundtrack for
+00001500: 2061 206d 6f76 6965 2063 616c 6c65 6420   a movie called 
+00001510: 7b6d 6f76 6965 5f74 6974 6c65 7d3f 220a  {movie_title}?".
+00001520: 290a 6368 6172 6163 7465 7273 5f74 656d  ).characters_tem
+00001530: 706c 6174 6520 3d20 5072 6f6d 7074 5465  plate = PromptTe
+00001540: 6d70 6c61 7465 280a 2020 2020 2257 6861  mplate(.    "Wha
+00001550: 7420 6172 6520 7477 6f20 6d61 696e 2063  t are two main c
+00001560: 6861 7261 6374 6572 7320 666f 7220 6120  haracters for a 
+00001570: 6d6f 7669 6520 6361 6c6c 6564 207b 6d6f  movie called {mo
+00001580: 7669 655f 7469 746c 657d 3f22 0a29 0a6c  vie_title}?".).l
+00001590: 7972 6963 735f 7465 6d70 6c61 7465 203d  yrics_template =
+000015a0: 2050 726f 6d70 7454 656d 706c 6174 6528   PromptTemplate(
+000015b0: 0a20 2020 2022 5772 6974 6520 6c79 7269  .    "Write lyri
+000015c0: 6373 206f 6620 6120 6d6f 7669 6520 736f  cs of a movie so
+000015d0: 6e67 2063 616c 6c65 6420 7b73 6f6e 675f  ng called {song_
+000015e0: 7469 746c 657d 2e20 5468 6520 6d61 696e  title}. The main
+000015f0: 2063 6861 7261 6374 6572 7320 6172 6520   characters are 
+00001600: 220a 2020 2020 227b 6d61 696e 5f63 6861  ".    "{main_cha
+00001610: 7261 6374 6572 737d 220a 290a 0a23 2043  racters}".)..# C
+00001620: 7265 6174 6520 666c 6f77 7374 6570 730a  reate flowsteps.
+00001630: 6d6f 7669 655f 7469 746c 655f 666c 6f77  movie_title_flow
+00001640: 7374 6570 203d 2046 6c6f 7753 7465 7028  step = FlowStep(
+00001650: 0a20 2020 206e 616d 653d 224d 6f76 6965  .    name="Movie
+00001660: 2054 6974 6c65 2046 6c6f 7773 7465 7022   Title Flowstep"
+00001670: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
+00001680: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
+00001690: 5f74 656d 706c 6174 653d 7469 746c 655f  _template=title_
+000016a0: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
+000016b0: 7470 7574 5f6b 6579 3d22 6d6f 7669 655f  tput_key="movie_
+000016c0: 7469 746c 6522 2c0a 290a 0a73 6f6e 675f  title",.)..song_
+000016d0: 7469 746c 655f 666c 6f77 7374 6570 203d  title_flowstep =
+000016e0: 2046 6c6f 7753 7465 7028 0a20 2020 206e   FlowStep(.    n
+000016f0: 616d 653d 2253 6f6e 6720 5469 746c 6520  ame="Song Title 
+00001700: 466c 6f77 7374 6570 222c 0a20 2020 206c  Flowstep",.    l
+00001710: 6c6d 3d6f 7065 6e61 695f 6c6c 6d2c 0a20  lm=openai_llm,. 
+00001720: 2020 2070 726f 6d70 745f 7465 6d70 6c61     prompt_templa
+00001730: 7465 3d73 6f6e 675f 7465 6d70 6c61 7465  te=song_template
+00001740: 2c0a 2020 2020 6f75 7470 7574 5f6b 6579  ,.    output_key
+00001750: 3d22 736f 6e67 5f74 6974 6c65 222c 0a29  ="song_title",.)
+00001760: 0a0a 6368 6172 6163 7465 7273 5f66 6c6f  ..characters_flo
+00001770: 7773 7465 7020 3d20 466c 6f77 5374 6570  wstep = FlowStep
+00001780: 280a 2020 2020 6e61 6d65 3d22 4368 6172  (.    name="Char
+00001790: 6163 7465 7273 2046 6c6f 7773 7465 7022  acters Flowstep"
+000017a0: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
+000017b0: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
+000017c0: 5f74 656d 706c 6174 653d 6368 6172 6163  _template=charac
+000017d0: 7465 7273 5f74 656d 706c 6174 652c 0a20  ters_template,. 
+000017e0: 2020 206f 7574 7075 745f 6b65 793d 226d     output_key="m
+000017f0: 6169 6e5f 6368 6172 6163 7465 7273 222c  ain_characters",
+00001800: 0a29 0a0a 736f 6e67 5f6c 7972 6963 735f  .)..song_lyrics_
+00001810: 666c 6f77 7374 6570 203d 2046 6c6f 7753  flowstep = FlowS
+00001820: 7465 7028 0a20 2020 206e 616d 653d 2253  tep(.    name="S
+00001830: 6f6e 6720 4c79 7269 6373 2046 6c6f 7773  ong Lyrics Flows
+00001840: 7465 7022 2c0a 2020 2020 6c6c 6d3d 6f70  tep",.    llm=op
+00001850: 656e 6169 5f6c 6c6d 2c0a 2020 2020 7072  enai_llm,.    pr
+00001860: 6f6d 7074 5f74 656d 706c 6174 653d 6c79  ompt_template=ly
+00001870: 7269 6373 5f74 656d 706c 6174 652c 0a20  rics_template,. 
+00001880: 2020 206f 7574 7075 745f 6b65 793d 2273     output_key="s
+00001890: 6f6e 675f 6c79 7269 6373 222c 0a29 0a0a  ong_lyrics",.)..
+000018a0: 2320 436f 6e6e 6563 7420 666c 6f77 7374  # Connect flowst
+000018b0: 6570 730a 6d6f 7669 655f 7469 746c 655f  eps.movie_title_
+000018c0: 666c 6f77 7374 6570 2e63 6f6e 6e65 6374  flowstep.connect
+000018d0: 2873 6f6e 675f 7469 746c 655f 666c 6f77  (song_title_flow
+000018e0: 7374 6570 2c20 6368 6172 6163 7465 7273  step, characters
+000018f0: 5f66 6c6f 7773 7465 702c 2073 6f6e 675f  _flowstep, song_
+00001900: 6c79 7269 6373 5f66 6c6f 7773 7465 7029  lyrics_flowstep)
+00001910: 0a73 6f6e 675f 7469 746c 655f 666c 6f77  .song_title_flow
+00001920: 7374 6570 2e63 6f6e 6e65 6374 2873 6f6e  step.connect(son
+00001930: 675f 6c79 7269 6373 5f66 6c6f 7773 7465  g_lyrics_flowste
+00001940: 7029 0a63 6861 7261 6374 6572 735f 666c  p).characters_fl
+00001950: 6f77 7374 6570 2e63 6f6e 6e65 6374 2873  owstep.connect(s
+00001960: 6f6e 675f 6c79 7269 6373 5f66 6c6f 7773  ong_lyrics_flows
+00001970: 7465 7029 0a0a 2320 4372 6561 7465 2061  tep)..# Create a
+00001980: 6e64 2072 756e 2046 6c6f 770a 736f 756e  nd run Flow.soun
+00001990: 6474 7261 636b 5f66 6c6f 7720 3d20 466c  dtrack_flow = Fl
+000019a0: 6f77 2874 6974 6c65 5f66 6c6f 7773 7465  ow(title_flowste
+000019b0: 7029 0a72 6573 756c 7473 203d 2073 6f75  p).results = sou
+000019c0: 6e64 7472 6163 6b5f 666c 6f77 2e73 7461  ndtrack_flow.sta
+000019d0: 7274 2874 6f70 6963 3d22 6672 6965 6e64  rt(topic="friend
+000019e0: 7368 6970 222c 2076 6572 626f 7365 3d54  ship", verbose=T
+000019f0: 7275 6529 0a60 6060 0a0a 2323 2320 4173  rue).```..### As
+00001a00: 796e 6320 466c 6f77 730a 536f 6d65 7469  ync Flows.Someti
+00001a10: 6d65 7320 6d75 6c74 6970 6c65 2066 6c6f  mes multiple flo
+00001a20: 7720 7374 6570 7320 6361 6e20 7275 6e20  w steps can run 
+00001a30: 696e 2070 6172 616c 6c65 6c20 6966 2061  in parallel if a
+00001a40: 6c6c 2074 6865 6972 2064 6570 656e 6465  ll their depende
+00001a50: 6e63 6965 7320 6172 6520 6d65 742e 200a  ncies are met. .
+00001a60: 466f 7220 6361 7365 7320 6c69 6b65 2074  For cases like t
+00001a70: 6869 732c 204c 4c4d 466c 6f77 7320 7072  his, LLMFlows pr
+00001a80: 6f76 6964 6573 2061 7379 6e63 2063 6c61  ovides async cla
+00001a90: 7373 6573 2074 6f20 696d 7072 6f76 6520  sses to improve 
+00001aa0: 7468 6520 7275 6e74 696d 6520 6f66 2061  the runtime of a
+00001ab0: 6e79 200a 636f 6d70 6c65 7820 666c 6f77  ny .complex flow
+00001ac0: 2062 7920 7275 6e6e 696e 6720 666c 6f77   by running flow
+00001ad0: 2073 7465 7073 2074 6861 7420 616c 7265   steps that alre
+00001ae0: 6164 7920 6861 7665 2061 6c6c 2074 6865  ady have all the
+00001af0: 6972 2072 6571 7569 7265 6420 696e 7075  ir required inpu
+00001b00: 7473 2069 6e20 0a70 6172 616c 6c65 6c2e  ts in .parallel.
+00001b10: 0a0a 6060 6070 7974 686f 6e0a 0a2e 2e2e  ..```python.....
+00001b20: 0a0a 6d6f 7669 655f 7469 746c 655f 666c  ..movie_title_fl
+00001b30: 6f77 7374 6570 203d 2041 7379 6e63 466c  owstep = AsyncFl
+00001b40: 6f77 5374 6570 280a 2020 2020 6e61 6d65  owStep(.    name
+00001b50: 3d22 466c 6f77 7374 6570 2031 222c 0a20  ="Flowstep 1",. 
+00001b60: 2020 206c 6c6d 3d6f 7065 6e61 695f 6c6c     llm=openai_ll
+00001b70: 6d2c 0a20 2020 2070 726f 6d70 745f 7465  m,.    prompt_te
+00001b80: 6d70 6c61 7465 3d74 6974 6c65 5f74 656d  mplate=title_tem
+00001b90: 706c 6174 652c 0a20 2020 206f 7574 7075  plate,.    outpu
+00001ba0: 745f 6b65 793d 226d 6f76 6965 5f74 6974  t_key="movie_tit
+00001bb0: 6c65 222c 0a29 0a0a 736f 6e67 5f74 6974  le",.)..song_tit
+00001bc0: 6c65 5f66 6c6f 7773 7465 7020 3d20 466c  le_flowstep = Fl
+00001bd0: 6f77 5374 6570 280a 2020 2020 6e61 6d65  owStep(.    name
+00001be0: 3d22 466c 6f77 7374 6570 2032 222c 0a20  ="Flowstep 2",. 
+00001bf0: 2020 206c 6c6d 3d6f 7065 6e61 695f 6c6c     llm=openai_ll
+00001c00: 6d2c 0a20 2020 2070 726f 6d70 745f 7465  m,.    prompt_te
+00001c10: 6d70 6c61 7465 3d73 6f6e 675f 7465 6d70  mplate=song_temp
+00001c20: 6c61 7465 2c0a 2020 2020 6f75 7470 7574  late,.    output
+00001c30: 5f6b 6579 3d22 736f 6e67 5f74 6974 6c65  _key="song_title
+00001c40: 222c 0a29 0a0a 6368 6172 6163 7465 7273  ",.)..characters
+00001c50: 5f66 6c6f 7773 7465 7020 3d20 4173 796e  _flowstep = Asyn
+00001c60: 6346 6c6f 7753 7465 7028 0a20 2020 206e  cFlowStep(.    n
+00001c70: 616d 653d 2246 6c6f 7773 7465 7020 3322  ame="Flowstep 3"
+00001c80: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
+00001c90: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
+00001ca0: 5f74 656d 706c 6174 653d 6368 6172 6163  _template=charac
+00001cb0: 7465 7273 5f74 656d 706c 6174 652c 0a20  ters_template,. 
+00001cc0: 2020 206f 7574 7075 745f 6b65 793d 226d     output_key="m
+00001cd0: 6169 6e5f 6368 6172 6163 7465 7273 222c  ain_characters",
+00001ce0: 0a29 0a0a 736f 6e67 5f6c 7972 6963 735f  .)..song_lyrics_
+00001cf0: 666c 6f77 7374 6570 203d 2041 7379 6e63  flowstep = Async
+00001d00: 466c 6f77 5374 6570 280a 2020 2020 6e61  FlowStep(.    na
+00001d10: 6d65 3d22 466c 6f77 7374 6570 2034 222c  me="Flowstep 4",
+00001d20: 0a20 2020 206c 6c6d 3d6f 7065 6e61 695f  .    llm=openai_
+00001d30: 6c6c 6d2c 0a20 2020 2070 726f 6d70 745f  llm,.    prompt_
+00001d40: 7465 6d70 6c61 7465 3d6c 7972 6963 735f  template=lyrics_
+00001d50: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
+00001d60: 7470 7574 5f6b 6579 3d22 736f 6e67 5f6c  tput_key="song_l
+00001d70: 7972 6963 7322 2c0a 290a 0a2e 2e2e 0a0a  yrics",.).......
+00001d80: 6060 600a 0a43 6865 636b 206f 7572 2064  ```..Check our d
+00001d90: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+00001da0: 206d 6f72 6520 6578 616d 706c 6573 2c20   more examples, 
+00001db0: 7375 6368 2061 7320 696e 7465 6772 6174  such as integrat
+00001dc0: 696e 6720 7665 6374 6f72 2064 6174 6162  ing vector datab
+00001dd0: 6173 6573 2c20 0a63 7265 6174 696e 6720  ases, .creating 
+00001de0: 7175 6573 7469 6f6e 2d61 6e73 7765 7269  question-answeri
+00001df0: 6e67 2061 7070 7320 616e 6420 7765 6220  ng apps and web 
+00001e00: 6170 706c 6963 6174 696f 6e73 2077 6974  applications wit
+00001e10: 6820 466c 6173 6b20 616e 6420 4661 7374  h Flask and Fast
+00001e20: 4150 492e 0a0a 2323 2046 6561 7475 7265  API...## Feature
+00001e30: 730a 0a23 2323 202a 2a4c 4c4d 732a 2a0a  s..### **LLMs**.
+00001e40: 2d20 5574 696c 697a 6520 4c4c 4d73 2073  - Utilize LLMs s
+00001e50: 7563 6820 6173 204f 7065 6e41 4927 7320  uch as OpenAI's 
+00001e60: 4368 6174 4750 5420 746f 2067 656e 6572  ChatGPT to gener
+00001e70: 6174 6520 6e61 7475 7261 6c20 6c61 6e67  ate natural lang
+00001e80: 7561 6765 2074 6578 742e 0a2d 2043 6f6e  uage text..- Con
+00001e90: 6669 6775 7265 204c 4c4d 2063 6c61 7373  figure LLM class
+00001ea0: 6573 2065 6173 696c 792c 2063 686f 6f73  es easily, choos
+00001eb0: 696e 6720 7370 6563 6966 6963 206d 6f64  ing specific mod
+00001ec0: 656c 732c 2070 6172 616d 6574 6572 732c  els, parameters,
+00001ed0: 2061 6e64 2073 6574 7469 6e67 732e 0a2d   and settings..-
+00001ee0: 2042 656e 6566 6974 2066 726f 6d20 6175   Benefit from au
+00001ef0: 746f 6d61 7469 6320 7265 7472 6965 7320  tomatic retries 
+00001f00: 7768 656e 206d 6f64 656c 2063 616c 6c73  when model calls
+00001f10: 2066 6169 6c2c 2065 6e73 7572 696e 6720   fail, ensuring 
+00001f20: 7265 6c69 6162 6c65 204c 4c4d 200a 2020  reliable LLM .  
+00001f30: 696e 7465 7261 6374 696f 6e73 2e0a 0a23  interactions...#
+00001f40: 2323 202a 2a50 726f 6d70 7420 5465 6d70  ## **Prompt Temp
+00001f50: 6c61 7465 732a 2a0a 2d20 4372 6561 7465  lates**.- Create
+00001f60: 2064 796e 616d 6963 2070 726f 6d70 7473   dynamic prompts
+00001f70: 2075 7369 6e67 2050 726f 6d70 7420 5465   using Prompt Te
+00001f80: 6d70 6c61 7465 732c 2070 726f 7669 6469  mplates, providi
+00001f90: 6e67 2066 6c65 7869 626c 6520 616e 6420  ng flexible and 
+00001fa0: 6375 7374 6f6d 697a 6162 6c65 200a 2020  customizable .  
+00001fb0: 7465 7874 2067 656e 6572 6174 696f 6e2e  text generation.
+00001fc0: 0a2d 2044 6566 696e 6520 7661 7269 6162  .- Define variab
+00001fd0: 6c65 7320 7769 7468 696e 2070 726f 6d70  les within promp
+00001fe0: 7473 2074 6f20 6765 6e65 7261 7465 2070  ts to generate p
+00001ff0: 726f 6d70 7420 7374 7269 6e67 7320 7461  rompt strings ta
+00002000: 696c 6f72 6564 2074 6f20 7370 6563 6966  ilored to specif
+00002010: 6963 200a 2020 696e 7075 7473 2e0a 0a23  ic .  inputs...#
+00002020: 2323 202a 2a46 6c6f 7773 2061 6e64 2046  ## **Flows and F
+00002030: 6c6f 7753 7465 7073 2a2a 0a2d 2053 7472  lowSteps**.- Str
+00002040: 7563 7475 7265 204c 4c4d 2061 7070 6c69  ucture LLM appli
+00002050: 6361 7469 6f6e 7320 7573 696e 6720 466c  cations using Fl
+00002060: 6f77 7320 616e 6420 466c 6f77 5374 6570  ows and FlowStep
+00002070: 732c 2070 726f 7669 6469 6e67 2061 2063  s, providing a c
+00002080: 6c65 6172 2061 6e64 206f 7267 616e 697a  lear and organiz
+00002090: 6564 2066 7261 6d65 776f 726b 2066 6f72  ed framework for
+000020a0: 2065 7865 6375 7469 6e67 204c 4c4d 2069   executing LLM i
+000020b0: 6e74 6572 6163 7469 6f6e 732e 0a2d 2043  nteractions..- C
+000020c0: 6f6e 6e65 6374 2066 6c6f 7720 7374 6570  onnect flow step
+000020d0: 7320 746f 2070 6173 7320 6f75 7470 7574  s to pass output
+000020e0: 7320 6173 2069 6e70 7574 732c 2066 6163  s as inputs, fac
+000020f0: 696c 6974 6174 696e 6720 7365 616d 6c65  ilitating seamle
+00002100: 7373 2064 6174 6120 666c 6f77 2061 6e64  ss data flow and
+00002110: 0a20 2020 206d 6169 6e74 6169 6e69 6e67  .    maintaining
+00002120: 2061 2074 7261 6e73 7061 7265 6e74 204c   a transparent L
+00002130: 4c4d 2070 6970 656c 696e 652e 0a2d 204c  LM pipeline..- L
+00002140: 6576 6572 6167 6520 4173 796e 6320 466c  everage Async Fl
+00002150: 6f77 7320 746f 2072 756e 204c 4c4d 7320  ows to run LLMs 
+00002160: 696e 2070 6172 616c 6c65 6c20 7768 656e  in parallel when
+00002170: 2061 6c6c 2074 6865 6972 2069 6e70 7574   all their input
+00002180: 7320 6172 6520 6176 6169 6c61 626c 652c  s are available,
+00002190: 200a 2020 6f70 7469 6d69 7a69 6e67 2070   .  optimizing p
+000021a0: 6572 666f 726d 616e 6365 2061 6e64 2065  erformance and e
+000021b0: 6666 6963 6965 6e63 792e 0a2d 2049 6e63  fficiency..- Inc
+000021c0: 6f72 706f 7261 7465 2063 7573 746f 6d20  orporate custom 
+000021d0: 7374 7269 6e67 206d 616e 6970 756c 6174  string manipulat
+000021e0: 696f 6e20 6675 6e63 7469 6f6e 7320 6469  ion functions di
+000021f0: 7265 6374 6c79 2069 6e74 6f20 666c 6f77  rectly into flow
+00002200: 732c 2061 6c6c 6f77 696e 6720 0a20 2073  s, allowing .  s
+00002210: 7065 6369 616c 697a 6564 2074 6578 7420  pecialized text 
+00002220: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
+00002230: 7769 7468 6f75 7420 7265 6c79 696e 6720  without relying 
+00002240: 736f 6c65 6c79 206f 6e20 4c4c 4d20 6361  solely on LLM ca
+00002250: 6c6c 732e 0a0a 2323 2320 2a2a 5665 6374  lls...### **Vect
+00002260: 6f72 5374 6f72 6520 496e 7465 6772 6174  orStore Integrat
+00002270: 696f 6e73 2a2a 0a2d 2049 6e74 6567 7261  ions**.- Integra
+00002280: 7465 2077 6974 6820 7665 6374 6f72 2064  te with vector d
+00002290: 6174 6162 6173 6573 206c 696b 6520 5069  atabases like Pi
+000022a0: 6e65 636f 6e65 2075 7369 6e67 2074 6865  necone using the
+000022b0: 2056 6563 746f 7253 746f 7265 466c 6f77   VectorStoreFlow
+000022c0: 5374 6570 2c20 0a20 2065 6d70 6f77 6572  Step, .  empower
+000022d0: 696e 6720 6566 6669 6369 656e 7420 616e  ing efficient an
+000022e0: 6420 7363 616c 6162 6c65 2073 746f 7261  d scalable stora
+000022f0: 6765 2061 6e64 2072 6574 7269 6576 616c  ge and retrieval
+00002300: 206f 6620 7665 6374 6f72 2065 6d62 6564   of vector embed
+00002310: 6469 6e67 732e 0a2d 204c 6576 6572 6167  dings..- Leverag
+00002320: 6520 7665 6374 6f72 2064 6174 6162 6173  e vector databas
+00002330: 6573 2066 6f72 2073 6561 6d6c 6573 7320  es for seamless 
+00002340: 7374 6f72 6167 6520 616e 6420 7175 6572  storage and quer
+00002350: 7969 6e67 206f 6620 7665 6374 6f72 732c  ying of vectors,
+00002360: 2065 6e61 626c 696e 6720 7374 7261 6967   enabling straig
+00002370: 6874 666f 7277 6172 6420 696e 7465 6772  htforward integr
+00002380: 6174 696f 6e20 7769 7468 204c 4c4d 2d70  ation with LLM-p
+00002390: 6f77 6572 6564 2061 7070 6c69 6361 7469  owered applicati
+000023a0: 6f6e 732e 0a0a 2323 2320 2a2a 4361 6c6c  ons...### **Call
+000023b0: 6261 636b 732a 2a0a 2d20 4578 6563 7574  backs**.- Execut
+000023c0: 6520 6361 6c6c 6261 636b 2066 756e 6374  e callback funct
+000023d0: 696f 6e73 2061 7420 6469 6666 6572 656e  ions at differen
+000023e0: 7420 7374 6167 6573 2077 6974 6869 6e20  t stages within 
+000023f0: 666c 6f77 2073 7465 7073 2c20 656e 6162  flow steps, enab
+00002400: 6c69 6e67 2065 6e68 616e 6365 6420 6375  ling enhanced cu
+00002410: 7374 6f6d 697a 6174 696f 6e2c 206c 6f67  stomization, log
+00002420: 6769 6e67 2c20 7472 6163 696e 672c 206f  ging, tracing, o
+00002430: 7220 6f74 6865 7220 7370 6563 6966 6963  r other specific
+00002440: 2069 6e74 6567 7261 7469 6f6e 732e 0a2d   integrations..-
+00002450: 2055 7469 6c69 7a65 2063 616c 6c62 6163   Utilize callbac
+00002460: 6b73 2074 6f20 636f 6d70 7265 6865 6e73  ks to comprehens
+00002470: 6976 656c 7920 636f 6e74 726f 6c20 616e  ively control an
+00002480: 6420 6d6f 6e69 746f 7220 4c4c 4d2d 706f  d monitor LLM-po
+00002490: 7765 7265 6420 6170 7073 2c20 656e 7375  wered apps, ensu
+000024a0: 7269 6e67 200a 2020 636c 6561 7220 7669  ring .  clear vi
+000024b0: 7369 6269 6c69 7479 2069 6e74 6f20 7468  sibility into th
+000024c0: 6520 6578 6563 7574 696f 6e20 7072 6f63  e execution proc
+000024d0: 6573 732e 0a0a 2323 2320 2a2a 4578 706c  ess...### **Expl
+000024e0: 6963 6974 2041 5049 2061 6e64 2046 756c  icit API and Ful
+000024f0: 6c20 5472 616e 7370 6172 656e 6379 2a2a  l Transparency**
+00002500: 0a57 6974 6820 4c4c 4d46 6c6f 7773 2079  .With LLMFlows y
+00002510: 6f75 2068 6176 6520 7468 6520 6675 6c6c  ou have the full
+00002520: 2063 6f6e 7472 6f6c 2074 6f20 6372 6561   control to crea
+00002530: 7465 2065 7870 6c69 6369 7420 6170 706c  te explicit appl
+00002540: 6963 6174 696f 6e73 2077 6974 686f 7574  ications without
+00002550: 2061 6e79 2068 6964 6465 6e20 7072 6f6d   any hidden prom
+00002560: 7074 7320 6f72 2070 7265 6465 6669 6e65  pts or predefine
+00002570: 6420 6265 6861 7669 6f72 732e 0a0a 496e  d behaviors...In
+00002580: 2061 6464 6974 696f 6e20 4c4c 4d46 6c6f   addition LLMFlo
+00002590: 7773 2061 6c6c 6f77 7320 796f 7520 746f  ws allows you to
+000025a0: 2061 6e73 7765 7220 7175 6573 7469 6f6e   answer question
+000025b0: 7320 7375 6368 2061 733a 0a0a 2d20 5768  s such as:..- Wh
+000025c0: 656e 2077 6173 2061 2070 6172 7469 6375  en was a particu
+000025d0: 6c61 7220 666c 6f77 7374 6570 2072 756e  lar flowstep run
+000025e0: 3f0a 2d20 486f 7720 6d75 6368 2074 696d  ?.- How much tim
+000025f0: 6520 6469 6420 6974 2074 616b 653f 0a2d  e did it take?.-
+00002600: 2057 6861 7420 7765 7265 2074 6865 2069   What were the i
+00002610: 6e70 7574 2076 6172 6961 626c 6573 3f0a  nput variables?.
+00002620: 2d20 5768 6174 2077 6173 2074 6865 2070  - What was the p
+00002630: 726f 6d70 7420 7465 6d70 6c61 7465 3f0a  rompt template?.
+00002640: 2d20 5768 6174 2064 6964 2074 6865 2070  - What did the p
+00002650: 726f 6d70 7420 6c6f 6f6b 206c 696b 653f  rompt look like?
+00002660: 0a2d 2057 6861 7420 7761 7320 7468 6520  .- What was the 
+00002670: 6578 6163 7420 636f 6e66 6967 7572 6174  exact configurat
+00002680: 696f 6e20 6f66 2074 6865 206d 6f64 656c  ion of the model
+00002690: 3f0a 2d20 486f 7720 6d61 6e79 2074 696d  ?.- How many tim
+000026a0: 6573 2064 6964 2077 6520 7265 7472 7920  es did we retry 
+000026b0: 7468 6520 7265 7175 6573 743f 0a2d 2057  the request?.- W
+000026c0: 6861 7420 7761 7320 7468 6520 7261 7720  hat was the raw 
+000026d0: 6461 7461 2074 6865 2041 5049 2072 6574  data the API ret
+000026e0: 7572 6e65 643f 0a2d 2048 6f77 206d 616e  urned?.- How man
+000026f0: 7920 746f 6b65 6e73 2077 6572 6520 7573  y tokens were us
+00002700: 6564 3f0a 2d20 5768 6174 2077 6173 2074  ed?.- What was t
+00002710: 6865 2066 696e 616c 2072 6573 756c 743f  he final result?
+00002720: 0a0a 2323 204c 6963 656e 7365 0a4c 4c4d  ..## License.LLM
+00002730: 466c 6f77 7320 6973 2063 6f76 6572 6564  Flows is covered
+00002740: 2062 7920 7468 6520 4d49 5420 6c69 6365   by the MIT lice
+00002750: 6e73 652e 2046 6f72 206d 6f72 6520 696e  nse. For more in
+00002760: 666f 726d 6174 696f 6e2c 2063 6865 636b  formation, check
+00002770: 2060 4c49 4345 4e43 452e 6d64 602e 0a0a   `LICENCE.md`...
+00002780: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00002790: 5468 616e 6b20 796f 7520 666f 7220 7370  Thank you for sp
+000027a0: 656e 6469 6e67 2074 696d 6520 676f 696e  ending time goin
+000027b0: 6720 6f76 6572 206f 7572 2052 4541 444d  g over our READM
+000027c0: 4521 2049 6620 796f 7520 6669 6e64 204c  E! If you find L
+000027d0: 4c4d 466c 6f77 7320 6578 6369 7469 6e67  LMFlows exciting
+000027e0: 2061 6e64 200a 796f 7520 6172 6520 636f   and .you are co
+000027f0: 6e73 6964 6572 696e 6720 636f 6e74 7269  nsidering contri
+00002800: 6275 7469 6e67 2c20 706c 6561 7365 2063  buting, please c
+00002810: 6865 636b 205b 6043 4f4e 5452 4942 5554  heck [`CONTRIBUT
+00002820: 494e 472e 6d64 605d 2868 7474 7073 3a2f  ING.md`](https:/
+00002830: 2f67 6974 6875 622e 636f 6d2f 7374 6f79  /github.com/stoy
+00002840: 616e 2d73 746f 7961 6e6f 762f 6c6c 6d66  an-stoyanov/llmf
+00002850: 6c6f 7773 2f62 6c6f 622f 6d61 696e 2f43  lows/blob/main/C
+00002860: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+00002870: 0a                                       .
```

### Comparing `llmflows-0.0.8/README.md` & `llmflows-0.0.9/llmflows.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,599 +1,648 @@
-00000000: 2320 4c4c 4d46 6c6f 7773 202d 2053 696d  # LLMFlows - Sim
-00000010: 706c 652c 2045 7870 6c69 6369 742c 2061  ple, Explicit, a
-00000020: 6e64 2054 7261 6e73 7061 7265 6e74 204c  nd Transparent L
-00000030: 4c4d 2041 7070 730a 0a3c 7020 616c 6967  LM Apps..<p alig
-00000040: 6e3d 2263 656e 7465 7222 3e0a 2020 3c69  n="center">.  <i
-00000050: 6d67 2073 7479 6c65 3d22 7769 6474 683a  mg style="width:
-00000060: 2038 3025 2220 7372 633d 2264 6f63 732f   80%" src="docs/
-00000070: 6c6c 6d66 6c6f 7773 5f6c 6173 745f 6c6f  llmflows_last_lo
-00000080: 676f 2e70 6e67 2220 2f3e 0a3c 2f70 3e0a  go.png" />.</p>.
-00000090: 0a5b 215b 5477 6974 7465 725d 2868 7474  .[![Twitter](htt
-000000a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000000b0: 2e69 6f2f 7477 6974 7465 722f 666f 6c6c  .io/twitter/foll
-000000c0: 6f77 2f4c 4c4d 466c 6f77 733f 7374 796c  ow/LLMFlows?styl
-000000d0: 653d 736f 6369 616c 295d 2868 7474 7073  e=social)](https
-000000e0: 3a2f 2f74 7769 7474 6572 2e63 6f6d 2f4c  ://twitter.com/L
-000000f0: 4c4d 466c 6f77 7329 0a21 5b50 796c 696e  LMFlows).![Pylin
-00000100: 7420 776f 726b 666c 6f77 5d28 6874 7470  t workflow](http
-00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000120: 746f 7961 6e2d 7374 6f79 616e 6f76 2f6c  toyan-stoyanov/l
-00000130: 6c6d 666c 6f77 2f61 6374 696f 6e73 2f77  lmflow/actions/w
-00000140: 6f72 6b66 6c6f 7773 2f70 796c 696e 742e  orkflows/pylint.
-00000150: 796d 6c2f 6261 6467 652e 7376 6729 0a21  yml/badge.svg).!
-00000160: 5b4c 6963 656e 7365 5d28 6874 7470 733a  [License](https:
-00000170: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000180: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
-00000190: 7374 6f79 616e 2d73 746f 7961 6e6f 762f  stoyan-stoyanov/
-000001a0: 6c6c 6d66 6c6f 7729 0a21 5b50 7950 695d  llmflow).![PyPi]
-000001b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000001c0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f6c  elds.io/pypi/v/l
-000001d0: 6c6d 666c 6f77 7329 0a21 5b53 7461 7273  lmflows).![Stars
-000001e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000001f0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000200: 7374 6172 732f 7374 6f79 616e 2d73 746f  stars/stoyan-sto
-00000210: 7961 6e6f 762f 6c6c 6d66 6c6f 773f 7374  yanov/llmflow?st
-00000220: 796c 653d 736f 6369 616c 290a 215b 5265  yle=social).![Re
-00000230: 6c65 6173 6520 6461 7465 5d28 6874 7470  lease date](http
-00000240: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000250: 696f 2f67 6974 6875 622f 7265 6c65 6173  io/github/releas
-00000260: 652d 6461 7465 2f73 746f 7961 6e2d 7374  e-date/stoyan-st
-00000270: 6f79 616e 6f76 2f6c 6c6d 666c 6f77 3f73  oyanov/llmflow?s
-00000280: 7479 6c65 3d73 6f63 6961 6c29 0a0a 446f  tyle=social)..Do
-00000290: 6375 6d65 6e74 6174 696f 6e3a 205b 6874  cumentation: [ht
-000002a0: 7470 733a 2f2f 7265 6164 7468 6564 6f63  tps://readthedoc
-000002b0: 732e 6f72 675d 2868 7474 7073 3a2f 2f72  s.org](https://r
-000002c0: 6561 6474 6865 646f 6373 2e6f 7267 2f29  eadthedocs.org/)
-000002d0: 3c62 722f 3e0a 5079 5049 3a20 5b68 7474  <br/>.PyPI: [htt
-000002e0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000002f0: 6f6a 6563 742f 6c6c 6d66 6c6f 7773 5d28  oject/llmflows](
-00000300: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000310: 2f70 726f 6a65 6374 2f6c 6c6d 666c 6f77  /project/llmflow
-00000320: 732f 293c 2f62 723e 0a54 7769 7474 6572  s/)</br>.Twitter
-00000330: 3a20 5b68 7474 7073 3a2f 2f74 7769 7474  : [https://twitt
-00000340: 6572 2e63 6f6d 2f4c 4c4d 466c 6f77 735d  er.com/LLMFlows]
-00000350: 2868 7474 7073 3a2f 2f74 7769 7474 6572  (https://twitter
-00000360: 2e63 6f6d 2f4c 4c4d 466c 6f77 7329 3c62  .com/LLMFlows)<b
-00000370: 722f 3e0a 5375 6273 7461 636b 3a20 5b68  r/>.Substack: [h
-00000380: 7474 7073 3a2f 2f6c 6c6d 666c 6f77 732e  ttps://llmflows.
-00000390: 7375 6273 7461 636b 2e63 6f6d 5d28 6874  substack.com](ht
-000003a0: 7470 733a 2f2f 6c6c 6d66 6c6f 7773 2e73  tps://llmflows.s
-000003b0: 7562 7374 6163 6b2e 636f 6d2f 293c 6272  ubstack.com/)<br
-000003c0: 2f3e 0a0a 2323 2041 626f 7574 0a4c 4c4d  />..## About.LLM
-000003d0: 466c 6f77 7320 6973 2061 2066 7261 6d65  Flows is a frame
-000003e0: 776f 726b 2066 6f72 2062 7569 6c64 696e  work for buildin
-000003f0: 6720 7369 6d70 6c65 2c20 6578 706c 6963  g simple, explic
-00000400: 6974 2c20 616e 6420 7472 616e 7370 6172  it, and transpar
-00000410: 656e 7420 4c4c 4d28 4c61 7267 6520 0a4c  ent LLM(Large .L
-00000420: 616e 6775 6167 6520 4d6f 6465 6c29 2061  anguage Model) a
-00000430: 7070 6c69 6361 7469 6f6e 732e 0a0a 2323  pplications...##
-00000440: 2049 6e73 7461 6c6c 6174 696f 6e0a 6060   Installation.``
-00000450: 600a 7069 7020 696e 7374 616c 6c20 6c6c  `.pip install ll
-00000460: 6d66 6c6f 7773 0a60 6060 0a0a 2323 2050  mflows.```..## P
-00000470: 6869 6c6f 736f 7068 790a 0a23 2323 202a  hilosophy..### *
-00000480: 2a53 696d 706c 652a 2a0a 4f75 7220 676f  *Simple**.Our go
-00000490: 616c 2069 7320 746f 2062 7569 6c64 2061  al is to build a
-000004a0: 2073 696d 706c 652c 2077 656c 6c2d 646f   simple, well-do
-000004b0: 6375 6d65 6e74 6564 2066 7261 6d65 776f  cumented framewo
-000004c0: 726b 2077 6974 6820 6d69 6e69 6d61 6c20  rk with minimal 
-000004d0: 6162 7374 7261 6374 696f 6e73 2074 6861  abstractions tha
-000004e0: 7420 0a61 6c6c 6f77 2075 7365 7273 2074  t .allow users t
-000004f0: 6f20 6275 696c 6420 666c 6578 6962 6c65  o build flexible
-00000500: 204c 4c4d 2d70 6f77 6572 6564 2061 7070   LLM-powered app
-00000510: 7320 7769 7468 6f75 7420 636f 6d70 726f  s without compro
-00000520: 6d69 7369 6e67 206f 6e20 6361 7061 6269  mising on capabi
-00000530: 6c69 7469 6573 2e0a 0a23 2323 202a 2a45  lities...### **E
-00000540: 7870 6c69 6369 742a 2a0a 5765 2077 616e  xplicit**.We wan
-00000550: 7420 746f 2063 7265 6174 6520 616e 2065  t to create an e
-00000560: 7870 6c69 6369 7420 4150 4920 656e 6162  xplicit API enab
-00000570: 6c69 6e67 2075 7365 7273 2074 6f20 7772  ling users to wr
-00000580: 6974 6520 636c 6561 6e20 616e 6420 7265  ite clean and re
-00000590: 6164 6162 6c65 2063 6f64 6520 7768 696c  adable code whil
-000005a0: 6520 0a65 6173 696c 7920 6372 6561 7469  e .easily creati
-000005b0: 6e67 2063 6f6d 706c 6578 2066 6c6f 7773  ng complex flows
-000005c0: 206f 6620 4c4c 4d73 2069 6e74 6572 6163   of LLMs interac
-000005d0: 7469 6e67 2077 6974 6820 6561 6368 206f  ting with each o
-000005e0: 7468 6572 2e20 4c4c 4d46 6c6f 7773 2720  ther. LLMFlows' 
-000005f0: 636c 6173 7365 7320 0a67 6976 6520 7573  classes .give us
-00000600: 6572 7320 6675 6c6c 2063 6f6e 7472 6f6c  ers full control
-00000610: 2061 6e64 2064 6f20 6e6f 7420 6861 7665   and do not have
-00000620: 2061 6e79 2068 6964 6465 6e20 7072 6f6d   any hidden prom
-00000630: 7074 7320 6f72 204c 4c4d 2063 616c 6c73  pts or LLM calls
-00000640: 2e20 0a0a 2323 2320 2a2a 5472 616e 7370  . ..### **Transp
-00000650: 6172 656e 742a 2a0a 5765 2061 696d 2074  arent**.We aim t
-00000660: 6f20 6865 6c70 2075 7365 7273 2068 6176  o help users hav
-00000670: 6520 6675 6c6c 2074 7261 6e73 7061 7265  e full transpare
-00000680: 6e63 7920 6f6e 2074 6865 6972 204c 4c4d  ncy on their LLM
-00000690: 2d70 6f77 6572 6564 2061 7070 7320 6279  -powered apps by
-000006a0: 2070 726f 7669 6469 6e67 200a 7472 6163   providing .trac
-000006b0: 6561 626c 6520 666c 6f77 7320 616e 6420  eable flows and 
-000006c0: 636f 6d70 6c65 7465 2069 6e66 6f72 6d61  complete informa
-000006d0: 7469 6f6e 2066 6f72 2065 6163 6820 6170  tion for each ap
-000006e0: 7020 636f 6d70 6f6e 656e 742c 206d 616b  p component, mak
-000006f0: 696e 6720 6974 2065 6173 7920 746f 200a  ing it easy to .
-00000700: 6d6f 6e69 746f 722c 206d 6169 6e74 6169  monitor, maintai
-00000710: 6e2c 2061 6e64 2064 6562 7567 2e0a 0a23  n, and debug...#
-00000720: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
-00000730: 640a 2323 2320 4c4c 4d73 0a4c 4c4d 7320  d.### LLMs.LLMs 
-00000740: 6172 6520 6f6e 6520 6f66 2074 6865 206d  are one of the m
-00000750: 6169 6e20 6162 7374 7261 6374 696f 6e73  ain abstractions
-00000760: 2069 6e20 4c4c 4d46 6c6f 7773 2e20 4c4c   in LLMFlows. LL
-00000770: 4d20 636c 6173 7365 7320 6172 6520 7772  M classes are wr
-00000780: 6170 7065 7273 2061 726f 756e 6420 4c4c  appers around LL
-00000790: 4d20 0a41 5049 7320 7375 6368 2061 7320  M .APIs such as 
-000007a0: 4f70 656e 4149 2773 2041 5049 732e 2054  OpenAI's APIs. T
-000007b0: 6865 7920 7072 6f76 6964 6520 6d65 7468  hey provide meth
-000007c0: 6f64 7320 666f 7220 636f 6e66 6967 7572  ods for configur
-000007d0: 696e 6720 616e 6420 6361 6c6c 696e 6720  ing and calling 
-000007e0: 7468 6573 6520 4150 4973 2c20 0a72 6574  these APIs, .ret
-000007f0: 7279 696e 6720 6661 696c 6564 2063 616c  rying failed cal
-00000800: 6c73 2c20 616e 6420 666f 726d 6174 7469  ls, and formatti
-00000810: 6e67 2074 6865 2072 6573 706f 6e73 6573  ng the responses
-00000820: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
-00000830: 6d20 6c6c 6d66 6c6f 7773 2e6c 6c6d 7320  m llmflows.llms 
-00000840: 696d 706f 7274 204f 7065 6e41 490a 0a6c  import OpenAI..l
-00000850: 6c6d 203d 204f 7065 6e41 4928 6170 695f  lm = OpenAI(api_
-00000860: 6b65 793d 223c 796f 7572 2d6f 7065 6e61  key="<your-opena
-00000870: 692d 6170 692d 6b65 793e 2229 0a0a 7265  i-api-key>")..re
-00000880: 7375 6c74 2c20 6361 6c6c 5f64 6174 612c  sult, call_data,
-00000890: 206d 6f64 656c 5f63 6f6e 6669 6720 3d20   model_config = 
-000008a0: 6c6c 6d2e 6765 6e65 7261 7465 280a 2020  llm.generate(.  
-000008b0: 2070 726f 6d70 743d 2247 656e 6572 6174   prompt="Generat
-000008c0: 6520 6120 636f 6f6c 2074 6974 6c65 2066  e a cool title f
-000008d0: 6f72 2061 6e20 3830 7320 726f 636b 2073  or an 80s rock s
-000008e0: 6f6e 6722 0a29 0a60 6060 0a0a 0a23 2323  ong".).```...###
-000008f0: 2050 726f 6d70 7454 656d 706c 6174 6573   PromptTemplates
-00000900: 0a54 6865 2060 5072 6f6d 7074 5465 6d70  .The `PromptTemp
-00000910: 6c61 7465 6020 636c 6173 7320 616c 6c6f  late` class allo
-00000920: 7773 2075 7320 746f 2063 7265 6174 6520  ws us to create 
-00000930: 7374 7269 6e67 7320 7769 7468 2076 6172  strings with var
-00000940: 6961 626c 6573 2074 6861 7420 7765 2063  iables that we c
-00000950: 616e 2066 696c 6c20 0a69 6e20 6479 6e61  an fill .in dyna
-00000960: 6d69 6361 6c6c 7920 6c61 7465 7220 6f6e  mically later on
-00000970: 2e20 4f6e 6365 2061 2070 726f 6d70 7420  . Once a prompt 
-00000980: 7465 6d70 6c61 7465 206f 626a 6563 7420  template object 
-00000990: 6973 2063 7265 6174 6564 2061 6e20 6163  is created an ac
-000009a0: 7475 616c 2070 726f 6d70 7420 6361 6e20  tual prompt can 
-000009b0: 0a62 6520 6765 6e65 7261 7465 6420 6279  .be generated by
-000009c0: 2070 726f 7669 6469 6e67 2074 6865 2072   providing the r
-000009d0: 6571 7569 7265 6420 7661 7269 6162 6c65  equired variable
-000009e0: 732e 0a0a 6060 6070 7974 686f 6e0a 6672  s...```python.fr
-000009f0: 6f6d 206c 6c6d 666c 6f77 732e 6c6c 6d73  om llmflows.llms
-00000a00: 2069 6d70 6f72 7420 4f70 656e 4149 0a66   import OpenAI.f
-00000a10: 726f 6d20 6c6c 6d66 6c6f 7773 2e70 726f  rom llmflows.pro
-00000a20: 6d70 7473 2069 6d70 6f72 7420 5072 6f6d  mpts import Prom
-00000a30: 7074 5465 6d70 6c61 7465 0a0a 0a70 726f  ptTemplate...pro
-00000a40: 6d70 745f 7465 6d70 6c61 7465 203d 2050  mpt_template = P
-00000a50: 726f 6d70 7454 656d 706c 6174 6528 0a20  romptTemplate(. 
-00000a60: 2020 2070 726f 6d70 743d 2247 656e 6572     prompt="Gener
-00000a70: 6174 6520 6120 7469 746c 6520 666f 7220  ate a title for 
-00000a80: 6120 3930 7320 6869 702d 686f 7020 736f  a 90s hip-hop so
-00000a90: 6e67 2061 626f 7574 207b 746f 7069 637d  ng about {topic}
-00000aa0: 2e22 0a29 0a6c 6c6d 5f70 726f 6d70 7420  .".).llm_prompt 
-00000ab0: 3d20 7072 6f6d 7074 5f74 656d 706c 6174  = prompt_templat
-00000ac0: 652e 6765 745f 7072 6f6d 7074 2874 6f70  e.get_prompt(top
-00000ad0: 6963 3d22 6672 6965 6e64 7368 6970 2229  ic="friendship")
-00000ae0: 0a0a 7072 696e 7428 6c6c 6d5f 7072 6f6d  ..print(llm_prom
-00000af0: 7074 290a 0a6c 6c6d 203d 204f 7065 6e41  pt)..llm = OpenA
-00000b00: 4928 6170 695f 6b65 793d 223c 796f 7572  I(api_key="<your
-00000b10: 2d6f 7065 6e61 692d 6170 692d 6b65 793e  -openai-api-key>
-00000b20: 2229 0a73 6f6e 675f 7469 746c 6520 3d20  ").song_title = 
-00000b30: 6c6c 6d2e 6765 6e65 7261 7465 286c 6c6d  llm.generate(llm
-00000b40: 5f70 726f 6d70 7429 0a0a 7072 696e 7428  _prompt)..print(
-00000b50: 736f 6e67 5f74 6974 6c65 290a 6060 600a  song_title).```.
-00000b60: 0a23 2323 2043 6861 7420 4c4c 4d73 0a55  .### Chat LLMs.U
-00000b70: 6e6c 696b 6520 7265 6775 6c61 7220 4c4c  nlike regular LL
-00000b80: 4d73 2074 6861 7420 6f6e 6c79 2072 6571  Ms that only req
-00000b90: 7569 7265 2061 2070 726f 6d70 7420 746f  uire a prompt to
-00000ba0: 2067 656e 6572 6174 6520 7465 7874 2c20   generate text, 
-00000bb0: 6368 6174 204c 4c4d 7320 7265 7175 6972  chat LLMs requir
-00000bc0: 6520 6120 0a63 6f6e 7665 7273 6174 696f  e a .conversatio
-00000bd0: 6e20 6869 7374 6f72 792e 2054 6865 2063  n history. The c
-00000be0: 6f6e 7665 7273 6174 696f 6e20 6869 7374  onversation hist
-00000bf0: 6f72 7920 6973 2072 6570 7265 7365 6e74  ory is represent
-00000c00: 6564 200a 6173 2061 206c 6973 7420 6f66  ed .as a list of
-00000c10: 206d 6573 7361 6765 7320 6265 7477 6565   messages betwee
-00000c20: 6e20 6120 7573 6572 2061 6e64 2061 6e20  n a user and an 
-00000c30: 6173 7369 7374 616e 742e 2054 6869 7320  assistant. This 
-00000c40: 636f 6e76 6572 7361 7469 6f6e 2068 6973  conversation his
-00000c50: 746f 7279 2069 7320 0a73 656e 7420 746f  tory is .sent to
-00000c60: 2074 6865 206d 6f64 656c 2c20 616e 6420   the model, and 
-00000c70: 6120 6e65 7720 6d65 7373 6167 6520 6973  a new message is
-00000c80: 2067 656e 6572 6174 6564 2062 6173 6564   generated based
-00000c90: 206f 6e20 6974 2e0a 0a4c 4c4d 466c 6f77   on it...LLMFlow
-00000ca0: 7320 7072 6f76 6964 6573 2061 2060 4d65  s provides a `Me
-00000cb0: 7373 6167 6548 6973 746f 7279 6020 636c  ssageHistory` cl
-00000cc0: 6173 7320 746f 206d 616e 6167 6520 7468  ass to manage th
-00000cd0: 6520 7265 7175 6972 6564 2063 6f6e 7665  e required conve
-00000ce0: 7273 6174 696f 6e20 6869 7374 6f72 7920  rsation history 
-00000cf0: 0a66 6f72 2063 6861 7420 4c4c 4d73 2e0a  .for chat LLMs..
-00000d00: 0a59 6f75 2063 616e 2062 7569 6c64 2061  .You can build a
-00000d10: 2073 696d 706c 6520 6368 6174 626f 7420   simple chatbot 
-00000d20: 6279 2075 7369 6e67 2074 6865 2060 4f70  by using the `Op
-00000d30: 656e 4149 4368 6174 6020 616e 6420 604d  enAIChat` and `M
-00000d40: 6573 7361 6765 4869 7374 6f72 7960 2063  essageHistory` c
-00000d50: 6c61 7373 6573 3a0a 0a60 6060 7079 7468  lasses:..```pyth
-00000d60: 6f6e 0a66 726f 6d20 6c6c 6d66 6c6f 7773  on.from llmflows
-00000d70: 2e6c 6c6d 7320 696d 706f 7274 204f 7065  .llms import Ope
-00000d80: 6e41 4943 6861 742c 204d 6573 7361 6765  nAIChat, Message
-00000d90: 4869 7374 6f72 790a 0a6c 6c6d 203d 204f  History..llm = O
-00000da0: 7065 6e41 4943 6861 7428 6170 695f 6b65  penAIChat(api_ke
-00000db0: 793d 223c 796f 7572 2d6f 7065 6e61 692d  y="<your-openai-
-00000dc0: 6170 692d 6b65 793e 2229 0a6d 6573 7361  api-key>").messa
-00000dd0: 6765 5f68 6973 746f 7279 203d 204d 6573  ge_history = Mes
-00000de0: 7361 6765 4869 7374 6f72 7928 290a 0a77  sageHistory()..w
-00000df0: 6869 6c65 2054 7275 653a 0a20 2020 2075  hile True:.    u
-00000e00: 7365 725f 6d65 7373 6167 6520 3d20 696e  ser_message = in
-00000e10: 7075 7428 2259 6f75 3a22 290a 2020 2020  put("You:").    
-00000e20: 6d65 7373 6167 655f 6869 7374 6f72 792e  message_history.
-00000e30: 6164 645f 7573 6572 5f6d 6573 7361 6765  add_user_message
-00000e40: 2875 7365 725f 6d65 7373 6167 6529 0a0a  (user_message)..
-00000e50: 2020 2020 6c6c 6d5f 7265 7370 6f6e 7365      llm_response
-00000e60: 2c20 6361 6c6c 5f64 6174 612c 206d 6f64  , call_data, mod
-00000e70: 656c 5f63 6f6e 6669 6720 3d20 6c6c 6d2e  el_config = llm.
-00000e80: 6765 6e65 7261 7465 286d 6573 7361 6765  generate(message
-00000e90: 5f68 6973 746f 7279 290a 2020 2020 6d65  _history).    me
-00000ea0: 7373 6167 655f 6869 7374 6f72 792e 6164  ssage_history.ad
-00000eb0: 645f 6169 5f6d 6573 7361 6765 286c 6c6d  d_ai_message(llm
-00000ec0: 5f72 6573 706f 6e73 6529 0a0a 2020 2020  _response)..    
-00000ed0: 7072 696e 7428 6622 4c4c 4d3a 207b 6c6c  print(f"LLM: {ll
-00000ee0: 6d5f 7265 7370 6f6e 7365 7d22 290a 6060  m_response}").``
-00000ef0: 600a 0a23 2323 204c 4c4d 2046 6c6f 7773  `..### LLM Flows
-00000f00: 0a4f 6674 656e 2074 696d 6573 2c20 7265  .Often times, re
-00000f10: 616c 2d77 6f72 6c64 2061 7070 6c69 6361  al-world applica
-00000f20: 7469 6f6e 7320 6361 6e20 6265 206d 6f72  tions can be mor
-00000f30: 6520 636f 6d70 6c65 7820 616e 6420 6361  e complex and ca
-00000f40: 6e20 6861 7665 2064 6570 656e 6465 6e63  n have dependenc
-00000f50: 6965 7320 0a62 6574 7765 656e 2070 726f  ies .between pro
-00000f60: 6d70 7473 2061 6e64 204c 4c4d 2063 616c  mpts and LLM cal
-00000f70: 6c73 2e20 466f 7220 6578 616d 706c 653a  ls. For example:
-00000f80: 0a0a 215b 436f 6d70 6c65 7820 666c 6f77  ..![Complex flow
-00000f90: 5d28 646f 6373 2f63 6f6d 706c 6578 5f66  ](docs/complex_f
-00000fa0: 6c6f 772e 706e 6729 0a0a 5768 656e 2079  low.png)..When y
-00000fb0: 6f75 2077 616e 7420 746f 2062 7569 6c64  ou want to build
-00000fc0: 2061 7070 7320 7769 7468 2063 6f6d 706c   apps with compl
-00000fd0: 6578 2064 6570 656e 6465 6e63 6965 7320  ex dependencies 
-00000fe0: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-00000ff0: 6046 6c6f 7760 2061 6e64 200a 6046 6c6f  `Flow` and .`Flo
-00001000: 7773 7465 7060 2063 6c61 7373 6573 2e20  wstep` classes. 
-00001010: 4c4c 4d46 6c6f 7773 2077 696c 6c20 6669  LLMFlows will fi
-00001020: 6775 7265 206f 7574 2074 6865 2064 6570  gure out the dep
-00001030: 656e 6465 6e63 6965 7320 616e 6420 6d61  endencies and ma
-00001040: 6b65 2073 7572 6520 6561 6368 200a 666c  ke sure each .fl
-00001050: 6f77 7374 6570 2072 756e 7320 6f6e 6c79  owstep runs only
-00001060: 2077 6865 6e20 616c 6c20 6974 7320 6465   when all its de
-00001070: 7065 6e64 656e 6369 6573 2061 7265 206d  pendencies are m
-00001080: 6574 3a0a 0a60 6060 7079 7468 6f6e 0a66  et:..```python.f
-00001090: 726f 6d20 6c6c 6d66 6c6f 7773 2e66 6c6f  rom llmflows.flo
-000010a0: 7773 2069 6d70 6f72 7420 466c 6f77 2c20  ws import Flow, 
-000010b0: 466c 6f77 5374 6570 0a66 726f 6d20 6c6c  FlowStep.from ll
-000010c0: 6d66 6c6f 7773 2e6c 6c6d 7320 696d 706f  mflows.llms impo
-000010d0: 7274 204f 7065 6e41 490a 6672 6f6d 206c  rt OpenAI.from l
-000010e0: 6c6d 666c 6f77 732e 7072 6f6d 7074 7320  lmflows.prompts 
-000010f0: 696d 706f 7274 2050 726f 6d70 7454 656d  import PromptTem
-00001100: 706c 6174 650a 0a6f 7065 6e61 695f 6c6c  plate..openai_ll
-00001110: 6d20 3d20 4f70 656e 4149 2861 7069 5f6b  m = OpenAI(api_k
-00001120: 6579 3d22 3c79 6f75 722d 6f70 656e 6169  ey="<your-openai
-00001130: 2d61 7069 2d6b 6579 3e22 290a 0a23 2043  -api-key>")..# C
-00001140: 7265 6174 6520 7072 6f6d 7074 2074 656d  reate prompt tem
-00001150: 706c 6174 6573 0a74 6974 6c65 5f74 656d  plates.title_tem
-00001160: 706c 6174 6520 3d20 5072 6f6d 7074 5465  plate = PromptTe
-00001170: 6d70 6c61 7465 2822 5768 6174 2069 7320  mplate("What is 
-00001180: 6120 676f 6f64 2074 6974 6c65 206f 6620  a good title of 
-00001190: 6120 6d6f 7669 6520 6162 6f75 7420 7b74  a movie about {t
-000011a0: 6f70 6963 7d3f 2229 0a73 6f6e 675f 7465  opic}?").song_te
-000011b0: 6d70 6c61 7465 203d 2050 726f 6d70 7454  mplate = PromptT
-000011c0: 656d 706c 6174 6528 0a20 2020 2022 5768  emplate(.    "Wh
-000011d0: 6174 2069 7320 6120 676f 6f64 2073 6f6e  at is a good son
-000011e0: 6720 7469 746c 6520 6f66 2061 2073 6f75  g title of a sou
-000011f0: 6e64 7472 6163 6b20 666f 7220 6120 6d6f  ndtrack for a mo
-00001200: 7669 6520 6361 6c6c 6564 207b 6d6f 7669  vie called {movi
-00001210: 655f 7469 746c 657d 3f22 0a29 0a63 6861  e_title}?".).cha
-00001220: 7261 6374 6572 735f 7465 6d70 6c61 7465  racters_template
-00001230: 203d 2050 726f 6d70 7454 656d 706c 6174   = PromptTemplat
-00001240: 6528 0a20 2020 2022 5768 6174 2061 7265  e(.    "What are
-00001250: 2074 776f 206d 6169 6e20 6368 6172 6163   two main charac
-00001260: 7465 7273 2066 6f72 2061 206d 6f76 6965  ters for a movie
-00001270: 2063 616c 6c65 6420 7b6d 6f76 6965 5f74   called {movie_t
-00001280: 6974 6c65 7d3f 220a 290a 6c79 7269 6373  itle}?".).lyrics
-00001290: 5f74 656d 706c 6174 6520 3d20 5072 6f6d  _template = Prom
-000012a0: 7074 5465 6d70 6c61 7465 280a 2020 2020  ptTemplate(.    
-000012b0: 2257 7269 7465 206c 7972 6963 7320 6f66  "Write lyrics of
-000012c0: 2061 206d 6f76 6965 2073 6f6e 6720 6361   a movie song ca
-000012d0: 6c6c 6564 207b 736f 6e67 5f74 6974 6c65  lled {song_title
-000012e0: 7d2e 2054 6865 206d 6169 6e20 6368 6172  }. The main char
-000012f0: 6163 7465 7273 2061 7265 2022 0a20 2020  acters are ".   
-00001300: 2022 7b6d 6169 6e5f 6368 6172 6163 7465   "{main_characte
-00001310: 7273 7d22 0a29 0a0a 2320 4372 6561 7465  rs}".)..# Create
-00001320: 2066 6c6f 7773 7465 7073 0a6d 6f76 6965   flowsteps.movie
-00001330: 5f74 6974 6c65 5f66 6c6f 7773 7465 7020  _title_flowstep 
-00001340: 3d20 466c 6f77 5374 6570 280a 2020 2020  = FlowStep(.    
-00001350: 6e61 6d65 3d22 4d6f 7669 6520 5469 746c  name="Movie Titl
-00001360: 6520 466c 6f77 7374 6570 222c 0a20 2020  e Flowstep",.   
-00001370: 206c 6c6d 3d6f 7065 6e61 695f 6c6c 6d2c   llm=openai_llm,
-00001380: 0a20 2020 2070 726f 6d70 745f 7465 6d70  .    prompt_temp
-00001390: 6c61 7465 3d74 6974 6c65 5f74 656d 706c  late=title_templ
-000013a0: 6174 652c 0a20 2020 206f 7574 7075 745f  ate,.    output_
-000013b0: 6b65 793d 226d 6f76 6965 5f74 6974 6c65  key="movie_title
-000013c0: 222c 0a29 0a0a 736f 6e67 5f74 6974 6c65  ",.)..song_title
-000013d0: 5f66 6c6f 7773 7465 7020 3d20 466c 6f77  _flowstep = Flow
-000013e0: 5374 6570 280a 2020 2020 6e61 6d65 3d22  Step(.    name="
-000013f0: 536f 6e67 2054 6974 6c65 2046 6c6f 7773  Song Title Flows
-00001400: 7465 7022 2c0a 2020 2020 6c6c 6d3d 6f70  tep",.    llm=op
-00001410: 656e 6169 5f6c 6c6d 2c0a 2020 2020 7072  enai_llm,.    pr
-00001420: 6f6d 7074 5f74 656d 706c 6174 653d 736f  ompt_template=so
-00001430: 6e67 5f74 656d 706c 6174 652c 0a20 2020  ng_template,.   
-00001440: 206f 7574 7075 745f 6b65 793d 2273 6f6e   output_key="son
-00001450: 675f 7469 746c 6522 2c0a 290a 0a63 6861  g_title",.)..cha
-00001460: 7261 6374 6572 735f 666c 6f77 7374 6570  racters_flowstep
-00001470: 203d 2046 6c6f 7753 7465 7028 0a20 2020   = FlowStep(.   
-00001480: 206e 616d 653d 2243 6861 7261 6374 6572   name="Character
-00001490: 7320 466c 6f77 7374 6570 222c 0a20 2020  s Flowstep",.   
-000014a0: 206c 6c6d 3d6f 7065 6e61 695f 6c6c 6d2c   llm=openai_llm,
-000014b0: 0a20 2020 2070 726f 6d70 745f 7465 6d70  .    prompt_temp
-000014c0: 6c61 7465 3d63 6861 7261 6374 6572 735f  late=characters_
-000014d0: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
-000014e0: 7470 7574 5f6b 6579 3d22 6d61 696e 5f63  tput_key="main_c
-000014f0: 6861 7261 6374 6572 7322 2c0a 290a 0a73  haracters",.)..s
-00001500: 6f6e 675f 6c79 7269 6373 5f66 6c6f 7773  ong_lyrics_flows
-00001510: 7465 7020 3d20 466c 6f77 5374 6570 280a  tep = FlowStep(.
-00001520: 2020 2020 6e61 6d65 3d22 536f 6e67 204c      name="Song L
-00001530: 7972 6963 7320 466c 6f77 7374 6570 222c  yrics Flowstep",
-00001540: 0a20 2020 206c 6c6d 3d6f 7065 6e61 695f  .    llm=openai_
-00001550: 6c6c 6d2c 0a20 2020 2070 726f 6d70 745f  llm,.    prompt_
-00001560: 7465 6d70 6c61 7465 3d6c 7972 6963 735f  template=lyrics_
-00001570: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
-00001580: 7470 7574 5f6b 6579 3d22 736f 6e67 5f6c  tput_key="song_l
-00001590: 7972 6963 7322 2c0a 290a 0a23 2043 6f6e  yrics",.)..# Con
-000015a0: 6e65 6374 2066 6c6f 7773 7465 7073 0a6d  nect flowsteps.m
-000015b0: 6f76 6965 5f74 6974 6c65 5f66 6c6f 7773  ovie_title_flows
-000015c0: 7465 702e 636f 6e6e 6563 7428 736f 6e67  tep.connect(song
-000015d0: 5f74 6974 6c65 5f66 6c6f 7773 7465 702c  _title_flowstep,
-000015e0: 2063 6861 7261 6374 6572 735f 666c 6f77   characters_flow
-000015f0: 7374 6570 2c20 736f 6e67 5f6c 7972 6963  step, song_lyric
-00001600: 735f 666c 6f77 7374 6570 290a 736f 6e67  s_flowstep).song
-00001610: 5f74 6974 6c65 5f66 6c6f 7773 7465 702e  _title_flowstep.
-00001620: 636f 6e6e 6563 7428 736f 6e67 5f6c 7972  connect(song_lyr
-00001630: 6963 735f 666c 6f77 7374 6570 290a 6368  ics_flowstep).ch
-00001640: 6172 6163 7465 7273 5f66 6c6f 7773 7465  aracters_flowste
-00001650: 702e 636f 6e6e 6563 7428 736f 6e67 5f6c  p.connect(song_l
-00001660: 7972 6963 735f 666c 6f77 7374 6570 290a  yrics_flowstep).
-00001670: 0a23 2043 7265 6174 6520 616e 6420 7275  .# Create and ru
-00001680: 6e20 466c 6f77 0a73 6f75 6e64 7472 6163  n Flow.soundtrac
-00001690: 6b5f 666c 6f77 203d 2046 6c6f 7728 7469  k_flow = Flow(ti
-000016a0: 746c 655f 666c 6f77 7374 6570 290a 7265  tle_flowstep).re
-000016b0: 7375 6c74 7320 3d20 736f 756e 6474 7261  sults = soundtra
-000016c0: 636b 5f66 6c6f 772e 7374 6172 7428 746f  ck_flow.start(to
-000016d0: 7069 633d 2266 7269 656e 6473 6869 7022  pic="friendship"
-000016e0: 2c20 7665 7262 6f73 653d 5472 7565 290a  , verbose=True).
-000016f0: 6060 600a 0a23 2323 2041 7379 6e63 2046  ```..### Async F
-00001700: 6c6f 7773 0a53 6f6d 6574 696d 6573 206d  lows.Sometimes m
-00001710: 756c 7469 706c 6520 666c 6f77 2073 7465  ultiple flow ste
-00001720: 7073 2063 616e 2072 756e 2069 6e20 7061  ps can run in pa
-00001730: 7261 6c6c 656c 2069 6620 616c 6c20 7468  rallel if all th
-00001740: 6569 7220 6465 7065 6e64 656e 6369 6573  eir dependencies
-00001750: 2061 7265 206d 6574 2e20 0a46 6f72 2063   are met. .For c
-00001760: 6173 6573 206c 696b 6520 7468 6973 2c20  ases like this, 
-00001770: 4c4c 4d46 6c6f 7773 2070 726f 7669 6465  LLMFlows provide
-00001780: 7320 6173 796e 6320 636c 6173 7365 7320  s async classes 
-00001790: 746f 2069 6d70 726f 7665 2074 6865 2072  to improve the r
-000017a0: 756e 7469 6d65 206f 6620 616e 7920 0a63  untime of any .c
-000017b0: 6f6d 706c 6578 2066 6c6f 7720 6279 2072  omplex flow by r
-000017c0: 756e 6e69 6e67 2066 6c6f 7720 7374 6570  unning flow step
-000017d0: 7320 7468 6174 2061 6c72 6561 6479 2068  s that already h
-000017e0: 6176 6520 616c 6c20 7468 6569 7220 7265  ave all their re
-000017f0: 7175 6972 6564 2069 6e70 7574 7320 696e  quired inputs in
-00001800: 200a 7061 7261 6c6c 656c 2e0a 0a60 6060   .parallel...```
-00001810: 7079 7468 6f6e 0a0a 2e2e 2e0a 0a6d 6f76  python.......mov
-00001820: 6965 5f74 6974 6c65 5f66 6c6f 7773 7465  ie_title_flowste
-00001830: 7020 3d20 4173 796e 6346 6c6f 7753 7465  p = AsyncFlowSte
-00001840: 7028 0a20 2020 206e 616d 653d 2246 6c6f  p(.    name="Flo
-00001850: 7773 7465 7020 3122 2c0a 2020 2020 6c6c  wstep 1",.    ll
-00001860: 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a 2020  m=openai_llm,.  
-00001870: 2020 7072 6f6d 7074 5f74 656d 706c 6174    prompt_templat
-00001880: 653d 7469 746c 655f 7465 6d70 6c61 7465  e=title_template
-00001890: 2c0a 2020 2020 6f75 7470 7574 5f6b 6579  ,.    output_key
-000018a0: 3d22 6d6f 7669 655f 7469 746c 6522 2c0a  ="movie_title",.
-000018b0: 290a 0a73 6f6e 675f 7469 746c 655f 666c  )..song_title_fl
-000018c0: 6f77 7374 6570 203d 2046 6c6f 7753 7465  owstep = FlowSte
-000018d0: 7028 0a20 2020 206e 616d 653d 2246 6c6f  p(.    name="Flo
-000018e0: 7773 7465 7020 3222 2c0a 2020 2020 6c6c  wstep 2",.    ll
-000018f0: 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a 2020  m=openai_llm,.  
-00001900: 2020 7072 6f6d 7074 5f74 656d 706c 6174    prompt_templat
-00001910: 653d 736f 6e67 5f74 656d 706c 6174 652c  e=song_template,
-00001920: 0a20 2020 206f 7574 7075 745f 6b65 793d  .    output_key=
-00001930: 2273 6f6e 675f 7469 746c 6522 2c0a 290a  "song_title",.).
-00001940: 0a63 6861 7261 6374 6572 735f 666c 6f77  .characters_flow
-00001950: 7374 6570 203d 2041 7379 6e63 466c 6f77  step = AsyncFlow
-00001960: 5374 6570 280a 2020 2020 6e61 6d65 3d22  Step(.    name="
-00001970: 466c 6f77 7374 6570 2033 222c 0a20 2020  Flowstep 3",.   
-00001980: 206c 6c6d 3d6f 7065 6e61 695f 6c6c 6d2c   llm=openai_llm,
-00001990: 0a20 2020 2070 726f 6d70 745f 7465 6d70  .    prompt_temp
-000019a0: 6c61 7465 3d63 6861 7261 6374 6572 735f  late=characters_
-000019b0: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
-000019c0: 7470 7574 5f6b 6579 3d22 6d61 696e 5f63  tput_key="main_c
-000019d0: 6861 7261 6374 6572 7322 2c0a 290a 0a73  haracters",.)..s
-000019e0: 6f6e 675f 6c79 7269 6373 5f66 6c6f 7773  ong_lyrics_flows
-000019f0: 7465 7020 3d20 4173 796e 6346 6c6f 7753  tep = AsyncFlowS
-00001a00: 7465 7028 0a20 2020 206e 616d 653d 2246  tep(.    name="F
-00001a10: 6c6f 7773 7465 7020 3422 2c0a 2020 2020  lowstep 4",.    
-00001a20: 6c6c 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a  llm=openai_llm,.
-00001a30: 2020 2020 7072 6f6d 7074 5f74 656d 706c      prompt_templ
-00001a40: 6174 653d 6c79 7269 6373 5f74 656d 706c  ate=lyrics_templ
-00001a50: 6174 652c 0a20 2020 206f 7574 7075 745f  ate,.    output_
-00001a60: 6b65 793d 2273 6f6e 675f 6c79 7269 6373  key="song_lyrics
-00001a70: 222c 0a29 0a0a 2e2e 2e0a 0a60 6060 0a0a  ",.).......```..
-00001a80: 4368 6563 6b20 6f75 7220 646f 6375 6d65  Check our docume
-00001a90: 6e74 6174 696f 6e20 666f 7220 6d6f 7265  ntation for more
-00001aa0: 2065 7861 6d70 6c65 732c 2073 7563 6820   examples, such 
-00001ab0: 6173 2069 6e74 6567 7261 7469 6e67 2076  as integrating v
-00001ac0: 6563 746f 7220 6461 7461 6261 7365 732c  ector databases,
-00001ad0: 200a 6372 6561 7469 6e67 2071 7565 7374   .creating quest
-00001ae0: 696f 6e2d 616e 7377 6572 696e 6720 6170  ion-answering ap
-00001af0: 7073 2061 6e64 2077 6562 2061 7070 6c69  ps and web appli
-00001b00: 6361 7469 6f6e 7320 7769 7468 2046 6c61  cations with Fla
-00001b10: 736b 2061 6e64 2046 6173 7441 5049 2e0a  sk and FastAPI..
-00001b20: 0a23 2320 4665 6174 7572 6573 0a0a 2323  .## Features..##
-00001b30: 2320 2a2a 4c4c 4d73 2a2a 0a2d 2055 7469  # **LLMs**.- Uti
-00001b40: 6c69 7a65 204c 4c4d 7320 7375 6368 2061  lize LLMs such a
-00001b50: 7320 4f70 656e 4149 2773 2043 6861 7447  s OpenAI's ChatG
-00001b60: 5054 2074 6f20 6765 6e65 7261 7465 206e  PT to generate n
-00001b70: 6174 7572 616c 206c 616e 6775 6167 6520  atural language 
-00001b80: 7465 7874 2e0a 2d20 436f 6e66 6967 7572  text..- Configur
-00001b90: 6520 4c4c 4d20 636c 6173 7365 7320 6561  e LLM classes ea
-00001ba0: 7369 6c79 2c20 6368 6f6f 7369 6e67 2073  sily, choosing s
-00001bb0: 7065 6369 6669 6320 6d6f 6465 6c73 2c20  pecific models, 
-00001bc0: 7061 7261 6d65 7465 7273 2c20 616e 6420  parameters, and 
-00001bd0: 7365 7474 696e 6773 2e0a 2d20 4265 6e65  settings..- Bene
-00001be0: 6669 7420 6672 6f6d 2061 7574 6f6d 6174  fit from automat
-00001bf0: 6963 2072 6574 7269 6573 2077 6865 6e20  ic retries when 
-00001c00: 6d6f 6465 6c20 6361 6c6c 7320 6661 696c  model calls fail
-00001c10: 2c20 656e 7375 7269 6e67 2072 656c 6961  , ensuring relia
-00001c20: 626c 6520 4c4c 4d20 0a20 2069 6e74 6572  ble LLM .  inter
-00001c30: 6163 7469 6f6e 732e 0a0a 2323 2320 2a2a  actions...### **
-00001c40: 5072 6f6d 7074 2054 656d 706c 6174 6573  Prompt Templates
-00001c50: 2a2a 0a2d 2043 7265 6174 6520 6479 6e61  **.- Create dyna
-00001c60: 6d69 6320 7072 6f6d 7074 7320 7573 696e  mic prompts usin
-00001c70: 6720 5072 6f6d 7074 2054 656d 706c 6174  g Prompt Templat
-00001c80: 6573 2c20 7072 6f76 6964 696e 6720 666c  es, providing fl
-00001c90: 6578 6962 6c65 2061 6e64 2063 7573 746f  exible and custo
-00001ca0: 6d69 7a61 626c 6520 0a20 2074 6578 7420  mizable .  text 
-00001cb0: 6765 6e65 7261 7469 6f6e 2e0a 2d20 4465  generation..- De
-00001cc0: 6669 6e65 2076 6172 6961 626c 6573 2077  fine variables w
-00001cd0: 6974 6869 6e20 7072 6f6d 7074 7320 746f  ithin prompts to
-00001ce0: 2067 656e 6572 6174 6520 7072 6f6d 7074   generate prompt
-00001cf0: 2073 7472 696e 6773 2074 6169 6c6f 7265   strings tailore
-00001d00: 6420 746f 2073 7065 6369 6669 6320 0a20  d to specific . 
-00001d10: 2069 6e70 7574 732e 0a0a 2323 2320 2a2a   inputs...### **
-00001d20: 466c 6f77 7320 616e 6420 466c 6f77 5374  Flows and FlowSt
-00001d30: 6570 732a 2a0a 2d20 5374 7275 6374 7572  eps**.- Structur
-00001d40: 6520 4c4c 4d20 6170 706c 6963 6174 696f  e LLM applicatio
-00001d50: 6e73 2075 7369 6e67 2046 6c6f 7773 2061  ns using Flows a
-00001d60: 6e64 2046 6c6f 7753 7465 7073 2c20 7072  nd FlowSteps, pr
-00001d70: 6f76 6964 696e 6720 6120 636c 6561 7220  oviding a clear 
-00001d80: 616e 6420 6f72 6761 6e69 7a65 6420 6672  and organized fr
-00001d90: 616d 6577 6f72 6b20 666f 7220 6578 6563  amework for exec
-00001da0: 7574 696e 6720 4c4c 4d20 696e 7465 7261  uting LLM intera
-00001db0: 6374 696f 6e73 2e0a 2d20 436f 6e6e 6563  ctions..- Connec
-00001dc0: 7420 666c 6f77 2073 7465 7073 2074 6f20  t flow steps to 
-00001dd0: 7061 7373 206f 7574 7075 7473 2061 7320  pass outputs as 
-00001de0: 696e 7075 7473 2c20 6661 6369 6c69 7461  inputs, facilita
-00001df0: 7469 6e67 2073 6561 6d6c 6573 7320 6461  ting seamless da
-00001e00: 7461 2066 6c6f 7720 616e 640a 2020 2020  ta flow and.    
-00001e10: 6d61 696e 7461 696e 696e 6720 6120 7472  maintaining a tr
-00001e20: 616e 7370 6172 656e 7420 4c4c 4d20 7069  ansparent LLM pi
-00001e30: 7065 6c69 6e65 2e0a 2d20 4c65 7665 7261  peline..- Levera
-00001e40: 6765 2041 7379 6e63 2046 6c6f 7773 2074  ge Async Flows t
-00001e50: 6f20 7275 6e20 4c4c 4d73 2069 6e20 7061  o run LLMs in pa
-00001e60: 7261 6c6c 656c 2077 6865 6e20 616c 6c20  rallel when all 
-00001e70: 7468 6569 7220 696e 7075 7473 2061 7265  their inputs are
-00001e80: 2061 7661 696c 6162 6c65 2c20 0a20 206f   available, .  o
-00001e90: 7074 696d 697a 696e 6720 7065 7266 6f72  ptimizing perfor
-00001ea0: 6d61 6e63 6520 616e 6420 6566 6669 6369  mance and effici
-00001eb0: 656e 6379 2e0a 2d20 496e 636f 7270 6f72  ency..- Incorpor
-00001ec0: 6174 6520 6375 7374 6f6d 2073 7472 696e  ate custom strin
-00001ed0: 6720 6d61 6e69 7075 6c61 7469 6f6e 2066  g manipulation f
-00001ee0: 756e 6374 696f 6e73 2064 6972 6563 746c  unctions directl
-00001ef0: 7920 696e 746f 2066 6c6f 7773 2c20 616c  y into flows, al
-00001f00: 6c6f 7769 6e67 200a 2020 7370 6563 6961  lowing .  specia
-00001f10: 6c69 7a65 6420 7465 7874 2074 7261 6e73  lized text trans
-00001f20: 666f 726d 6174 696f 6e73 2077 6974 686f  formations witho
-00001f30: 7574 2072 656c 7969 6e67 2073 6f6c 656c  ut relying solel
-00001f40: 7920 6f6e 204c 4c4d 2063 616c 6c73 2e0a  y on LLM calls..
-00001f50: 0a23 2323 202a 2a56 6563 746f 7253 746f  .### **VectorSto
-00001f60: 7265 2049 6e74 6567 7261 7469 6f6e 732a  re Integrations*
-00001f70: 2a0a 2d20 496e 7465 6772 6174 6520 7769  *.- Integrate wi
-00001f80: 7468 2076 6563 746f 7220 6461 7461 6261  th vector databa
-00001f90: 7365 7320 6c69 6b65 2050 696e 6563 6f6e  ses like Pinecon
-00001fa0: 6520 7573 696e 6720 7468 6520 5665 6374  e using the Vect
-00001fb0: 6f72 5374 6f72 6546 6c6f 7753 7465 702c  orStoreFlowStep,
-00001fc0: 200a 2020 656d 706f 7765 7269 6e67 2065   .  empowering e
-00001fd0: 6666 6963 6965 6e74 2061 6e64 2073 6361  fficient and sca
-00001fe0: 6c61 626c 6520 7374 6f72 6167 6520 616e  lable storage an
-00001ff0: 6420 7265 7472 6965 7661 6c20 6f66 2076  d retrieval of v
-00002000: 6563 746f 7220 656d 6265 6464 696e 6773  ector embeddings
-00002010: 2e0a 2d20 4c65 7665 7261 6765 2076 6563  ..- Leverage vec
-00002020: 746f 7220 6461 7461 6261 7365 7320 666f  tor databases fo
-00002030: 7220 7365 616d 6c65 7373 2073 746f 7261  r seamless stora
-00002040: 6765 2061 6e64 2071 7565 7279 696e 6720  ge and querying 
-00002050: 6f66 2076 6563 746f 7273 2c20 656e 6162  of vectors, enab
-00002060: 6c69 6e67 2073 7472 6169 6768 7466 6f72  ling straightfor
-00002070: 7761 7264 2069 6e74 6567 7261 7469 6f6e  ward integration
-00002080: 2077 6974 6820 4c4c 4d2d 706f 7765 7265   with LLM-powere
-00002090: 6420 6170 706c 6963 6174 696f 6e73 2e0a  d applications..
-000020a0: 0a23 2323 202a 2a43 616c 6c62 6163 6b73  .### **Callbacks
-000020b0: 2a2a 0a2d 2045 7865 6375 7465 2063 616c  **.- Execute cal
-000020c0: 6c62 6163 6b20 6675 6e63 7469 6f6e 7320  lback functions 
-000020d0: 6174 2064 6966 6665 7265 6e74 2073 7461  at different sta
-000020e0: 6765 7320 7769 7468 696e 2066 6c6f 7720  ges within flow 
-000020f0: 7374 6570 732c 2065 6e61 626c 696e 6720  steps, enabling 
-00002100: 656e 6861 6e63 6564 2063 7573 746f 6d69  enhanced customi
-00002110: 7a61 7469 6f6e 2c20 6c6f 6767 696e 672c  zation, logging,
-00002120: 2074 7261 6369 6e67 2c20 6f72 206f 7468   tracing, or oth
-00002130: 6572 2073 7065 6369 6669 6320 696e 7465  er specific inte
-00002140: 6772 6174 696f 6e73 2e0a 2d20 5574 696c  grations..- Util
-00002150: 697a 6520 6361 6c6c 6261 636b 7320 746f  ize callbacks to
-00002160: 2063 6f6d 7072 6568 656e 7369 7665 6c79   comprehensively
-00002170: 2063 6f6e 7472 6f6c 2061 6e64 206d 6f6e   control and mon
-00002180: 6974 6f72 204c 4c4d 2d70 6f77 6572 6564  itor LLM-powered
-00002190: 2061 7070 732c 2065 6e73 7572 696e 6720   apps, ensuring 
-000021a0: 0a20 2063 6c65 6172 2076 6973 6962 696c  .  clear visibil
-000021b0: 6974 7920 696e 746f 2074 6865 2065 7865  ity into the exe
-000021c0: 6375 7469 6f6e 2070 726f 6365 7373 2e0a  cution process..
-000021d0: 0a23 2323 202a 2a45 7870 6c69 6369 7420  .### **Explicit 
-000021e0: 4150 4920 616e 6420 4675 6c6c 2054 7261  API and Full Tra
-000021f0: 6e73 7061 7265 6e63 792a 2a0a 5769 7468  nsparency**.With
-00002200: 204c 4c4d 466c 6f77 7320 796f 7520 6861   LLMFlows you ha
-00002210: 7665 2074 6865 2066 756c 6c20 636f 6e74  ve the full cont
-00002220: 726f 6c20 746f 2063 7265 6174 6520 6578  rol to create ex
-00002230: 706c 6963 6974 2061 7070 6c69 6361 7469  plicit applicati
-00002240: 6f6e 7320 7769 7468 6f75 7420 616e 7920  ons without any 
-00002250: 6869 6464 656e 2070 726f 6d70 7473 206f  hidden prompts o
-00002260: 7220 7072 6564 6566 696e 6564 2062 6568  r predefined beh
-00002270: 6176 696f 7273 2e0a 0a49 6e20 6164 6469  aviors...In addi
-00002280: 7469 6f6e 204c 4c4d 466c 6f77 7320 616c  tion LLMFlows al
-00002290: 6c6f 7773 2079 6f75 2074 6f20 616e 7377  lows you to answ
-000022a0: 6572 2071 7565 7374 696f 6e73 2073 7563  er questions suc
-000022b0: 6820 6173 3a0a 0a2d 2057 6865 6e20 7761  h as:..- When wa
-000022c0: 7320 6120 7061 7274 6963 756c 6172 2066  s a particular f
-000022d0: 6c6f 7773 7465 7020 7275 6e3f 0a2d 2048  lowstep run?.- H
-000022e0: 6f77 206d 7563 6820 7469 6d65 2064 6964  ow much time did
-000022f0: 2069 7420 7461 6b65 3f0a 2d20 5768 6174   it take?.- What
-00002300: 2077 6572 6520 7468 6520 696e 7075 7420   were the input 
-00002310: 7661 7269 6162 6c65 733f 0a2d 2057 6861  variables?.- Wha
-00002320: 7420 7761 7320 7468 6520 7072 6f6d 7074  t was the prompt
-00002330: 2074 656d 706c 6174 653f 0a2d 2057 6861   template?.- Wha
-00002340: 7420 6469 6420 7468 6520 7072 6f6d 7074  t did the prompt
-00002350: 206c 6f6f 6b20 6c69 6b65 3f0a 2d20 5768   look like?.- Wh
-00002360: 6174 2077 6173 2074 6865 2065 7861 6374  at was the exact
-00002370: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
-00002380: 6620 7468 6520 6d6f 6465 6c3f 0a2d 2048  f the model?.- H
-00002390: 6f77 206d 616e 7920 7469 6d65 7320 6469  ow many times di
-000023a0: 6420 7765 2072 6574 7279 2074 6865 2072  d we retry the r
-000023b0: 6571 7565 7374 3f0a 2d20 5768 6174 2077  equest?.- What w
-000023c0: 6173 2074 6865 2072 6177 2064 6174 6120  as the raw data 
-000023d0: 7468 6520 4150 4920 7265 7475 726e 6564  the API returned
-000023e0: 3f0a 2d20 486f 7720 6d61 6e79 2074 6f6b  ?.- How many tok
-000023f0: 656e 7320 7765 7265 2075 7365 643f 0a2d  ens were used?.-
-00002400: 2057 6861 7420 7761 7320 7468 6520 6669   What was the fi
-00002410: 6e61 6c20 7265 7375 6c74 3f0a 0a23 2320  nal result?..## 
-00002420: 4c69 6365 6e73 650a 4c4c 4d46 6c6f 7773  License.LLMFlows
-00002430: 2069 7320 636f 7665 7265 6420 6279 2074   is covered by t
-00002440: 6865 204d 4954 206c 6963 656e 7365 2e20  he MIT license. 
-00002450: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
-00002460: 7469 6f6e 2c20 6368 6563 6b20 604c 4943  tion, check `LIC
-00002470: 454e 4345 2e6d 6460 2e0a 0a23 2320 436f  ENCE.md`...## Co
-00002480: 6e74 7269 6275 7469 6e67 0a54 6861 6e6b  ntributing.Thank
-00002490: 2079 6f75 2066 6f72 2073 7065 6e64 696e   you for spendin
-000024a0: 6720 7469 6d65 2067 6f69 6e67 206f 7665  g time going ove
-000024b0: 7220 6f75 7220 5245 4144 4d45 2120 4966  r our README! If
-000024c0: 2079 6f75 2066 696e 6420 4c4c 4d46 6c6f   you find LLMFlo
-000024d0: 7773 2065 7863 6974 696e 6720 616e 6420  ws exciting and 
-000024e0: 0a79 6f75 2061 7265 2063 6f6e 7369 6465  .you are conside
-000024f0: 7269 6e67 2063 6f6e 7472 6962 7574 696e  ring contributin
-00002500: 672c 2070 6c65 6173 6520 6368 6563 6b20  g, please check 
-00002510: 5b60 434f 4e54 5249 4255 5449 4e47 2e6d  [`CONTRIBUTING.m
-00002520: 6460 5d28 6874 7470 733a 2f2f 6769 7468  d`](https://gith
-00002530: 7562 2e63 6f6d 2f73 746f 7961 6e2d 7374  ub.com/stoyan-st
-00002540: 6f79 616e 6f76 2f6c 6c6d 666c 6f77 732f  oyanov/llmflows/
-00002550: 626c 6f62 2f6d 6169 6e2f 434f 4e54 5249  blob/main/CONTRI
-00002560: 4255 5449 4e47 2e6d 6429 2e0a            BUTING.md)..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6c6c 6d66  : 2.1.Name: llmf
+00000020: 6c6f 7773 0a56 6572 7369 6f6e 3a20 302e  lows.Version: 0.
+00000030: 302e 390a 5375 6d6d 6172 793a 204c 4c4d  0.9.Summary: LLM
+00000040: 466c 6f77 7320 2d20 5369 6d70 6c65 2c20  Flows - Simple, 
+00000050: 4578 706c 6963 6974 2061 6e64 2054 7261  Explicit and Tra
+00000060: 6e73 7061 7265 6e74 204c 4c4d 2041 7070  nsparent LLM App
+00000070: 730a 4175 7468 6f72 3a20 5374 6f79 616e  s.Author: Stoyan
+00000080: 2053 746f 7961 6e6f 760a 5072 6f6a 6563   Stoyanov.Projec
+00000090: 742d 5552 4c3a 2048 6f6d 6570 6167 652c  t-URL: Homepage,
+000000a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000b0: 636f 6d2f 7374 6f79 616e 2d73 746f 7961  com/stoyan-stoya
+000000c0: 6e6f 762f 6c6c 6d66 6c6f 7773 0a50 726f  nov/llmflows.Pro
+000000d0: 6a65 6374 2d55 524c 3a20 6769 7468 7562  ject-URL: github
+000000e0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+000000f0: 2e63 6f6d 2f73 746f 7961 6e2d 7374 6f79  .com/stoyan-stoy
+00000100: 616e 6f76 2f6c 6c6d 666c 6f77 730a 436c  anov/llmflows.Cl
+00000110: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000120: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000130: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+00000140: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000150: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000160: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000170: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000180: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000190: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+000001a0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+000001b0: 203e 3d33 2e39 0a44 6573 6372 6970 7469   >=3.9.Descripti
+000001c0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+000001d0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
+000001e0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+000001f0: 454e 5345 0a0a 2320 4c4c 4d46 6c6f 7773  ENSE..# LLMFlows
+00000200: 202d 2053 696d 706c 652c 2045 7870 6c69   - Simple, Expli
+00000210: 6369 742c 2061 6e64 2054 7261 6e73 7061  cit, and Transpa
+00000220: 7265 6e74 204c 4c4d 2041 7070 730a 3c62  rent LLM Apps.<b
+00000230: 722f 3e0a 3c62 722f 3e0a 3c62 722f 3e0a  r/>.<br/>.<br/>.
+00000240: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000250: 223e 0a20 203c 696d 6720 7374 796c 653d  ">.  <img style=
+00000260: 2277 6964 7468 3a20 3830 2522 2073 7263  "width: 80%" src
+00000270: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000280: 2e63 6f6d 2f73 746f 7961 6e2d 7374 6f79  .com/stoyan-stoy
+00000290: 616e 6f76 2f6c 6c6d 666c 6f77 732f 626c  anov/llmflows/bl
+000002a0: 6f62 2f6d 6169 6e2f 646f 6373 2f6c 6c6d  ob/main/docs/llm
+000002b0: 666c 6f77 735f 6c61 7374 5f6c 6f67 6f2e  flows_last_logo.
+000002c0: 706e 6722 2f3e 0a3c 2f70 3e0a 3c62 722f  png"/>.</p>.<br/
+000002d0: 3e0a 3c62 722f 3e0a 3c62 722f 3e0a 0a5b  >.<br/>.<br/>..[
+000002e0: 215b 5477 6974 7465 725d 2868 7474 7073  ![Twitter](https
+000002f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000300: 6f2f 7477 6974 7465 722f 666f 6c6c 6f77  o/twitter/follow
+00000310: 2f4c 4c4d 466c 6f77 733f 7374 796c 653d  /LLMFlows?style=
+00000320: 736f 6369 616c 295d 2868 7474 7073 3a2f  social)](https:/
+00000330: 2f74 7769 7474 6572 2e63 6f6d 2f4c 4c4d  /twitter.com/LLM
+00000340: 466c 6f77 7329 0a21 5b50 796c 696e 7420  Flows).![Pylint 
+00000350: 776f 726b 666c 6f77 5d28 6874 7470 733a  workflow](https:
+00000360: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746f  //github.com/sto
+00000370: 7961 6e2d 7374 6f79 616e 6f76 2f6c 6c6d  yan-stoyanov/llm
+00000380: 666c 6f77 732f 6163 7469 6f6e 732f 776f  flows/actions/wo
+00000390: 726b 666c 6f77 732f 7079 6c69 6e74 2e79  rkflows/pylint.y
+000003a0: 6d6c 2f62 6164 6765 2e73 7667 290a 215b  ml/badge.svg).![
+000003b0: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+000003c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000003d0: 6769 7468 7562 2f6c 6963 656e 7365 2f73  github/license/s
+000003e0: 746f 7961 6e2d 7374 6f79 616e 6f76 2f6c  toyan-stoyanov/l
+000003f0: 6c6d 666c 6f77 7329 0a21 5b50 7950 695d  lmflows).![PyPi]
+00000400: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000410: 656c 6473 2e69 6f2f 7079 7069 2f76 2f6c  elds.io/pypi/v/l
+00000420: 6c6d 666c 6f77 7329 0a21 5b53 7461 7273  lmflows).![Stars
+00000430: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000440: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000450: 7374 6172 732f 7374 6f79 616e 2d73 746f  stars/stoyan-sto
+00000460: 7961 6e6f 762f 6c6c 6d66 6c6f 7773 3f73  yanov/llmflows?s
+00000470: 7479 6c65 3d73 6f63 6961 6c29 0a21 5b52  tyle=social).![R
+00000480: 656c 6561 7365 2064 6174 655d 2868 7474  elease date](htt
+00000490: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000004a0: 2e69 6f2f 6769 7468 7562 2f72 656c 6561  .io/github/relea
+000004b0: 7365 2d64 6174 652f 7374 6f79 616e 2d73  se-date/stoyan-s
+000004c0: 746f 7961 6e6f 762f 6c6c 6d66 6c6f 7773  toyanov/llmflows
+000004d0: 3f73 7479 6c65 3d73 6f63 6961 6c29 0a0a  ?style=social)..
+000004e0: 446f 6375 6d65 6e74 6174 696f 6e3a 203c  Documentation: <
+000004f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000500: 6c6c 6d66 6c6f 7773 2e72 6561 6474 6865  llmflows.readthe
+00000510: 646f 6373 2e69 6f2f 2220 7461 7267 6574  docs.io/" target
+00000520: 3d22 5f62 6c61 6e6b 223e 6874 7470 733a  ="_blank">https:
+00000530: 2f2f 6c6c 6d66 6c6f 7773 2e72 6561 6474  //llmflows.readt
+00000540: 6865 646f 6373 2e69 6f3c 2f61 3e3c 2f62  hedocs.io</a></b
+00000550: 723e 0a50 7950 493a 203c 6120 6872 6566  r>.PyPI: <a href
+00000560: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000570: 7267 2f70 726f 6a65 6374 2f6c 6c6d 666c  rg/project/llmfl
+00000580: 6f77 732f 2220 7461 7267 6574 3d22 5f62  ows/" target="_b
+00000590: 6c61 6e6b 223e 6874 7470 733a 2f2f 7079  lank">https://py
+000005a0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
+000005b0: 6c6d 666c 6f77 733c 2f61 3e3c 2f62 723e  lmflows</a></br>
+000005c0: 0a54 7769 7474 6572 3a20 3c61 2068 7265  .Twitter: <a hre
+000005d0: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
+000005e0: 6572 2e63 6f6d 2f4c 4c4d 466c 6f77 732f  er.com/LLMFlows/
+000005f0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000600: 223e 6874 7470 733a 2f2f 7477 6974 7465  ">https://twitte
+00000610: 722e 636f 6d2f 4c4c 4d46 6c6f 7773 3c2f  r.com/LLMFlows</
+00000620: 613e 3c2f 6272 3e0a 5375 6273 7461 636b  a></br>.Substack
+00000630: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
+00000640: 3a2f 2f6c 6c6d 666c 6f77 732e 7375 6273  ://llmflows.subs
+00000650: 7461 636b 2e63 6f6d 2f22 2074 6172 6765  tack.com/" targe
+00000660: 743d 225f 626c 616e 6b22 3e68 7474 7073  t="_blank">https
+00000670: 3a2f 2f6c 6c6d 666c 6f77 732e 7375 6273  ://llmflows.subs
+00000680: 7461 636b 2e63 6f6d 3c2f 613e 3c2f 6272  tack.com</a></br
+00000690: 3e0a 0a23 2320 4162 6f75 740a 4c4c 4d46  >..## About.LLMF
+000006a0: 6c6f 7773 2069 7320 6120 6672 616d 6577  lows is a framew
+000006b0: 6f72 6b20 666f 7220 6275 696c 6469 6e67  ork for building
+000006c0: 2073 696d 706c 652c 2065 7870 6c69 6369   simple, explici
+000006d0: 742c 2061 6e64 2074 7261 6e73 7061 7265  t, and transpare
+000006e0: 6e74 204c 4c4d 284c 6172 6765 200a 4c61  nt LLM(Large .La
+000006f0: 6e67 7561 6765 204d 6f64 656c 2920 6170  nguage Model) ap
+00000700: 706c 6963 6174 696f 6e73 2e0a 0a23 2320  plications...## 
+00000710: 496e 7374 616c 6c61 7469 6f6e 0a60 6060  Installation.```
+00000720: 0a70 6970 2069 6e73 7461 6c6c 206c 6c6d  .pip install llm
+00000730: 666c 6f77 730a 6060 600a 0a23 2320 5068  flows.```..## Ph
+00000740: 696c 6f73 6f70 6879 0a0a 2323 2320 2a2a  ilosophy..### **
+00000750: 5369 6d70 6c65 2a2a 0a4f 7572 2067 6f61  Simple**.Our goa
+00000760: 6c20 6973 2074 6f20 6275 696c 6420 6120  l is to build a 
+00000770: 7369 6d70 6c65 2c20 7765 6c6c 2d64 6f63  simple, well-doc
+00000780: 756d 656e 7465 6420 6672 616d 6577 6f72  umented framewor
+00000790: 6b20 7769 7468 206d 696e 696d 616c 2061  k with minimal a
+000007a0: 6273 7472 6163 7469 6f6e 7320 7468 6174  bstractions that
+000007b0: 200a 616c 6c6f 7720 7573 6572 7320 746f   .allow users to
+000007c0: 2062 7569 6c64 2066 6c65 7869 626c 6520   build flexible 
+000007d0: 4c4c 4d2d 706f 7765 7265 6420 6170 7073  LLM-powered apps
+000007e0: 2077 6974 686f 7574 2063 6f6d 7072 6f6d   without comprom
+000007f0: 6973 696e 6720 6f6e 2063 6170 6162 696c  ising on capabil
+00000800: 6974 6965 732e 0a0a 2323 2320 2a2a 4578  ities...### **Ex
+00000810: 706c 6963 6974 2a2a 0a57 6520 7761 6e74  plicit**.We want
+00000820: 2074 6f20 6372 6561 7465 2061 6e20 6578   to create an ex
+00000830: 706c 6963 6974 2041 5049 2065 6e61 626c  plicit API enabl
+00000840: 696e 6720 7573 6572 7320 746f 2077 7269  ing users to wri
+00000850: 7465 2063 6c65 616e 2061 6e64 2072 6561  te clean and rea
+00000860: 6461 626c 6520 636f 6465 2077 6869 6c65  dable code while
+00000870: 200a 6561 7369 6c79 2063 7265 6174 696e   .easily creatin
+00000880: 6720 636f 6d70 6c65 7820 666c 6f77 7320  g complex flows 
+00000890: 6f66 204c 4c4d 7320 696e 7465 7261 6374  of LLMs interact
+000008a0: 696e 6720 7769 7468 2065 6163 6820 6f74  ing with each ot
+000008b0: 6865 722e 204c 4c4d 466c 6f77 7327 2063  her. LLMFlows' c
+000008c0: 6c61 7373 6573 200a 6769 7665 2075 7365  lasses .give use
+000008d0: 7273 2066 756c 6c20 636f 6e74 726f 6c20  rs full control 
+000008e0: 616e 6420 646f 206e 6f74 2068 6176 6520  and do not have 
+000008f0: 616e 7920 6869 6464 656e 2070 726f 6d70  any hidden promp
+00000900: 7473 206f 7220 4c4c 4d20 6361 6c6c 732e  ts or LLM calls.
+00000910: 200a 0a23 2323 202a 2a54 7261 6e73 7061   ..### **Transpa
+00000920: 7265 6e74 2a2a 0a57 6520 6169 6d20 746f  rent**.We aim to
+00000930: 2068 656c 7020 7573 6572 7320 6861 7665   help users have
+00000940: 2066 756c 6c20 7472 616e 7370 6172 656e   full transparen
+00000950: 6379 206f 6e20 7468 6569 7220 4c4c 4d2d  cy on their LLM-
+00000960: 706f 7765 7265 6420 6170 7073 2062 7920  powered apps by 
+00000970: 7072 6f76 6964 696e 6720 0a74 7261 6365  providing .trace
+00000980: 6162 6c65 2066 6c6f 7773 2061 6e64 2063  able flows and c
+00000990: 6f6d 706c 6574 6520 696e 666f 726d 6174  omplete informat
+000009a0: 696f 6e20 666f 7220 6561 6368 2061 7070  ion for each app
+000009b0: 2063 6f6d 706f 6e65 6e74 2c20 6d61 6b69   component, maki
+000009c0: 6e67 2069 7420 6561 7379 2074 6f20 0a6d  ng it easy to .m
+000009d0: 6f6e 6974 6f72 2c20 6d61 696e 7461 696e  onitor, maintain
+000009e0: 2c20 616e 6420 6465 6275 672e 0a0a 2323  , and debug...##
+000009f0: 2047 6574 7469 6e67 2053 7461 7274 6564   Getting Started
+00000a00: 0a23 2323 204c 4c4d 730a 4c4c 4d73 2061  .### LLMs.LLMs a
+00000a10: 7265 206f 6e65 206f 6620 7468 6520 6d61  re one of the ma
+00000a20: 696e 2061 6273 7472 6163 7469 6f6e 7320  in abstractions 
+00000a30: 696e 204c 4c4d 466c 6f77 732e 204c 4c4d  in LLMFlows. LLM
+00000a40: 2063 6c61 7373 6573 2061 7265 2077 7261   classes are wra
+00000a50: 7070 6572 7320 6172 6f75 6e64 204c 4c4d  ppers around LLM
+00000a60: 200a 4150 4973 2073 7563 6820 6173 204f   .APIs such as O
+00000a70: 7065 6e41 4927 7320 4150 4973 2e20 5468  penAI's APIs. Th
+00000a80: 6579 2070 726f 7669 6465 206d 6574 686f  ey provide metho
+00000a90: 6473 2066 6f72 2063 6f6e 6669 6775 7269  ds for configuri
+00000aa0: 6e67 2061 6e64 2063 616c 6c69 6e67 2074  ng and calling t
+00000ab0: 6865 7365 2041 5049 732c 200a 7265 7472  hese APIs, .retr
+00000ac0: 7969 6e67 2066 6169 6c65 6420 6361 6c6c  ying failed call
+00000ad0: 732c 2061 6e64 2066 6f72 6d61 7474 696e  s, and formattin
+00000ae0: 6720 7468 6520 7265 7370 6f6e 7365 732e  g the responses.
+00000af0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000b00: 206c 6c6d 666c 6f77 732e 6c6c 6d73 2069   llmflows.llms i
+00000b10: 6d70 6f72 7420 4f70 656e 4149 0a0a 6c6c  mport OpenAI..ll
+00000b20: 6d20 3d20 4f70 656e 4149 2861 7069 5f6b  m = OpenAI(api_k
+00000b30: 6579 3d22 3c79 6f75 722d 6f70 656e 6169  ey="<your-openai
+00000b40: 2d61 7069 2d6b 6579 3e22 290a 0a72 6573  -api-key>")..res
+00000b50: 756c 742c 2063 616c 6c5f 6461 7461 2c20  ult, call_data, 
+00000b60: 6d6f 6465 6c5f 636f 6e66 6967 203d 206c  model_config = l
+00000b70: 6c6d 2e67 656e 6572 6174 6528 0a20 2020  lm.generate(.   
+00000b80: 7072 6f6d 7074 3d22 4765 6e65 7261 7465  prompt="Generate
+00000b90: 2061 2063 6f6f 6c20 7469 746c 6520 666f   a cool title fo
+00000ba0: 7220 616e 2038 3073 2072 6f63 6b20 736f  r an 80s rock so
+00000bb0: 6e67 220a 290a 6060 600a 0a0a 2323 2320  ng".).```...### 
+00000bc0: 5072 6f6d 7074 5465 6d70 6c61 7465 730a  PromptTemplates.
+00000bd0: 5468 6520 6050 726f 6d70 7454 656d 706c  The `PromptTempl
+00000be0: 6174 6560 2063 6c61 7373 2061 6c6c 6f77  ate` class allow
+00000bf0: 7320 7573 2074 6f20 6372 6561 7465 2073  s us to create s
+00000c00: 7472 696e 6773 2077 6974 6820 7661 7269  trings with vari
+00000c10: 6162 6c65 7320 7468 6174 2077 6520 6361  ables that we ca
+00000c20: 6e20 6669 6c6c 200a 696e 2064 796e 616d  n fill .in dynam
+00000c30: 6963 616c 6c79 206c 6174 6572 206f 6e2e  ically later on.
+00000c40: 204f 6e63 6520 6120 7072 6f6d 7074 2074   Once a prompt t
+00000c50: 656d 706c 6174 6520 6f62 6a65 6374 2069  emplate object i
+00000c60: 7320 6372 6561 7465 6420 616e 2061 6374  s created an act
+00000c70: 7561 6c20 7072 6f6d 7074 2063 616e 200a  ual prompt can .
+00000c80: 6265 2067 656e 6572 6174 6564 2062 7920  be generated by 
+00000c90: 7072 6f76 6964 696e 6720 7468 6520 7265  providing the re
+00000ca0: 7175 6972 6564 2076 6172 6961 626c 6573  quired variables
+00000cb0: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+00000cc0: 6d20 6c6c 6d66 6c6f 7773 2e6c 6c6d 7320  m llmflows.llms 
+00000cd0: 696d 706f 7274 204f 7065 6e41 490a 6672  import OpenAI.fr
+00000ce0: 6f6d 206c 6c6d 666c 6f77 732e 7072 6f6d  om llmflows.prom
+00000cf0: 7074 7320 696d 706f 7274 2050 726f 6d70  pts import Promp
+00000d00: 7454 656d 706c 6174 650a 0a0a 7072 6f6d  tTemplate...prom
+00000d10: 7074 5f74 656d 706c 6174 6520 3d20 5072  pt_template = Pr
+00000d20: 6f6d 7074 5465 6d70 6c61 7465 280a 2020  omptTemplate(.  
+00000d30: 2020 7072 6f6d 7074 3d22 4765 6e65 7261    prompt="Genera
+00000d40: 7465 2061 2074 6974 6c65 2066 6f72 2061  te a title for a
+00000d50: 2039 3073 2068 6970 2d68 6f70 2073 6f6e   90s hip-hop son
+00000d60: 6720 6162 6f75 7420 7b74 6f70 6963 7d2e  g about {topic}.
+00000d70: 220a 290a 6c6c 6d5f 7072 6f6d 7074 203d  ".).llm_prompt =
+00000d80: 2070 726f 6d70 745f 7465 6d70 6c61 7465   prompt_template
+00000d90: 2e67 6574 5f70 726f 6d70 7428 746f 7069  .get_prompt(topi
+00000da0: 633d 2266 7269 656e 6473 6869 7022 290a  c="friendship").
+00000db0: 0a70 7269 6e74 286c 6c6d 5f70 726f 6d70  .print(llm_promp
+00000dc0: 7429 0a0a 6c6c 6d20 3d20 4f70 656e 4149  t)..llm = OpenAI
+00000dd0: 2861 7069 5f6b 6579 3d22 3c79 6f75 722d  (api_key="<your-
+00000de0: 6f70 656e 6169 2d61 7069 2d6b 6579 3e22  openai-api-key>"
+00000df0: 290a 736f 6e67 5f74 6974 6c65 203d 206c  ).song_title = l
+00000e00: 6c6d 2e67 656e 6572 6174 6528 6c6c 6d5f  lm.generate(llm_
+00000e10: 7072 6f6d 7074 290a 0a70 7269 6e74 2873  prompt)..print(s
+00000e20: 6f6e 675f 7469 746c 6529 0a60 6060 0a0a  ong_title).```..
+00000e30: 2323 2320 4368 6174 204c 4c4d 730a 556e  ### Chat LLMs.Un
+00000e40: 6c69 6b65 2072 6567 756c 6172 204c 4c4d  like regular LLM
+00000e50: 7320 7468 6174 206f 6e6c 7920 7265 7175  s that only requ
+00000e60: 6972 6520 6120 7072 6f6d 7074 2074 6f20  ire a prompt to 
+00000e70: 6765 6e65 7261 7465 2074 6578 742c 2063  generate text, c
+00000e80: 6861 7420 4c4c 4d73 2072 6571 7569 7265  hat LLMs require
+00000e90: 2061 200a 636f 6e76 6572 7361 7469 6f6e   a .conversation
+00000ea0: 2068 6973 746f 7279 2e20 5468 6520 636f   history. The co
+00000eb0: 6e76 6572 7361 7469 6f6e 2068 6973 746f  nversation histo
+00000ec0: 7279 2069 7320 7265 7072 6573 656e 7465  ry is represente
+00000ed0: 6420 0a61 7320 6120 6c69 7374 206f 6620  d .as a list of 
+00000ee0: 6d65 7373 6167 6573 2062 6574 7765 656e  messages between
+00000ef0: 2061 2075 7365 7220 616e 6420 616e 2061   a user and an a
+00000f00: 7373 6973 7461 6e74 2e20 5468 6973 2063  ssistant. This c
+00000f10: 6f6e 7665 7273 6174 696f 6e20 6869 7374  onversation hist
+00000f20: 6f72 7920 6973 200a 7365 6e74 2074 6f20  ory is .sent to 
+00000f30: 7468 6520 6d6f 6465 6c2c 2061 6e64 2061  the model, and a
+00000f40: 206e 6577 206d 6573 7361 6765 2069 7320   new message is 
+00000f50: 6765 6e65 7261 7465 6420 6261 7365 6420  generated based 
+00000f60: 6f6e 2069 742e 0a0a 4c4c 4d46 6c6f 7773  on it...LLMFlows
+00000f70: 2070 726f 7669 6465 7320 6120 604d 6573   provides a `Mes
+00000f80: 7361 6765 4869 7374 6f72 7960 2063 6c61  sageHistory` cla
+00000f90: 7373 2074 6f20 6d61 6e61 6765 2074 6865  ss to manage the
+00000fa0: 2072 6571 7569 7265 6420 636f 6e76 6572   required conver
+00000fb0: 7361 7469 6f6e 2068 6973 746f 7279 200a  sation history .
+00000fc0: 666f 7220 6368 6174 204c 4c4d 732e 0a0a  for chat LLMs...
+00000fd0: 596f 7520 6361 6e20 6275 696c 6420 6120  You can build a 
+00000fe0: 7369 6d70 6c65 2063 6861 7462 6f74 2062  simple chatbot b
+00000ff0: 7920 7573 696e 6720 7468 6520 604f 7065  y using the `Ope
+00001000: 6e41 4943 6861 7460 2061 6e64 2060 4d65  nAIChat` and `Me
+00001010: 7373 6167 6548 6973 746f 7279 6020 636c  ssageHistory` cl
+00001020: 6173 7365 733a 0a0a 6060 6070 7974 686f  asses:..```pytho
+00001030: 6e0a 6672 6f6d 206c 6c6d 666c 6f77 732e  n.from llmflows.
+00001040: 6c6c 6d73 2069 6d70 6f72 7420 4f70 656e  llms import Open
+00001050: 4149 4368 6174 2c20 4d65 7373 6167 6548  AIChat, MessageH
+00001060: 6973 746f 7279 0a0a 6c6c 6d20 3d20 4f70  istory..llm = Op
+00001070: 656e 4149 4368 6174 2861 7069 5f6b 6579  enAIChat(api_key
+00001080: 3d22 3c79 6f75 722d 6f70 656e 6169 2d61  ="<your-openai-a
+00001090: 7069 2d6b 6579 3e22 290a 6d65 7373 6167  pi-key>").messag
+000010a0: 655f 6869 7374 6f72 7920 3d20 4d65 7373  e_history = Mess
+000010b0: 6167 6548 6973 746f 7279 2829 0a0a 7768  ageHistory()..wh
+000010c0: 696c 6520 5472 7565 3a0a 2020 2020 7573  ile True:.    us
+000010d0: 6572 5f6d 6573 7361 6765 203d 2069 6e70  er_message = inp
+000010e0: 7574 2822 596f 753a 2229 0a20 2020 206d  ut("You:").    m
+000010f0: 6573 7361 6765 5f68 6973 746f 7279 2e61  essage_history.a
+00001100: 6464 5f75 7365 725f 6d65 7373 6167 6528  dd_user_message(
+00001110: 7573 6572 5f6d 6573 7361 6765 290a 0a20  user_message).. 
+00001120: 2020 206c 6c6d 5f72 6573 706f 6e73 652c     llm_response,
+00001130: 2063 616c 6c5f 6461 7461 2c20 6d6f 6465   call_data, mode
+00001140: 6c5f 636f 6e66 6967 203d 206c 6c6d 2e67  l_config = llm.g
+00001150: 656e 6572 6174 6528 6d65 7373 6167 655f  enerate(message_
+00001160: 6869 7374 6f72 7929 0a20 2020 206d 6573  history).    mes
+00001170: 7361 6765 5f68 6973 746f 7279 2e61 6464  sage_history.add
+00001180: 5f61 695f 6d65 7373 6167 6528 6c6c 6d5f  _ai_message(llm_
+00001190: 7265 7370 6f6e 7365 290a 0a20 2020 2070  response)..    p
+000011a0: 7269 6e74 2866 224c 4c4d 3a20 7b6c 6c6d  rint(f"LLM: {llm
+000011b0: 5f72 6573 706f 6e73 657d 2229 0a60 6060  _response}").```
+000011c0: 0a0a 2323 2320 4c4c 4d20 466c 6f77 730a  ..### LLM Flows.
+000011d0: 4f66 7465 6e20 7469 6d65 732c 2072 6561  Often times, rea
+000011e0: 6c2d 776f 726c 6420 6170 706c 6963 6174  l-world applicat
+000011f0: 696f 6e73 2063 616e 2062 6520 6d6f 7265  ions can be more
+00001200: 2063 6f6d 706c 6578 2061 6e64 2063 616e   complex and can
+00001210: 2068 6176 6520 6465 7065 6e64 656e 6369   have dependenci
+00001220: 6573 200a 6265 7477 6565 6e20 7072 6f6d  es .between prom
+00001230: 7074 7320 616e 6420 4c4c 4d20 6361 6c6c  pts and LLM call
+00001240: 732e 2046 6f72 2065 7861 6d70 6c65 3a0a  s. For example:.
+00001250: 0a21 5b43 6f6d 706c 6578 2066 6c6f 775d  .![Complex flow]
+00001260: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001270: 636f 6d2f 7374 6f79 616e 2d73 746f 7961  com/stoyan-stoya
+00001280: 6e6f 762f 6c6c 6d66 6c6f 7773 2f62 6c6f  nov/llmflows/blo
+00001290: 622f 6d61 696e 2f64 6f63 732f 636f 6d70  b/main/docs/comp
+000012a0: 6c65 785f 666c 6f77 2e70 6e67 290a 0a57  lex_flow.png)..W
+000012b0: 6865 6e20 796f 7520 7761 6e74 2074 6f20  hen you want to 
+000012c0: 6275 696c 6420 6170 7073 2077 6974 6820  build apps with 
+000012d0: 636f 6d70 6c65 7820 6465 7065 6e64 656e  complex dependen
+000012e0: 6369 6573 2079 6f75 2063 616e 2075 7365  cies you can use
+000012f0: 2074 6865 2060 466c 6f77 6020 616e 6420   the `Flow` and 
+00001300: 0a60 466c 6f77 7374 6570 6020 636c 6173  .`Flowstep` clas
+00001310: 7365 732e 204c 4c4d 466c 6f77 7320 7769  ses. LLMFlows wi
+00001320: 6c6c 2066 6967 7572 6520 6f75 7420 7468  ll figure out th
+00001330: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
+00001340: 6e64 206d 616b 6520 7375 7265 2065 6163  nd make sure eac
+00001350: 6820 0a66 6c6f 7773 7465 7020 7275 6e73  h .flowstep runs
+00001360: 206f 6e6c 7920 7768 656e 2061 6c6c 2069   only when all i
+00001370: 7473 2064 6570 656e 6465 6e63 6965 7320  ts dependencies 
+00001380: 6172 6520 6d65 743a 0a0a 6060 6070 7974  are met:..```pyt
+00001390: 686f 6e0a 6672 6f6d 206c 6c6d 666c 6f77  hon.from llmflow
+000013a0: 732e 666c 6f77 7320 696d 706f 7274 2046  s.flows import F
+000013b0: 6c6f 772c 2046 6c6f 7753 7465 700a 6672  low, FlowStep.fr
+000013c0: 6f6d 206c 6c6d 666c 6f77 732e 6c6c 6d73  om llmflows.llms
+000013d0: 2069 6d70 6f72 7420 4f70 656e 4149 0a66   import OpenAI.f
+000013e0: 726f 6d20 6c6c 6d66 6c6f 7773 2e70 726f  rom llmflows.pro
+000013f0: 6d70 7473 2069 6d70 6f72 7420 5072 6f6d  mpts import Prom
+00001400: 7074 5465 6d70 6c61 7465 0a0a 6f70 656e  ptTemplate..open
+00001410: 6169 5f6c 6c6d 203d 204f 7065 6e41 4928  ai_llm = OpenAI(
+00001420: 6170 695f 6b65 793d 223c 796f 7572 2d6f  api_key="<your-o
+00001430: 7065 6e61 692d 6170 692d 6b65 793e 2229  penai-api-key>")
+00001440: 0a0a 2320 4372 6561 7465 2070 726f 6d70  ..# Create promp
+00001450: 7420 7465 6d70 6c61 7465 730a 7469 746c  t templates.titl
+00001460: 655f 7465 6d70 6c61 7465 203d 2050 726f  e_template = Pro
+00001470: 6d70 7454 656d 706c 6174 6528 2257 6861  mptTemplate("Wha
+00001480: 7420 6973 2061 2067 6f6f 6420 7469 746c  t is a good titl
+00001490: 6520 6f66 2061 206d 6f76 6965 2061 626f  e of a movie abo
+000014a0: 7574 207b 746f 7069 637d 3f22 290a 736f  ut {topic}?").so
+000014b0: 6e67 5f74 656d 706c 6174 6520 3d20 5072  ng_template = Pr
+000014c0: 6f6d 7074 5465 6d70 6c61 7465 280a 2020  omptTemplate(.  
+000014d0: 2020 2257 6861 7420 6973 2061 2067 6f6f    "What is a goo
+000014e0: 6420 736f 6e67 2074 6974 6c65 206f 6620  d song title of 
+000014f0: 6120 736f 756e 6474 7261 636b 2066 6f72  a soundtrack for
+00001500: 2061 206d 6f76 6965 2063 616c 6c65 6420   a movie called 
+00001510: 7b6d 6f76 6965 5f74 6974 6c65 7d3f 220a  {movie_title}?".
+00001520: 290a 6368 6172 6163 7465 7273 5f74 656d  ).characters_tem
+00001530: 706c 6174 6520 3d20 5072 6f6d 7074 5465  plate = PromptTe
+00001540: 6d70 6c61 7465 280a 2020 2020 2257 6861  mplate(.    "Wha
+00001550: 7420 6172 6520 7477 6f20 6d61 696e 2063  t are two main c
+00001560: 6861 7261 6374 6572 7320 666f 7220 6120  haracters for a 
+00001570: 6d6f 7669 6520 6361 6c6c 6564 207b 6d6f  movie called {mo
+00001580: 7669 655f 7469 746c 657d 3f22 0a29 0a6c  vie_title}?".).l
+00001590: 7972 6963 735f 7465 6d70 6c61 7465 203d  yrics_template =
+000015a0: 2050 726f 6d70 7454 656d 706c 6174 6528   PromptTemplate(
+000015b0: 0a20 2020 2022 5772 6974 6520 6c79 7269  .    "Write lyri
+000015c0: 6373 206f 6620 6120 6d6f 7669 6520 736f  cs of a movie so
+000015d0: 6e67 2063 616c 6c65 6420 7b73 6f6e 675f  ng called {song_
+000015e0: 7469 746c 657d 2e20 5468 6520 6d61 696e  title}. The main
+000015f0: 2063 6861 7261 6374 6572 7320 6172 6520   characters are 
+00001600: 220a 2020 2020 227b 6d61 696e 5f63 6861  ".    "{main_cha
+00001610: 7261 6374 6572 737d 220a 290a 0a23 2043  racters}".)..# C
+00001620: 7265 6174 6520 666c 6f77 7374 6570 730a  reate flowsteps.
+00001630: 6d6f 7669 655f 7469 746c 655f 666c 6f77  movie_title_flow
+00001640: 7374 6570 203d 2046 6c6f 7753 7465 7028  step = FlowStep(
+00001650: 0a20 2020 206e 616d 653d 224d 6f76 6965  .    name="Movie
+00001660: 2054 6974 6c65 2046 6c6f 7773 7465 7022   Title Flowstep"
+00001670: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
+00001680: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
+00001690: 5f74 656d 706c 6174 653d 7469 746c 655f  _template=title_
+000016a0: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
+000016b0: 7470 7574 5f6b 6579 3d22 6d6f 7669 655f  tput_key="movie_
+000016c0: 7469 746c 6522 2c0a 290a 0a73 6f6e 675f  title",.)..song_
+000016d0: 7469 746c 655f 666c 6f77 7374 6570 203d  title_flowstep =
+000016e0: 2046 6c6f 7753 7465 7028 0a20 2020 206e   FlowStep(.    n
+000016f0: 616d 653d 2253 6f6e 6720 5469 746c 6520  ame="Song Title 
+00001700: 466c 6f77 7374 6570 222c 0a20 2020 206c  Flowstep",.    l
+00001710: 6c6d 3d6f 7065 6e61 695f 6c6c 6d2c 0a20  lm=openai_llm,. 
+00001720: 2020 2070 726f 6d70 745f 7465 6d70 6c61     prompt_templa
+00001730: 7465 3d73 6f6e 675f 7465 6d70 6c61 7465  te=song_template
+00001740: 2c0a 2020 2020 6f75 7470 7574 5f6b 6579  ,.    output_key
+00001750: 3d22 736f 6e67 5f74 6974 6c65 222c 0a29  ="song_title",.)
+00001760: 0a0a 6368 6172 6163 7465 7273 5f66 6c6f  ..characters_flo
+00001770: 7773 7465 7020 3d20 466c 6f77 5374 6570  wstep = FlowStep
+00001780: 280a 2020 2020 6e61 6d65 3d22 4368 6172  (.    name="Char
+00001790: 6163 7465 7273 2046 6c6f 7773 7465 7022  acters Flowstep"
+000017a0: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
+000017b0: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
+000017c0: 5f74 656d 706c 6174 653d 6368 6172 6163  _template=charac
+000017d0: 7465 7273 5f74 656d 706c 6174 652c 0a20  ters_template,. 
+000017e0: 2020 206f 7574 7075 745f 6b65 793d 226d     output_key="m
+000017f0: 6169 6e5f 6368 6172 6163 7465 7273 222c  ain_characters",
+00001800: 0a29 0a0a 736f 6e67 5f6c 7972 6963 735f  .)..song_lyrics_
+00001810: 666c 6f77 7374 6570 203d 2046 6c6f 7753  flowstep = FlowS
+00001820: 7465 7028 0a20 2020 206e 616d 653d 2253  tep(.    name="S
+00001830: 6f6e 6720 4c79 7269 6373 2046 6c6f 7773  ong Lyrics Flows
+00001840: 7465 7022 2c0a 2020 2020 6c6c 6d3d 6f70  tep",.    llm=op
+00001850: 656e 6169 5f6c 6c6d 2c0a 2020 2020 7072  enai_llm,.    pr
+00001860: 6f6d 7074 5f74 656d 706c 6174 653d 6c79  ompt_template=ly
+00001870: 7269 6373 5f74 656d 706c 6174 652c 0a20  rics_template,. 
+00001880: 2020 206f 7574 7075 745f 6b65 793d 2273     output_key="s
+00001890: 6f6e 675f 6c79 7269 6373 222c 0a29 0a0a  ong_lyrics",.)..
+000018a0: 2320 436f 6e6e 6563 7420 666c 6f77 7374  # Connect flowst
+000018b0: 6570 730a 6d6f 7669 655f 7469 746c 655f  eps.movie_title_
+000018c0: 666c 6f77 7374 6570 2e63 6f6e 6e65 6374  flowstep.connect
+000018d0: 2873 6f6e 675f 7469 746c 655f 666c 6f77  (song_title_flow
+000018e0: 7374 6570 2c20 6368 6172 6163 7465 7273  step, characters
+000018f0: 5f66 6c6f 7773 7465 702c 2073 6f6e 675f  _flowstep, song_
+00001900: 6c79 7269 6373 5f66 6c6f 7773 7465 7029  lyrics_flowstep)
+00001910: 0a73 6f6e 675f 7469 746c 655f 666c 6f77  .song_title_flow
+00001920: 7374 6570 2e63 6f6e 6e65 6374 2873 6f6e  step.connect(son
+00001930: 675f 6c79 7269 6373 5f66 6c6f 7773 7465  g_lyrics_flowste
+00001940: 7029 0a63 6861 7261 6374 6572 735f 666c  p).characters_fl
+00001950: 6f77 7374 6570 2e63 6f6e 6e65 6374 2873  owstep.connect(s
+00001960: 6f6e 675f 6c79 7269 6373 5f66 6c6f 7773  ong_lyrics_flows
+00001970: 7465 7029 0a0a 2320 4372 6561 7465 2061  tep)..# Create a
+00001980: 6e64 2072 756e 2046 6c6f 770a 736f 756e  nd run Flow.soun
+00001990: 6474 7261 636b 5f66 6c6f 7720 3d20 466c  dtrack_flow = Fl
+000019a0: 6f77 2874 6974 6c65 5f66 6c6f 7773 7465  ow(title_flowste
+000019b0: 7029 0a72 6573 756c 7473 203d 2073 6f75  p).results = sou
+000019c0: 6e64 7472 6163 6b5f 666c 6f77 2e73 7461  ndtrack_flow.sta
+000019d0: 7274 2874 6f70 6963 3d22 6672 6965 6e64  rt(topic="friend
+000019e0: 7368 6970 222c 2076 6572 626f 7365 3d54  ship", verbose=T
+000019f0: 7275 6529 0a60 6060 0a0a 2323 2320 4173  rue).```..### As
+00001a00: 796e 6320 466c 6f77 730a 536f 6d65 7469  ync Flows.Someti
+00001a10: 6d65 7320 6d75 6c74 6970 6c65 2066 6c6f  mes multiple flo
+00001a20: 7720 7374 6570 7320 6361 6e20 7275 6e20  w steps can run 
+00001a30: 696e 2070 6172 616c 6c65 6c20 6966 2061  in parallel if a
+00001a40: 6c6c 2074 6865 6972 2064 6570 656e 6465  ll their depende
+00001a50: 6e63 6965 7320 6172 6520 6d65 742e 200a  ncies are met. .
+00001a60: 466f 7220 6361 7365 7320 6c69 6b65 2074  For cases like t
+00001a70: 6869 732c 204c 4c4d 466c 6f77 7320 7072  his, LLMFlows pr
+00001a80: 6f76 6964 6573 2061 7379 6e63 2063 6c61  ovides async cla
+00001a90: 7373 6573 2074 6f20 696d 7072 6f76 6520  sses to improve 
+00001aa0: 7468 6520 7275 6e74 696d 6520 6f66 2061  the runtime of a
+00001ab0: 6e79 200a 636f 6d70 6c65 7820 666c 6f77  ny .complex flow
+00001ac0: 2062 7920 7275 6e6e 696e 6720 666c 6f77   by running flow
+00001ad0: 2073 7465 7073 2074 6861 7420 616c 7265   steps that alre
+00001ae0: 6164 7920 6861 7665 2061 6c6c 2074 6865  ady have all the
+00001af0: 6972 2072 6571 7569 7265 6420 696e 7075  ir required inpu
+00001b00: 7473 2069 6e20 0a70 6172 616c 6c65 6c2e  ts in .parallel.
+00001b10: 0a0a 6060 6070 7974 686f 6e0a 0a2e 2e2e  ..```python.....
+00001b20: 0a0a 6d6f 7669 655f 7469 746c 655f 666c  ..movie_title_fl
+00001b30: 6f77 7374 6570 203d 2041 7379 6e63 466c  owstep = AsyncFl
+00001b40: 6f77 5374 6570 280a 2020 2020 6e61 6d65  owStep(.    name
+00001b50: 3d22 466c 6f77 7374 6570 2031 222c 0a20  ="Flowstep 1",. 
+00001b60: 2020 206c 6c6d 3d6f 7065 6e61 695f 6c6c     llm=openai_ll
+00001b70: 6d2c 0a20 2020 2070 726f 6d70 745f 7465  m,.    prompt_te
+00001b80: 6d70 6c61 7465 3d74 6974 6c65 5f74 656d  mplate=title_tem
+00001b90: 706c 6174 652c 0a20 2020 206f 7574 7075  plate,.    outpu
+00001ba0: 745f 6b65 793d 226d 6f76 6965 5f74 6974  t_key="movie_tit
+00001bb0: 6c65 222c 0a29 0a0a 736f 6e67 5f74 6974  le",.)..song_tit
+00001bc0: 6c65 5f66 6c6f 7773 7465 7020 3d20 466c  le_flowstep = Fl
+00001bd0: 6f77 5374 6570 280a 2020 2020 6e61 6d65  owStep(.    name
+00001be0: 3d22 466c 6f77 7374 6570 2032 222c 0a20  ="Flowstep 2",. 
+00001bf0: 2020 206c 6c6d 3d6f 7065 6e61 695f 6c6c     llm=openai_ll
+00001c00: 6d2c 0a20 2020 2070 726f 6d70 745f 7465  m,.    prompt_te
+00001c10: 6d70 6c61 7465 3d73 6f6e 675f 7465 6d70  mplate=song_temp
+00001c20: 6c61 7465 2c0a 2020 2020 6f75 7470 7574  late,.    output
+00001c30: 5f6b 6579 3d22 736f 6e67 5f74 6974 6c65  _key="song_title
+00001c40: 222c 0a29 0a0a 6368 6172 6163 7465 7273  ",.)..characters
+00001c50: 5f66 6c6f 7773 7465 7020 3d20 4173 796e  _flowstep = Asyn
+00001c60: 6346 6c6f 7753 7465 7028 0a20 2020 206e  cFlowStep(.    n
+00001c70: 616d 653d 2246 6c6f 7773 7465 7020 3322  ame="Flowstep 3"
+00001c80: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
+00001c90: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
+00001ca0: 5f74 656d 706c 6174 653d 6368 6172 6163  _template=charac
+00001cb0: 7465 7273 5f74 656d 706c 6174 652c 0a20  ters_template,. 
+00001cc0: 2020 206f 7574 7075 745f 6b65 793d 226d     output_key="m
+00001cd0: 6169 6e5f 6368 6172 6163 7465 7273 222c  ain_characters",
+00001ce0: 0a29 0a0a 736f 6e67 5f6c 7972 6963 735f  .)..song_lyrics_
+00001cf0: 666c 6f77 7374 6570 203d 2041 7379 6e63  flowstep = Async
+00001d00: 466c 6f77 5374 6570 280a 2020 2020 6e61  FlowStep(.    na
+00001d10: 6d65 3d22 466c 6f77 7374 6570 2034 222c  me="Flowstep 4",
+00001d20: 0a20 2020 206c 6c6d 3d6f 7065 6e61 695f  .    llm=openai_
+00001d30: 6c6c 6d2c 0a20 2020 2070 726f 6d70 745f  llm,.    prompt_
+00001d40: 7465 6d70 6c61 7465 3d6c 7972 6963 735f  template=lyrics_
+00001d50: 7465 6d70 6c61 7465 2c0a 2020 2020 6f75  template,.    ou
+00001d60: 7470 7574 5f6b 6579 3d22 736f 6e67 5f6c  tput_key="song_l
+00001d70: 7972 6963 7322 2c0a 290a 0a2e 2e2e 0a0a  yrics",.).......
+00001d80: 6060 600a 0a43 6865 636b 206f 7572 2064  ```..Check our d
+00001d90: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+00001da0: 206d 6f72 6520 6578 616d 706c 6573 2c20   more examples, 
+00001db0: 7375 6368 2061 7320 696e 7465 6772 6174  such as integrat
+00001dc0: 696e 6720 7665 6374 6f72 2064 6174 6162  ing vector datab
+00001dd0: 6173 6573 2c20 0a63 7265 6174 696e 6720  ases, .creating 
+00001de0: 7175 6573 7469 6f6e 2d61 6e73 7765 7269  question-answeri
+00001df0: 6e67 2061 7070 7320 616e 6420 7765 6220  ng apps and web 
+00001e00: 6170 706c 6963 6174 696f 6e73 2077 6974  applications wit
+00001e10: 6820 466c 6173 6b20 616e 6420 4661 7374  h Flask and Fast
+00001e20: 4150 492e 0a0a 2323 2046 6561 7475 7265  API...## Feature
+00001e30: 730a 0a23 2323 202a 2a4c 4c4d 732a 2a0a  s..### **LLMs**.
+00001e40: 2d20 5574 696c 697a 6520 4c4c 4d73 2073  - Utilize LLMs s
+00001e50: 7563 6820 6173 204f 7065 6e41 4927 7320  uch as OpenAI's 
+00001e60: 4368 6174 4750 5420 746f 2067 656e 6572  ChatGPT to gener
+00001e70: 6174 6520 6e61 7475 7261 6c20 6c61 6e67  ate natural lang
+00001e80: 7561 6765 2074 6578 742e 0a2d 2043 6f6e  uage text..- Con
+00001e90: 6669 6775 7265 204c 4c4d 2063 6c61 7373  figure LLM class
+00001ea0: 6573 2065 6173 696c 792c 2063 686f 6f73  es easily, choos
+00001eb0: 696e 6720 7370 6563 6966 6963 206d 6f64  ing specific mod
+00001ec0: 656c 732c 2070 6172 616d 6574 6572 732c  els, parameters,
+00001ed0: 2061 6e64 2073 6574 7469 6e67 732e 0a2d   and settings..-
+00001ee0: 2042 656e 6566 6974 2066 726f 6d20 6175   Benefit from au
+00001ef0: 746f 6d61 7469 6320 7265 7472 6965 7320  tomatic retries 
+00001f00: 7768 656e 206d 6f64 656c 2063 616c 6c73  when model calls
+00001f10: 2066 6169 6c2c 2065 6e73 7572 696e 6720   fail, ensuring 
+00001f20: 7265 6c69 6162 6c65 204c 4c4d 200a 2020  reliable LLM .  
+00001f30: 696e 7465 7261 6374 696f 6e73 2e0a 0a23  interactions...#
+00001f40: 2323 202a 2a50 726f 6d70 7420 5465 6d70  ## **Prompt Temp
+00001f50: 6c61 7465 732a 2a0a 2d20 4372 6561 7465  lates**.- Create
+00001f60: 2064 796e 616d 6963 2070 726f 6d70 7473   dynamic prompts
+00001f70: 2075 7369 6e67 2050 726f 6d70 7420 5465   using Prompt Te
+00001f80: 6d70 6c61 7465 732c 2070 726f 7669 6469  mplates, providi
+00001f90: 6e67 2066 6c65 7869 626c 6520 616e 6420  ng flexible and 
+00001fa0: 6375 7374 6f6d 697a 6162 6c65 200a 2020  customizable .  
+00001fb0: 7465 7874 2067 656e 6572 6174 696f 6e2e  text generation.
+00001fc0: 0a2d 2044 6566 696e 6520 7661 7269 6162  .- Define variab
+00001fd0: 6c65 7320 7769 7468 696e 2070 726f 6d70  les within promp
+00001fe0: 7473 2074 6f20 6765 6e65 7261 7465 2070  ts to generate p
+00001ff0: 726f 6d70 7420 7374 7269 6e67 7320 7461  rompt strings ta
+00002000: 696c 6f72 6564 2074 6f20 7370 6563 6966  ilored to specif
+00002010: 6963 200a 2020 696e 7075 7473 2e0a 0a23  ic .  inputs...#
+00002020: 2323 202a 2a46 6c6f 7773 2061 6e64 2046  ## **Flows and F
+00002030: 6c6f 7753 7465 7073 2a2a 0a2d 2053 7472  lowSteps**.- Str
+00002040: 7563 7475 7265 204c 4c4d 2061 7070 6c69  ucture LLM appli
+00002050: 6361 7469 6f6e 7320 7573 696e 6720 466c  cations using Fl
+00002060: 6f77 7320 616e 6420 466c 6f77 5374 6570  ows and FlowStep
+00002070: 732c 2070 726f 7669 6469 6e67 2061 2063  s, providing a c
+00002080: 6c65 6172 2061 6e64 206f 7267 616e 697a  lear and organiz
+00002090: 6564 2066 7261 6d65 776f 726b 2066 6f72  ed framework for
+000020a0: 2065 7865 6375 7469 6e67 204c 4c4d 2069   executing LLM i
+000020b0: 6e74 6572 6163 7469 6f6e 732e 0a2d 2043  nteractions..- C
+000020c0: 6f6e 6e65 6374 2066 6c6f 7720 7374 6570  onnect flow step
+000020d0: 7320 746f 2070 6173 7320 6f75 7470 7574  s to pass output
+000020e0: 7320 6173 2069 6e70 7574 732c 2066 6163  s as inputs, fac
+000020f0: 696c 6974 6174 696e 6720 7365 616d 6c65  ilitating seamle
+00002100: 7373 2064 6174 6120 666c 6f77 2061 6e64  ss data flow and
+00002110: 0a20 2020 206d 6169 6e74 6169 6e69 6e67  .    maintaining
+00002120: 2061 2074 7261 6e73 7061 7265 6e74 204c   a transparent L
+00002130: 4c4d 2070 6970 656c 696e 652e 0a2d 204c  LM pipeline..- L
+00002140: 6576 6572 6167 6520 4173 796e 6320 466c  everage Async Fl
+00002150: 6f77 7320 746f 2072 756e 204c 4c4d 7320  ows to run LLMs 
+00002160: 696e 2070 6172 616c 6c65 6c20 7768 656e  in parallel when
+00002170: 2061 6c6c 2074 6865 6972 2069 6e70 7574   all their input
+00002180: 7320 6172 6520 6176 6169 6c61 626c 652c  s are available,
+00002190: 200a 2020 6f70 7469 6d69 7a69 6e67 2070   .  optimizing p
+000021a0: 6572 666f 726d 616e 6365 2061 6e64 2065  erformance and e
+000021b0: 6666 6963 6965 6e63 792e 0a2d 2049 6e63  fficiency..- Inc
+000021c0: 6f72 706f 7261 7465 2063 7573 746f 6d20  orporate custom 
+000021d0: 7374 7269 6e67 206d 616e 6970 756c 6174  string manipulat
+000021e0: 696f 6e20 6675 6e63 7469 6f6e 7320 6469  ion functions di
+000021f0: 7265 6374 6c79 2069 6e74 6f20 666c 6f77  rectly into flow
+00002200: 732c 2061 6c6c 6f77 696e 6720 0a20 2073  s, allowing .  s
+00002210: 7065 6369 616c 697a 6564 2074 6578 7420  pecialized text 
+00002220: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
+00002230: 7769 7468 6f75 7420 7265 6c79 696e 6720  without relying 
+00002240: 736f 6c65 6c79 206f 6e20 4c4c 4d20 6361  solely on LLM ca
+00002250: 6c6c 732e 0a0a 2323 2320 2a2a 5665 6374  lls...### **Vect
+00002260: 6f72 5374 6f72 6520 496e 7465 6772 6174  orStore Integrat
+00002270: 696f 6e73 2a2a 0a2d 2049 6e74 6567 7261  ions**.- Integra
+00002280: 7465 2077 6974 6820 7665 6374 6f72 2064  te with vector d
+00002290: 6174 6162 6173 6573 206c 696b 6520 5069  atabases like Pi
+000022a0: 6e65 636f 6e65 2075 7369 6e67 2074 6865  necone using the
+000022b0: 2056 6563 746f 7253 746f 7265 466c 6f77   VectorStoreFlow
+000022c0: 5374 6570 2c20 0a20 2065 6d70 6f77 6572  Step, .  empower
+000022d0: 696e 6720 6566 6669 6369 656e 7420 616e  ing efficient an
+000022e0: 6420 7363 616c 6162 6c65 2073 746f 7261  d scalable stora
+000022f0: 6765 2061 6e64 2072 6574 7269 6576 616c  ge and retrieval
+00002300: 206f 6620 7665 6374 6f72 2065 6d62 6564   of vector embed
+00002310: 6469 6e67 732e 0a2d 204c 6576 6572 6167  dings..- Leverag
+00002320: 6520 7665 6374 6f72 2064 6174 6162 6173  e vector databas
+00002330: 6573 2066 6f72 2073 6561 6d6c 6573 7320  es for seamless 
+00002340: 7374 6f72 6167 6520 616e 6420 7175 6572  storage and quer
+00002350: 7969 6e67 206f 6620 7665 6374 6f72 732c  ying of vectors,
+00002360: 2065 6e61 626c 696e 6720 7374 7261 6967   enabling straig
+00002370: 6874 666f 7277 6172 6420 696e 7465 6772  htforward integr
+00002380: 6174 696f 6e20 7769 7468 204c 4c4d 2d70  ation with LLM-p
+00002390: 6f77 6572 6564 2061 7070 6c69 6361 7469  owered applicati
+000023a0: 6f6e 732e 0a0a 2323 2320 2a2a 4361 6c6c  ons...### **Call
+000023b0: 6261 636b 732a 2a0a 2d20 4578 6563 7574  backs**.- Execut
+000023c0: 6520 6361 6c6c 6261 636b 2066 756e 6374  e callback funct
+000023d0: 696f 6e73 2061 7420 6469 6666 6572 656e  ions at differen
+000023e0: 7420 7374 6167 6573 2077 6974 6869 6e20  t stages within 
+000023f0: 666c 6f77 2073 7465 7073 2c20 656e 6162  flow steps, enab
+00002400: 6c69 6e67 2065 6e68 616e 6365 6420 6375  ling enhanced cu
+00002410: 7374 6f6d 697a 6174 696f 6e2c 206c 6f67  stomization, log
+00002420: 6769 6e67 2c20 7472 6163 696e 672c 206f  ging, tracing, o
+00002430: 7220 6f74 6865 7220 7370 6563 6966 6963  r other specific
+00002440: 2069 6e74 6567 7261 7469 6f6e 732e 0a2d   integrations..-
+00002450: 2055 7469 6c69 7a65 2063 616c 6c62 6163   Utilize callbac
+00002460: 6b73 2074 6f20 636f 6d70 7265 6865 6e73  ks to comprehens
+00002470: 6976 656c 7920 636f 6e74 726f 6c20 616e  ively control an
+00002480: 6420 6d6f 6e69 746f 7220 4c4c 4d2d 706f  d monitor LLM-po
+00002490: 7765 7265 6420 6170 7073 2c20 656e 7375  wered apps, ensu
+000024a0: 7269 6e67 200a 2020 636c 6561 7220 7669  ring .  clear vi
+000024b0: 7369 6269 6c69 7479 2069 6e74 6f20 7468  sibility into th
+000024c0: 6520 6578 6563 7574 696f 6e20 7072 6f63  e execution proc
+000024d0: 6573 732e 0a0a 2323 2320 2a2a 4578 706c  ess...### **Expl
+000024e0: 6963 6974 2041 5049 2061 6e64 2046 756c  icit API and Ful
+000024f0: 6c20 5472 616e 7370 6172 656e 6379 2a2a  l Transparency**
+00002500: 0a57 6974 6820 4c4c 4d46 6c6f 7773 2079  .With LLMFlows y
+00002510: 6f75 2068 6176 6520 7468 6520 6675 6c6c  ou have the full
+00002520: 2063 6f6e 7472 6f6c 2074 6f20 6372 6561   control to crea
+00002530: 7465 2065 7870 6c69 6369 7420 6170 706c  te explicit appl
+00002540: 6963 6174 696f 6e73 2077 6974 686f 7574  ications without
+00002550: 2061 6e79 2068 6964 6465 6e20 7072 6f6d   any hidden prom
+00002560: 7074 7320 6f72 2070 7265 6465 6669 6e65  pts or predefine
+00002570: 6420 6265 6861 7669 6f72 732e 0a0a 496e  d behaviors...In
+00002580: 2061 6464 6974 696f 6e20 4c4c 4d46 6c6f   addition LLMFlo
+00002590: 7773 2061 6c6c 6f77 7320 796f 7520 746f  ws allows you to
+000025a0: 2061 6e73 7765 7220 7175 6573 7469 6f6e   answer question
+000025b0: 7320 7375 6368 2061 733a 0a0a 2d20 5768  s such as:..- Wh
+000025c0: 656e 2077 6173 2061 2070 6172 7469 6375  en was a particu
+000025d0: 6c61 7220 666c 6f77 7374 6570 2072 756e  lar flowstep run
+000025e0: 3f0a 2d20 486f 7720 6d75 6368 2074 696d  ?.- How much tim
+000025f0: 6520 6469 6420 6974 2074 616b 653f 0a2d  e did it take?.-
+00002600: 2057 6861 7420 7765 7265 2074 6865 2069   What were the i
+00002610: 6e70 7574 2076 6172 6961 626c 6573 3f0a  nput variables?.
+00002620: 2d20 5768 6174 2077 6173 2074 6865 2070  - What was the p
+00002630: 726f 6d70 7420 7465 6d70 6c61 7465 3f0a  rompt template?.
+00002640: 2d20 5768 6174 2064 6964 2074 6865 2070  - What did the p
+00002650: 726f 6d70 7420 6c6f 6f6b 206c 696b 653f  rompt look like?
+00002660: 0a2d 2057 6861 7420 7761 7320 7468 6520  .- What was the 
+00002670: 6578 6163 7420 636f 6e66 6967 7572 6174  exact configurat
+00002680: 696f 6e20 6f66 2074 6865 206d 6f64 656c  ion of the model
+00002690: 3f0a 2d20 486f 7720 6d61 6e79 2074 696d  ?.- How many tim
+000026a0: 6573 2064 6964 2077 6520 7265 7472 7920  es did we retry 
+000026b0: 7468 6520 7265 7175 6573 743f 0a2d 2057  the request?.- W
+000026c0: 6861 7420 7761 7320 7468 6520 7261 7720  hat was the raw 
+000026d0: 6461 7461 2074 6865 2041 5049 2072 6574  data the API ret
+000026e0: 7572 6e65 643f 0a2d 2048 6f77 206d 616e  urned?.- How man
+000026f0: 7920 746f 6b65 6e73 2077 6572 6520 7573  y tokens were us
+00002700: 6564 3f0a 2d20 5768 6174 2077 6173 2074  ed?.- What was t
+00002710: 6865 2066 696e 616c 2072 6573 756c 743f  he final result?
+00002720: 0a0a 2323 204c 6963 656e 7365 0a4c 4c4d  ..## License.LLM
+00002730: 466c 6f77 7320 6973 2063 6f76 6572 6564  Flows is covered
+00002740: 2062 7920 7468 6520 4d49 5420 6c69 6365   by the MIT lice
+00002750: 6e73 652e 2046 6f72 206d 6f72 6520 696e  nse. For more in
+00002760: 666f 726d 6174 696f 6e2c 2063 6865 636b  formation, check
+00002770: 2060 4c49 4345 4e43 452e 6d64 602e 0a0a   `LICENCE.md`...
+00002780: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00002790: 5468 616e 6b20 796f 7520 666f 7220 7370  Thank you for sp
+000027a0: 656e 6469 6e67 2074 696d 6520 676f 696e  ending time goin
+000027b0: 6720 6f76 6572 206f 7572 2052 4541 444d  g over our READM
+000027c0: 4521 2049 6620 796f 7520 6669 6e64 204c  E! If you find L
+000027d0: 4c4d 466c 6f77 7320 6578 6369 7469 6e67  LMFlows exciting
+000027e0: 2061 6e64 200a 796f 7520 6172 6520 636f   and .you are co
+000027f0: 6e73 6964 6572 696e 6720 636f 6e74 7269  nsidering contri
+00002800: 6275 7469 6e67 2c20 706c 6561 7365 2063  buting, please c
+00002810: 6865 636b 205b 6043 4f4e 5452 4942 5554  heck [`CONTRIBUT
+00002820: 494e 472e 6d64 605d 2868 7474 7073 3a2f  ING.md`](https:/
+00002830: 2f67 6974 6875 622e 636f 6d2f 7374 6f79  /github.com/stoy
+00002840: 616e 2d73 746f 7961 6e6f 762f 6c6c 6d66  an-stoyanov/llmf
+00002850: 6c6f 7773 2f62 6c6f 622f 6d61 696e 2f43  lows/blob/main/C
+00002860: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+00002870: 0a                                       .
```

### Comparing `llmflows-0.0.8/llmflows/callbacks/async_base_callback.py` & `llmflows-0.0.9/llmflows/callbacks/async_base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/callbacks/async_functional_callback.py` & `llmflows-0.0.9/llmflows/callbacks/async_functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/callbacks/base_callback.py` & `llmflows-0.0.9/llmflows/callbacks/base_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/callbacks/functional_callback.py` & `llmflows-0.0.9/llmflows/callbacks/functional_callback.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/async_base_flow.py` & `llmflows-0.0.9/llmflows/flows/async_base_flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/async_base_flowstep.py` & `llmflows-0.0.9/llmflows/flows/async_base_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/async_chat_flowstep.py` & `llmflows-0.0.9/llmflows/flows/async_chat_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/async_flow.py` & `llmflows-0.0.9/llmflows/flows/async_flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/async_flowstep.py` & `llmflows-0.0.9/llmflows/flows/async_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/base_flow.py` & `llmflows-0.0.9/llmflows/flows/base_flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/base_flowstep.py` & `llmflows-0.0.9/llmflows/flows/base_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/chat_flowstep.py` & `llmflows-0.0.9/llmflows/flows/chat_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/flow.py` & `llmflows-0.0.9/llmflows/flows/flow.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/flowstep.py` & `llmflows-0.0.9/llmflows/flows/flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/functional_flowstep.py` & `llmflows-0.0.9/llmflows/flows/functional_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/flows/vectorstore_flowstep.py` & `llmflows-0.0.9/llmflows/flows/vectorstore_flowstep.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/llms/llm.py` & `llmflows-0.0.9/llmflows/llms/llm.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/llms/llm_utils.py` & `llmflows-0.0.9/llmflows/llms/llm_utils.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/llms/message_history.py` & `llmflows-0.0.9/llmflows/llms/message_history.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/llms/openai.py` & `llmflows-0.0.9/llmflows/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/llms/openai_chat.py` & `llmflows-0.0.9/llmflows/llms/openai_chat.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/llms/openai_embeddings.py` & `llmflows-0.0.9/llmflows/llms/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/prompts/prompt_template.py` & `llmflows-0.0.9/llmflows/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/vectorstores/pinecone.py` & `llmflows-0.0.9/llmflows/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/vectorstores/vector_doc.py` & `llmflows-0.0.9/llmflows/vectorstores/vector_doc.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows/vectorstores/vector_store.py` & `llmflows-0.0.9/llmflows/vectorstores/vector_store.py`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/llmflows.egg-info/PKG-INFO` & `llmflows-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,631 +1,616 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6c6c 6d66  : 2.1.Name: llmf
-00000020: 6c6f 7773 0a56 6572 7369 6f6e 3a20 302e  lows.Version: 0.
-00000030: 302e 380a 5375 6d6d 6172 793a 204c 4c4d  0.8.Summary: LLM
-00000040: 466c 6f77 7320 2d20 5369 6d70 6c65 2c20  Flows - Simple, 
-00000050: 4578 706c 6963 6974 2061 6e64 2054 7261  Explicit and Tra
-00000060: 6e73 7061 7265 6e74 204c 4c4d 2041 7070  nsparent LLM App
-00000070: 730a 4175 7468 6f72 3a20 5374 6f79 616e  s.Author: Stoyan
-00000080: 2053 746f 7961 6e6f 760a 5072 6f6a 6563   Stoyanov.Projec
-00000090: 742d 5552 4c3a 2048 6f6d 6570 6167 652c  t-URL: Homepage,
-000000a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000000b0: 636f 6d2f 7374 6f79 616e 2d73 746f 7961  com/stoyan-stoya
-000000c0: 6e6f 762f 6c6c 6d66 6c6f 7773 0a50 726f  nov/llmflows.Pro
-000000d0: 6a65 6374 2d55 524c 3a20 6769 7468 7562  ject-URL: github
-000000e0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-000000f0: 2e63 6f6d 2f73 746f 7961 6e2d 7374 6f79  .com/stoyan-stoy
-00000100: 616e 6f76 2f6c 6c6d 666c 6f77 730a 436c  anov/llmflows.Cl
-00000110: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000120: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000130: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-00000140: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-00000150: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000160: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000170: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
-00000180: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000190: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
-000001a0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-000001b0: 203e 3d33 2e39 0a44 6573 6372 6970 7469   >=3.9.Descripti
-000001c0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000001d0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-000001e0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-000001f0: 454e 5345 0a0a 2320 4c4c 4d46 6c6f 7773  ENSE..# LLMFlows
-00000200: 202d 2053 696d 706c 652c 2045 7870 6c69   - Simple, Expli
-00000210: 6369 742c 2061 6e64 2054 7261 6e73 7061  cit, and Transpa
-00000220: 7265 6e74 204c 4c4d 2041 7070 730a 0a3c  rent LLM Apps..<
-00000230: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000240: 3e0a 2020 3c69 6d67 2073 7479 6c65 3d22  >.  <img style="
-00000250: 7769 6474 683a 2038 3025 2220 7372 633d  width: 80%" src=
-00000260: 2264 6f63 732f 6c6c 6d66 6c6f 7773 5f6c  "docs/llmflows_l
-00000270: 6173 745f 6c6f 676f 2e70 6e67 2220 2f3e  ast_logo.png" />
-00000280: 0a3c 2f70 3e0a 0a5b 215b 5477 6974 7465  .</p>..[![Twitte
-00000290: 725d 2868 7474 7073 3a2f 2f69 6d67 2e73  r](https://img.s
-000002a0: 6869 656c 6473 2e69 6f2f 7477 6974 7465  hields.io/twitte
-000002b0: 722f 666f 6c6c 6f77 2f4c 4c4d 466c 6f77  r/follow/LLMFlow
-000002c0: 733f 7374 796c 653d 736f 6369 616c 295d  s?style=social)]
-000002d0: 2868 7474 7073 3a2f 2f74 7769 7474 6572  (https://twitter
-000002e0: 2e63 6f6d 2f4c 4c4d 466c 6f77 7329 0a21  .com/LLMFlows).!
-000002f0: 5b50 796c 696e 7420 776f 726b 666c 6f77  [Pylint workflow
-00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000310: 2e63 6f6d 2f73 746f 7961 6e2d 7374 6f79  .com/stoyan-stoy
-00000320: 616e 6f76 2f6c 6c6d 666c 6f77 2f61 6374  anov/llmflow/act
-00000330: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00000340: 796c 696e 742e 796d 6c2f 6261 6467 652e  ylint.yml/badge.
-00000350: 7376 6729 0a21 5b4c 6963 656e 7365 5d28  svg).![License](
-00000360: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000370: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
-00000380: 6365 6e73 652f 7374 6f79 616e 2d73 746f  cense/stoyan-sto
-00000390: 7961 6e6f 762f 6c6c 6d66 6c6f 7729 0a21  yanov/llmflow).!
-000003a0: 5b50 7950 695d 2868 7474 7073 3a2f 2f69  [PyPi](https://i
-000003b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000003c0: 7069 2f76 2f6c 6c6d 666c 6f77 7329 0a21  pi/v/llmflows).!
-000003d0: 5b53 7461 7273 5d28 6874 7470 733a 2f2f  [Stars](https://
-000003e0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-000003f0: 6974 6875 622f 7374 6172 732f 7374 6f79  ithub/stars/stoy
-00000400: 616e 2d73 746f 7961 6e6f 762f 6c6c 6d66  an-stoyanov/llmf
-00000410: 6c6f 773f 7374 796c 653d 736f 6369 616c  low?style=social
-00000420: 290a 215b 5265 6c65 6173 6520 6461 7465  ).![Release date
-00000430: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000440: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000450: 7265 6c65 6173 652d 6461 7465 2f73 746f  release-date/sto
-00000460: 7961 6e2d 7374 6f79 616e 6f76 2f6c 6c6d  yan-stoyanov/llm
-00000470: 666c 6f77 3f73 7479 6c65 3d73 6f63 6961  flow?style=socia
-00000480: 6c29 0a0a 446f 6375 6d65 6e74 6174 696f  l)..Documentatio
-00000490: 6e3a 205b 6874 7470 733a 2f2f 7265 6164  n: [https://read
-000004a0: 7468 6564 6f63 732e 6f72 675d 2868 7474  thedocs.org](htt
-000004b0: 7073 3a2f 2f72 6561 6474 6865 646f 6373  ps://readthedocs
-000004c0: 2e6f 7267 2f29 3c62 722f 3e0a 5079 5049  .org/)<br/>.PyPI
-000004d0: 3a20 5b68 7474 7073 3a2f 2f70 7970 692e  : [https://pypi.
-000004e0: 6f72 672f 7072 6f6a 6563 742f 6c6c 6d66  org/project/llmf
-000004f0: 6c6f 7773 5d28 6874 7470 733a 2f2f 7079  lows](https://py
-00000500: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
-00000510: 6c6d 666c 6f77 732f 293c 2f62 723e 0a54  lmflows/)</br>.T
-00000520: 7769 7474 6572 3a20 5b68 7474 7073 3a2f  witter: [https:/
-00000530: 2f74 7769 7474 6572 2e63 6f6d 2f4c 4c4d  /twitter.com/LLM
-00000540: 466c 6f77 735d 2868 7474 7073 3a2f 2f74  Flows](https://t
-00000550: 7769 7474 6572 2e63 6f6d 2f4c 4c4d 466c  witter.com/LLMFl
-00000560: 6f77 7329 3c62 722f 3e0a 5375 6273 7461  ows)<br/>.Substa
-00000570: 636b 3a20 5b68 7474 7073 3a2f 2f6c 6c6d  ck: [https://llm
-00000580: 666c 6f77 732e 7375 6273 7461 636b 2e63  flows.substack.c
-00000590: 6f6d 5d28 6874 7470 733a 2f2f 6c6c 6d66  om](https://llmf
-000005a0: 6c6f 7773 2e73 7562 7374 6163 6b2e 636f  lows.substack.co
-000005b0: 6d2f 293c 6272 2f3e 0a0a 2323 2041 626f  m/)<br/>..## Abo
-000005c0: 7574 0a4c 4c4d 466c 6f77 7320 6973 2061  ut.LLMFlows is a
-000005d0: 2066 7261 6d65 776f 726b 2066 6f72 2062   framework for b
-000005e0: 7569 6c64 696e 6720 7369 6d70 6c65 2c20  uilding simple, 
-000005f0: 6578 706c 6963 6974 2c20 616e 6420 7472  explicit, and tr
-00000600: 616e 7370 6172 656e 7420 4c4c 4d28 4c61  ansparent LLM(La
-00000610: 7267 6520 0a4c 616e 6775 6167 6520 4d6f  rge .Language Mo
-00000620: 6465 6c29 2061 7070 6c69 6361 7469 6f6e  del) application
-00000630: 732e 0a0a 2323 2049 6e73 7461 6c6c 6174  s...## Installat
-00000640: 696f 6e0a 6060 600a 7069 7020 696e 7374  ion.```.pip inst
-00000650: 616c 6c20 6c6c 6d66 6c6f 7773 0a60 6060  all llmflows.```
-00000660: 0a0a 2323 2050 6869 6c6f 736f 7068 790a  ..## Philosophy.
-00000670: 0a23 2323 202a 2a53 696d 706c 652a 2a0a  .### **Simple**.
-00000680: 4f75 7220 676f 616c 2069 7320 746f 2062  Our goal is to b
-00000690: 7569 6c64 2061 2073 696d 706c 652c 2077  uild a simple, w
-000006a0: 656c 6c2d 646f 6375 6d65 6e74 6564 2066  ell-documented f
-000006b0: 7261 6d65 776f 726b 2077 6974 6820 6d69  ramework with mi
-000006c0: 6e69 6d61 6c20 6162 7374 7261 6374 696f  nimal abstractio
-000006d0: 6e73 2074 6861 7420 0a61 6c6c 6f77 2075  ns that .allow u
-000006e0: 7365 7273 2074 6f20 6275 696c 6420 666c  sers to build fl
-000006f0: 6578 6962 6c65 204c 4c4d 2d70 6f77 6572  exible LLM-power
-00000700: 6564 2061 7070 7320 7769 7468 6f75 7420  ed apps without 
-00000710: 636f 6d70 726f 6d69 7369 6e67 206f 6e20  compromising on 
-00000720: 6361 7061 6269 6c69 7469 6573 2e0a 0a23  capabilities...#
-00000730: 2323 202a 2a45 7870 6c69 6369 742a 2a0a  ## **Explicit**.
-00000740: 5765 2077 616e 7420 746f 2063 7265 6174  We want to creat
-00000750: 6520 616e 2065 7870 6c69 6369 7420 4150  e an explicit AP
-00000760: 4920 656e 6162 6c69 6e67 2075 7365 7273  I enabling users
-00000770: 2074 6f20 7772 6974 6520 636c 6561 6e20   to write clean 
-00000780: 616e 6420 7265 6164 6162 6c65 2063 6f64  and readable cod
-00000790: 6520 7768 696c 6520 0a65 6173 696c 7920  e while .easily 
-000007a0: 6372 6561 7469 6e67 2063 6f6d 706c 6578  creating complex
-000007b0: 2066 6c6f 7773 206f 6620 4c4c 4d73 2069   flows of LLMs i
-000007c0: 6e74 6572 6163 7469 6e67 2077 6974 6820  nteracting with 
-000007d0: 6561 6368 206f 7468 6572 2e20 4c4c 4d46  each other. LLMF
-000007e0: 6c6f 7773 2720 636c 6173 7365 7320 0a67  lows' classes .g
-000007f0: 6976 6520 7573 6572 7320 6675 6c6c 2063  ive users full c
-00000800: 6f6e 7472 6f6c 2061 6e64 2064 6f20 6e6f  ontrol and do no
-00000810: 7420 6861 7665 2061 6e79 2068 6964 6465  t have any hidde
-00000820: 6e20 7072 6f6d 7074 7320 6f72 204c 4c4d  n prompts or LLM
-00000830: 2063 616c 6c73 2e20 0a0a 2323 2320 2a2a   calls. ..### **
-00000840: 5472 616e 7370 6172 656e 742a 2a0a 5765  Transparent**.We
-00000850: 2061 696d 2074 6f20 6865 6c70 2075 7365   aim to help use
-00000860: 7273 2068 6176 6520 6675 6c6c 2074 7261  rs have full tra
-00000870: 6e73 7061 7265 6e63 7920 6f6e 2074 6865  nsparency on the
-00000880: 6972 204c 4c4d 2d70 6f77 6572 6564 2061  ir LLM-powered a
-00000890: 7070 7320 6279 2070 726f 7669 6469 6e67  pps by providing
-000008a0: 200a 7472 6163 6561 626c 6520 666c 6f77   .traceable flow
-000008b0: 7320 616e 6420 636f 6d70 6c65 7465 2069  s and complete i
-000008c0: 6e66 6f72 6d61 7469 6f6e 2066 6f72 2065  nformation for e
-000008d0: 6163 6820 6170 7020 636f 6d70 6f6e 656e  ach app componen
-000008e0: 742c 206d 616b 696e 6720 6974 2065 6173  t, making it eas
-000008f0: 7920 746f 200a 6d6f 6e69 746f 722c 206d  y to .monitor, m
-00000900: 6169 6e74 6169 6e2c 2061 6e64 2064 6562  aintain, and deb
-00000910: 7567 2e0a 0a23 2320 4765 7474 696e 6720  ug...## Getting 
-00000920: 5374 6172 7465 640a 2323 2320 4c4c 4d73  Started.### LLMs
-00000930: 0a4c 4c4d 7320 6172 6520 6f6e 6520 6f66  .LLMs are one of
-00000940: 2074 6865 206d 6169 6e20 6162 7374 7261   the main abstra
-00000950: 6374 696f 6e73 2069 6e20 4c4c 4d46 6c6f  ctions in LLMFlo
-00000960: 7773 2e20 4c4c 4d20 636c 6173 7365 7320  ws. LLM classes 
-00000970: 6172 6520 7772 6170 7065 7273 2061 726f  are wrappers aro
-00000980: 756e 6420 4c4c 4d20 0a41 5049 7320 7375  und LLM .APIs su
-00000990: 6368 2061 7320 4f70 656e 4149 2773 2041  ch as OpenAI's A
-000009a0: 5049 732e 2054 6865 7920 7072 6f76 6964  PIs. They provid
-000009b0: 6520 6d65 7468 6f64 7320 666f 7220 636f  e methods for co
-000009c0: 6e66 6967 7572 696e 6720 616e 6420 6361  nfiguring and ca
-000009d0: 6c6c 696e 6720 7468 6573 6520 4150 4973  lling these APIs
-000009e0: 2c20 0a72 6574 7279 696e 6720 6661 696c  , .retrying fail
-000009f0: 6564 2063 616c 6c73 2c20 616e 6420 666f  ed calls, and fo
-00000a00: 726d 6174 7469 6e67 2074 6865 2072 6573  rmatting the res
-00000a10: 706f 6e73 6573 2e0a 0a60 6060 7079 7468  ponses...```pyth
-00000a20: 6f6e 0a66 726f 6d20 6c6c 6d66 6c6f 7773  on.from llmflows
-00000a30: 2e6c 6c6d 7320 696d 706f 7274 204f 7065  .llms import Ope
-00000a40: 6e41 490a 0a6c 6c6d 203d 204f 7065 6e41  nAI..llm = OpenA
-00000a50: 4928 6170 695f 6b65 793d 223c 796f 7572  I(api_key="<your
-00000a60: 2d6f 7065 6e61 692d 6170 692d 6b65 793e  -openai-api-key>
-00000a70: 2229 0a0a 7265 7375 6c74 2c20 6361 6c6c  ")..result, call
-00000a80: 5f64 6174 612c 206d 6f64 656c 5f63 6f6e  _data, model_con
-00000a90: 6669 6720 3d20 6c6c 6d2e 6765 6e65 7261  fig = llm.genera
-00000aa0: 7465 280a 2020 2070 726f 6d70 743d 2247  te(.   prompt="G
-00000ab0: 656e 6572 6174 6520 6120 636f 6f6c 2074  enerate a cool t
-00000ac0: 6974 6c65 2066 6f72 2061 6e20 3830 7320  itle for an 80s 
-00000ad0: 726f 636b 2073 6f6e 6722 0a29 0a60 6060  rock song".).```
-00000ae0: 0a0a 0a23 2323 2050 726f 6d70 7454 656d  ...### PromptTem
-00000af0: 706c 6174 6573 0a54 6865 2060 5072 6f6d  plates.The `Prom
-00000b00: 7074 5465 6d70 6c61 7465 6020 636c 6173  ptTemplate` clas
-00000b10: 7320 616c 6c6f 7773 2075 7320 746f 2063  s allows us to c
-00000b20: 7265 6174 6520 7374 7269 6e67 7320 7769  reate strings wi
-00000b30: 7468 2076 6172 6961 626c 6573 2074 6861  th variables tha
-00000b40: 7420 7765 2063 616e 2066 696c 6c20 0a69  t we can fill .i
-00000b50: 6e20 6479 6e61 6d69 6361 6c6c 7920 6c61  n dynamically la
-00000b60: 7465 7220 6f6e 2e20 4f6e 6365 2061 2070  ter on. Once a p
-00000b70: 726f 6d70 7420 7465 6d70 6c61 7465 206f  rompt template o
-00000b80: 626a 6563 7420 6973 2063 7265 6174 6564  bject is created
-00000b90: 2061 6e20 6163 7475 616c 2070 726f 6d70   an actual promp
-00000ba0: 7420 6361 6e20 0a62 6520 6765 6e65 7261  t can .be genera
-00000bb0: 7465 6420 6279 2070 726f 7669 6469 6e67  ted by providing
-00000bc0: 2074 6865 2072 6571 7569 7265 6420 7661   the required va
-00000bd0: 7269 6162 6c65 732e 0a0a 6060 6070 7974  riables...```pyt
-00000be0: 686f 6e0a 6672 6f6d 206c 6c6d 666c 6f77  hon.from llmflow
-00000bf0: 732e 6c6c 6d73 2069 6d70 6f72 7420 4f70  s.llms import Op
-00000c00: 656e 4149 0a66 726f 6d20 6c6c 6d66 6c6f  enAI.from llmflo
-00000c10: 7773 2e70 726f 6d70 7473 2069 6d70 6f72  ws.prompts impor
-00000c20: 7420 5072 6f6d 7074 5465 6d70 6c61 7465  t PromptTemplate
-00000c30: 0a0a 0a70 726f 6d70 745f 7465 6d70 6c61  ...prompt_templa
-00000c40: 7465 203d 2050 726f 6d70 7454 656d 706c  te = PromptTempl
-00000c50: 6174 6528 0a20 2020 2070 726f 6d70 743d  ate(.    prompt=
-00000c60: 2247 656e 6572 6174 6520 6120 7469 746c  "Generate a titl
-00000c70: 6520 666f 7220 6120 3930 7320 6869 702d  e for a 90s hip-
-00000c80: 686f 7020 736f 6e67 2061 626f 7574 207b  hop song about {
-00000c90: 746f 7069 637d 2e22 0a29 0a6c 6c6d 5f70  topic}.".).llm_p
-00000ca0: 726f 6d70 7420 3d20 7072 6f6d 7074 5f74  rompt = prompt_t
-00000cb0: 656d 706c 6174 652e 6765 745f 7072 6f6d  emplate.get_prom
-00000cc0: 7074 2874 6f70 6963 3d22 6672 6965 6e64  pt(topic="friend
-00000cd0: 7368 6970 2229 0a0a 7072 696e 7428 6c6c  ship")..print(ll
-00000ce0: 6d5f 7072 6f6d 7074 290a 0a6c 6c6d 203d  m_prompt)..llm =
-00000cf0: 204f 7065 6e41 4928 6170 695f 6b65 793d   OpenAI(api_key=
-00000d00: 223c 796f 7572 2d6f 7065 6e61 692d 6170  "<your-openai-ap
-00000d10: 692d 6b65 793e 2229 0a73 6f6e 675f 7469  i-key>").song_ti
-00000d20: 746c 6520 3d20 6c6c 6d2e 6765 6e65 7261  tle = llm.genera
-00000d30: 7465 286c 6c6d 5f70 726f 6d70 7429 0a0a  te(llm_prompt)..
-00000d40: 7072 696e 7428 736f 6e67 5f74 6974 6c65  print(song_title
-00000d50: 290a 6060 600a 0a23 2323 2043 6861 7420  ).```..### Chat 
-00000d60: 4c4c 4d73 0a55 6e6c 696b 6520 7265 6775  LLMs.Unlike regu
-00000d70: 6c61 7220 4c4c 4d73 2074 6861 7420 6f6e  lar LLMs that on
-00000d80: 6c79 2072 6571 7569 7265 2061 2070 726f  ly require a pro
-00000d90: 6d70 7420 746f 2067 656e 6572 6174 6520  mpt to generate 
-00000da0: 7465 7874 2c20 6368 6174 204c 4c4d 7320  text, chat LLMs 
-00000db0: 7265 7175 6972 6520 6120 0a63 6f6e 7665  require a .conve
-00000dc0: 7273 6174 696f 6e20 6869 7374 6f72 792e  rsation history.
-00000dd0: 2054 6865 2063 6f6e 7665 7273 6174 696f   The conversatio
-00000de0: 6e20 6869 7374 6f72 7920 6973 2072 6570  n history is rep
-00000df0: 7265 7365 6e74 6564 200a 6173 2061 206c  resented .as a l
-00000e00: 6973 7420 6f66 206d 6573 7361 6765 7320  ist of messages 
-00000e10: 6265 7477 6565 6e20 6120 7573 6572 2061  between a user a
-00000e20: 6e64 2061 6e20 6173 7369 7374 616e 742e  nd an assistant.
-00000e30: 2054 6869 7320 636f 6e76 6572 7361 7469   This conversati
-00000e40: 6f6e 2068 6973 746f 7279 2069 7320 0a73  on history is .s
-00000e50: 656e 7420 746f 2074 6865 206d 6f64 656c  ent to the model
-00000e60: 2c20 616e 6420 6120 6e65 7720 6d65 7373  , and a new mess
-00000e70: 6167 6520 6973 2067 656e 6572 6174 6564  age is generated
-00000e80: 2062 6173 6564 206f 6e20 6974 2e0a 0a4c   based on it...L
-00000e90: 4c4d 466c 6f77 7320 7072 6f76 6964 6573  LMFlows provides
-00000ea0: 2061 2060 4d65 7373 6167 6548 6973 746f   a `MessageHisto
-00000eb0: 7279 6020 636c 6173 7320 746f 206d 616e  ry` class to man
-00000ec0: 6167 6520 7468 6520 7265 7175 6972 6564  age the required
-00000ed0: 2063 6f6e 7665 7273 6174 696f 6e20 6869   conversation hi
-00000ee0: 7374 6f72 7920 0a66 6f72 2063 6861 7420  story .for chat 
-00000ef0: 4c4c 4d73 2e0a 0a59 6f75 2063 616e 2062  LLMs...You can b
-00000f00: 7569 6c64 2061 2073 696d 706c 6520 6368  uild a simple ch
-00000f10: 6174 626f 7420 6279 2075 7369 6e67 2074  atbot by using t
-00000f20: 6865 2060 4f70 656e 4149 4368 6174 6020  he `OpenAIChat` 
-00000f30: 616e 6420 604d 6573 7361 6765 4869 7374  and `MessageHist
-00000f40: 6f72 7960 2063 6c61 7373 6573 3a0a 0a60  ory` classes:..`
-00000f50: 6060 7079 7468 6f6e 0a66 726f 6d20 6c6c  ``python.from ll
-00000f60: 6d66 6c6f 7773 2e6c 6c6d 7320 696d 706f  mflows.llms impo
-00000f70: 7274 204f 7065 6e41 4943 6861 742c 204d  rt OpenAIChat, M
-00000f80: 6573 7361 6765 4869 7374 6f72 790a 0a6c  essageHistory..l
-00000f90: 6c6d 203d 204f 7065 6e41 4943 6861 7428  lm = OpenAIChat(
-00000fa0: 6170 695f 6b65 793d 223c 796f 7572 2d6f  api_key="<your-o
-00000fb0: 7065 6e61 692d 6170 692d 6b65 793e 2229  penai-api-key>")
-00000fc0: 0a6d 6573 7361 6765 5f68 6973 746f 7279  .message_history
-00000fd0: 203d 204d 6573 7361 6765 4869 7374 6f72   = MessageHistor
-00000fe0: 7928 290a 0a77 6869 6c65 2054 7275 653a  y()..while True:
-00000ff0: 0a20 2020 2075 7365 725f 6d65 7373 6167  .    user_messag
-00001000: 6520 3d20 696e 7075 7428 2259 6f75 3a22  e = input("You:"
-00001010: 290a 2020 2020 6d65 7373 6167 655f 6869  ).    message_hi
-00001020: 7374 6f72 792e 6164 645f 7573 6572 5f6d  story.add_user_m
-00001030: 6573 7361 6765 2875 7365 725f 6d65 7373  essage(user_mess
-00001040: 6167 6529 0a0a 2020 2020 6c6c 6d5f 7265  age)..    llm_re
-00001050: 7370 6f6e 7365 2c20 6361 6c6c 5f64 6174  sponse, call_dat
-00001060: 612c 206d 6f64 656c 5f63 6f6e 6669 6720  a, model_config 
-00001070: 3d20 6c6c 6d2e 6765 6e65 7261 7465 286d  = llm.generate(m
-00001080: 6573 7361 6765 5f68 6973 746f 7279 290a  essage_history).
-00001090: 2020 2020 6d65 7373 6167 655f 6869 7374      message_hist
-000010a0: 6f72 792e 6164 645f 6169 5f6d 6573 7361  ory.add_ai_messa
-000010b0: 6765 286c 6c6d 5f72 6573 706f 6e73 6529  ge(llm_response)
-000010c0: 0a0a 2020 2020 7072 696e 7428 6622 4c4c  ..    print(f"LL
-000010d0: 4d3a 207b 6c6c 6d5f 7265 7370 6f6e 7365  M: {llm_response
-000010e0: 7d22 290a 6060 600a 0a23 2323 204c 4c4d  }").```..### LLM
-000010f0: 2046 6c6f 7773 0a4f 6674 656e 2074 696d   Flows.Often tim
-00001100: 6573 2c20 7265 616c 2d77 6f72 6c64 2061  es, real-world a
-00001110: 7070 6c69 6361 7469 6f6e 7320 6361 6e20  pplications can 
-00001120: 6265 206d 6f72 6520 636f 6d70 6c65 7820  be more complex 
-00001130: 616e 6420 6361 6e20 6861 7665 2064 6570  and can have dep
-00001140: 656e 6465 6e63 6965 7320 0a62 6574 7765  endencies .betwe
-00001150: 656e 2070 726f 6d70 7473 2061 6e64 204c  en prompts and L
-00001160: 4c4d 2063 616c 6c73 2e20 466f 7220 6578  LM calls. For ex
-00001170: 616d 706c 653a 0a0a 215b 436f 6d70 6c65  ample:..![Comple
-00001180: 7820 666c 6f77 5d28 646f 6373 2f63 6f6d  x flow](docs/com
-00001190: 706c 6578 5f66 6c6f 772e 706e 6729 0a0a  plex_flow.png)..
-000011a0: 5768 656e 2079 6f75 2077 616e 7420 746f  When you want to
-000011b0: 2062 7569 6c64 2061 7070 7320 7769 7468   build apps with
-000011c0: 2063 6f6d 706c 6578 2064 6570 656e 6465   complex depende
-000011d0: 6e63 6965 7320 796f 7520 6361 6e20 7573  ncies you can us
-000011e0: 6520 7468 6520 6046 6c6f 7760 2061 6e64  e the `Flow` and
-000011f0: 200a 6046 6c6f 7773 7465 7060 2063 6c61   .`Flowstep` cla
-00001200: 7373 6573 2e20 4c4c 4d46 6c6f 7773 2077  sses. LLMFlows w
-00001210: 696c 6c20 6669 6775 7265 206f 7574 2074  ill figure out t
-00001220: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
-00001230: 616e 6420 6d61 6b65 2073 7572 6520 6561  and make sure ea
-00001240: 6368 200a 666c 6f77 7374 6570 2072 756e  ch .flowstep run
-00001250: 7320 6f6e 6c79 2077 6865 6e20 616c 6c20  s only when all 
-00001260: 6974 7320 6465 7065 6e64 656e 6369 6573  its dependencies
-00001270: 2061 7265 206d 6574 3a0a 0a60 6060 7079   are met:..```py
-00001280: 7468 6f6e 0a66 726f 6d20 6c6c 6d66 6c6f  thon.from llmflo
-00001290: 7773 2e66 6c6f 7773 2069 6d70 6f72 7420  ws.flows import 
-000012a0: 466c 6f77 2c20 466c 6f77 5374 6570 0a66  Flow, FlowStep.f
-000012b0: 726f 6d20 6c6c 6d66 6c6f 7773 2e6c 6c6d  rom llmflows.llm
-000012c0: 7320 696d 706f 7274 204f 7065 6e41 490a  s import OpenAI.
-000012d0: 6672 6f6d 206c 6c6d 666c 6f77 732e 7072  from llmflows.pr
-000012e0: 6f6d 7074 7320 696d 706f 7274 2050 726f  ompts import Pro
-000012f0: 6d70 7454 656d 706c 6174 650a 0a6f 7065  mptTemplate..ope
-00001300: 6e61 695f 6c6c 6d20 3d20 4f70 656e 4149  nai_llm = OpenAI
-00001310: 2861 7069 5f6b 6579 3d22 3c79 6f75 722d  (api_key="<your-
-00001320: 6f70 656e 6169 2d61 7069 2d6b 6579 3e22  openai-api-key>"
-00001330: 290a 0a23 2043 7265 6174 6520 7072 6f6d  )..# Create prom
-00001340: 7074 2074 656d 706c 6174 6573 0a74 6974  pt templates.tit
-00001350: 6c65 5f74 656d 706c 6174 6520 3d20 5072  le_template = Pr
-00001360: 6f6d 7074 5465 6d70 6c61 7465 2822 5768  omptTemplate("Wh
-00001370: 6174 2069 7320 6120 676f 6f64 2074 6974  at is a good tit
-00001380: 6c65 206f 6620 6120 6d6f 7669 6520 6162  le of a movie ab
-00001390: 6f75 7420 7b74 6f70 6963 7d3f 2229 0a73  out {topic}?").s
-000013a0: 6f6e 675f 7465 6d70 6c61 7465 203d 2050  ong_template = P
-000013b0: 726f 6d70 7454 656d 706c 6174 6528 0a20  romptTemplate(. 
-000013c0: 2020 2022 5768 6174 2069 7320 6120 676f     "What is a go
-000013d0: 6f64 2073 6f6e 6720 7469 746c 6520 6f66  od song title of
-000013e0: 2061 2073 6f75 6e64 7472 6163 6b20 666f   a soundtrack fo
-000013f0: 7220 6120 6d6f 7669 6520 6361 6c6c 6564  r a movie called
-00001400: 207b 6d6f 7669 655f 7469 746c 657d 3f22   {movie_title}?"
-00001410: 0a29 0a63 6861 7261 6374 6572 735f 7465  .).characters_te
-00001420: 6d70 6c61 7465 203d 2050 726f 6d70 7454  mplate = PromptT
-00001430: 656d 706c 6174 6528 0a20 2020 2022 5768  emplate(.    "Wh
-00001440: 6174 2061 7265 2074 776f 206d 6169 6e20  at are two main 
-00001450: 6368 6172 6163 7465 7273 2066 6f72 2061  characters for a
-00001460: 206d 6f76 6965 2063 616c 6c65 6420 7b6d   movie called {m
-00001470: 6f76 6965 5f74 6974 6c65 7d3f 220a 290a  ovie_title}?".).
-00001480: 6c79 7269 6373 5f74 656d 706c 6174 6520  lyrics_template 
-00001490: 3d20 5072 6f6d 7074 5465 6d70 6c61 7465  = PromptTemplate
-000014a0: 280a 2020 2020 2257 7269 7465 206c 7972  (.    "Write lyr
-000014b0: 6963 7320 6f66 2061 206d 6f76 6965 2073  ics of a movie s
-000014c0: 6f6e 6720 6361 6c6c 6564 207b 736f 6e67  ong called {song
-000014d0: 5f74 6974 6c65 7d2e 2054 6865 206d 6169  _title}. The mai
-000014e0: 6e20 6368 6172 6163 7465 7273 2061 7265  n characters are
-000014f0: 2022 0a20 2020 2022 7b6d 6169 6e5f 6368   ".    "{main_ch
-00001500: 6172 6163 7465 7273 7d22 0a29 0a0a 2320  aracters}".)..# 
-00001510: 4372 6561 7465 2066 6c6f 7773 7465 7073  Create flowsteps
-00001520: 0a6d 6f76 6965 5f74 6974 6c65 5f66 6c6f  .movie_title_flo
-00001530: 7773 7465 7020 3d20 466c 6f77 5374 6570  wstep = FlowStep
-00001540: 280a 2020 2020 6e61 6d65 3d22 4d6f 7669  (.    name="Movi
-00001550: 6520 5469 746c 6520 466c 6f77 7374 6570  e Title Flowstep
-00001560: 222c 0a20 2020 206c 6c6d 3d6f 7065 6e61  ",.    llm=opena
-00001570: 695f 6c6c 6d2c 0a20 2020 2070 726f 6d70  i_llm,.    promp
-00001580: 745f 7465 6d70 6c61 7465 3d74 6974 6c65  t_template=title
-00001590: 5f74 656d 706c 6174 652c 0a20 2020 206f  _template,.    o
-000015a0: 7574 7075 745f 6b65 793d 226d 6f76 6965  utput_key="movie
-000015b0: 5f74 6974 6c65 222c 0a29 0a0a 736f 6e67  _title",.)..song
-000015c0: 5f74 6974 6c65 5f66 6c6f 7773 7465 7020  _title_flowstep 
-000015d0: 3d20 466c 6f77 5374 6570 280a 2020 2020  = FlowStep(.    
-000015e0: 6e61 6d65 3d22 536f 6e67 2054 6974 6c65  name="Song Title
-000015f0: 2046 6c6f 7773 7465 7022 2c0a 2020 2020   Flowstep",.    
-00001600: 6c6c 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a  llm=openai_llm,.
-00001610: 2020 2020 7072 6f6d 7074 5f74 656d 706c      prompt_templ
-00001620: 6174 653d 736f 6e67 5f74 656d 706c 6174  ate=song_templat
-00001630: 652c 0a20 2020 206f 7574 7075 745f 6b65  e,.    output_ke
-00001640: 793d 2273 6f6e 675f 7469 746c 6522 2c0a  y="song_title",.
-00001650: 290a 0a63 6861 7261 6374 6572 735f 666c  )..characters_fl
-00001660: 6f77 7374 6570 203d 2046 6c6f 7753 7465  owstep = FlowSte
-00001670: 7028 0a20 2020 206e 616d 653d 2243 6861  p(.    name="Cha
-00001680: 7261 6374 6572 7320 466c 6f77 7374 6570  racters Flowstep
-00001690: 222c 0a20 2020 206c 6c6d 3d6f 7065 6e61  ",.    llm=opena
-000016a0: 695f 6c6c 6d2c 0a20 2020 2070 726f 6d70  i_llm,.    promp
-000016b0: 745f 7465 6d70 6c61 7465 3d63 6861 7261  t_template=chara
-000016c0: 6374 6572 735f 7465 6d70 6c61 7465 2c0a  cters_template,.
-000016d0: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
-000016e0: 6d61 696e 5f63 6861 7261 6374 6572 7322  main_characters"
-000016f0: 2c0a 290a 0a73 6f6e 675f 6c79 7269 6373  ,.)..song_lyrics
-00001700: 5f66 6c6f 7773 7465 7020 3d20 466c 6f77  _flowstep = Flow
-00001710: 5374 6570 280a 2020 2020 6e61 6d65 3d22  Step(.    name="
-00001720: 536f 6e67 204c 7972 6963 7320 466c 6f77  Song Lyrics Flow
-00001730: 7374 6570 222c 0a20 2020 206c 6c6d 3d6f  step",.    llm=o
-00001740: 7065 6e61 695f 6c6c 6d2c 0a20 2020 2070  penai_llm,.    p
-00001750: 726f 6d70 745f 7465 6d70 6c61 7465 3d6c  rompt_template=l
-00001760: 7972 6963 735f 7465 6d70 6c61 7465 2c0a  yrics_template,.
-00001770: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
-00001780: 736f 6e67 5f6c 7972 6963 7322 2c0a 290a  song_lyrics",.).
-00001790: 0a23 2043 6f6e 6e65 6374 2066 6c6f 7773  .# Connect flows
-000017a0: 7465 7073 0a6d 6f76 6965 5f74 6974 6c65  teps.movie_title
-000017b0: 5f66 6c6f 7773 7465 702e 636f 6e6e 6563  _flowstep.connec
-000017c0: 7428 736f 6e67 5f74 6974 6c65 5f66 6c6f  t(song_title_flo
-000017d0: 7773 7465 702c 2063 6861 7261 6374 6572  wstep, character
-000017e0: 735f 666c 6f77 7374 6570 2c20 736f 6e67  s_flowstep, song
-000017f0: 5f6c 7972 6963 735f 666c 6f77 7374 6570  _lyrics_flowstep
-00001800: 290a 736f 6e67 5f74 6974 6c65 5f66 6c6f  ).song_title_flo
-00001810: 7773 7465 702e 636f 6e6e 6563 7428 736f  wstep.connect(so
-00001820: 6e67 5f6c 7972 6963 735f 666c 6f77 7374  ng_lyrics_flowst
-00001830: 6570 290a 6368 6172 6163 7465 7273 5f66  ep).characters_f
-00001840: 6c6f 7773 7465 702e 636f 6e6e 6563 7428  lowstep.connect(
-00001850: 736f 6e67 5f6c 7972 6963 735f 666c 6f77  song_lyrics_flow
-00001860: 7374 6570 290a 0a23 2043 7265 6174 6520  step)..# Create 
-00001870: 616e 6420 7275 6e20 466c 6f77 0a73 6f75  and run Flow.sou
-00001880: 6e64 7472 6163 6b5f 666c 6f77 203d 2046  ndtrack_flow = F
-00001890: 6c6f 7728 7469 746c 655f 666c 6f77 7374  low(title_flowst
-000018a0: 6570 290a 7265 7375 6c74 7320 3d20 736f  ep).results = so
-000018b0: 756e 6474 7261 636b 5f66 6c6f 772e 7374  undtrack_flow.st
-000018c0: 6172 7428 746f 7069 633d 2266 7269 656e  art(topic="frien
-000018d0: 6473 6869 7022 2c20 7665 7262 6f73 653d  dship", verbose=
-000018e0: 5472 7565 290a 6060 600a 0a23 2323 2041  True).```..### A
-000018f0: 7379 6e63 2046 6c6f 7773 0a53 6f6d 6574  sync Flows.Somet
-00001900: 696d 6573 206d 756c 7469 706c 6520 666c  imes multiple fl
-00001910: 6f77 2073 7465 7073 2063 616e 2072 756e  ow steps can run
-00001920: 2069 6e20 7061 7261 6c6c 656c 2069 6620   in parallel if 
-00001930: 616c 6c20 7468 6569 7220 6465 7065 6e64  all their depend
-00001940: 656e 6369 6573 2061 7265 206d 6574 2e20  encies are met. 
-00001950: 0a46 6f72 2063 6173 6573 206c 696b 6520  .For cases like 
-00001960: 7468 6973 2c20 4c4c 4d46 6c6f 7773 2070  this, LLMFlows p
-00001970: 726f 7669 6465 7320 6173 796e 6320 636c  rovides async cl
-00001980: 6173 7365 7320 746f 2069 6d70 726f 7665  asses to improve
-00001990: 2074 6865 2072 756e 7469 6d65 206f 6620   the runtime of 
-000019a0: 616e 7920 0a63 6f6d 706c 6578 2066 6c6f  any .complex flo
-000019b0: 7720 6279 2072 756e 6e69 6e67 2066 6c6f  w by running flo
-000019c0: 7720 7374 6570 7320 7468 6174 2061 6c72  w steps that alr
-000019d0: 6561 6479 2068 6176 6520 616c 6c20 7468  eady have all th
-000019e0: 6569 7220 7265 7175 6972 6564 2069 6e70  eir required inp
-000019f0: 7574 7320 696e 200a 7061 7261 6c6c 656c  uts in .parallel
-00001a00: 2e0a 0a60 6060 7079 7468 6f6e 0a0a 2e2e  ...```python....
-00001a10: 2e0a 0a6d 6f76 6965 5f74 6974 6c65 5f66  ...movie_title_f
-00001a20: 6c6f 7773 7465 7020 3d20 4173 796e 6346  lowstep = AsyncF
-00001a30: 6c6f 7753 7465 7028 0a20 2020 206e 616d  lowStep(.    nam
-00001a40: 653d 2246 6c6f 7773 7465 7020 3122 2c0a  e="Flowstep 1",.
-00001a50: 2020 2020 6c6c 6d3d 6f70 656e 6169 5f6c      llm=openai_l
-00001a60: 6c6d 2c0a 2020 2020 7072 6f6d 7074 5f74  lm,.    prompt_t
-00001a70: 656d 706c 6174 653d 7469 746c 655f 7465  emplate=title_te
-00001a80: 6d70 6c61 7465 2c0a 2020 2020 6f75 7470  mplate,.    outp
-00001a90: 7574 5f6b 6579 3d22 6d6f 7669 655f 7469  ut_key="movie_ti
-00001aa0: 746c 6522 2c0a 290a 0a73 6f6e 675f 7469  tle",.)..song_ti
-00001ab0: 746c 655f 666c 6f77 7374 6570 203d 2046  tle_flowstep = F
-00001ac0: 6c6f 7753 7465 7028 0a20 2020 206e 616d  lowStep(.    nam
-00001ad0: 653d 2246 6c6f 7773 7465 7020 3222 2c0a  e="Flowstep 2",.
-00001ae0: 2020 2020 6c6c 6d3d 6f70 656e 6169 5f6c      llm=openai_l
-00001af0: 6c6d 2c0a 2020 2020 7072 6f6d 7074 5f74  lm,.    prompt_t
-00001b00: 656d 706c 6174 653d 736f 6e67 5f74 656d  emplate=song_tem
-00001b10: 706c 6174 652c 0a20 2020 206f 7574 7075  plate,.    outpu
-00001b20: 745f 6b65 793d 2273 6f6e 675f 7469 746c  t_key="song_titl
-00001b30: 6522 2c0a 290a 0a63 6861 7261 6374 6572  e",.)..character
-00001b40: 735f 666c 6f77 7374 6570 203d 2041 7379  s_flowstep = Asy
-00001b50: 6e63 466c 6f77 5374 6570 280a 2020 2020  ncFlowStep(.    
-00001b60: 6e61 6d65 3d22 466c 6f77 7374 6570 2033  name="Flowstep 3
-00001b70: 222c 0a20 2020 206c 6c6d 3d6f 7065 6e61  ",.    llm=opena
-00001b80: 695f 6c6c 6d2c 0a20 2020 2070 726f 6d70  i_llm,.    promp
-00001b90: 745f 7465 6d70 6c61 7465 3d63 6861 7261  t_template=chara
-00001ba0: 6374 6572 735f 7465 6d70 6c61 7465 2c0a  cters_template,.
-00001bb0: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
-00001bc0: 6d61 696e 5f63 6861 7261 6374 6572 7322  main_characters"
-00001bd0: 2c0a 290a 0a73 6f6e 675f 6c79 7269 6373  ,.)..song_lyrics
-00001be0: 5f66 6c6f 7773 7465 7020 3d20 4173 796e  _flowstep = Asyn
-00001bf0: 6346 6c6f 7753 7465 7028 0a20 2020 206e  cFlowStep(.    n
-00001c00: 616d 653d 2246 6c6f 7773 7465 7020 3422  ame="Flowstep 4"
-00001c10: 2c0a 2020 2020 6c6c 6d3d 6f70 656e 6169  ,.    llm=openai
-00001c20: 5f6c 6c6d 2c0a 2020 2020 7072 6f6d 7074  _llm,.    prompt
-00001c30: 5f74 656d 706c 6174 653d 6c79 7269 6373  _template=lyrics
-00001c40: 5f74 656d 706c 6174 652c 0a20 2020 206f  _template,.    o
-00001c50: 7574 7075 745f 6b65 793d 2273 6f6e 675f  utput_key="song_
-00001c60: 6c79 7269 6373 222c 0a29 0a0a 2e2e 2e0a  lyrics",.)......
-00001c70: 0a60 6060 0a0a 4368 6563 6b20 6f75 7220  .```..Check our 
-00001c80: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00001c90: 7220 6d6f 7265 2065 7861 6d70 6c65 732c  r more examples,
-00001ca0: 2073 7563 6820 6173 2069 6e74 6567 7261   such as integra
-00001cb0: 7469 6e67 2076 6563 746f 7220 6461 7461  ting vector data
-00001cc0: 6261 7365 732c 200a 6372 6561 7469 6e67  bases, .creating
-00001cd0: 2071 7565 7374 696f 6e2d 616e 7377 6572   question-answer
-00001ce0: 696e 6720 6170 7073 2061 6e64 2077 6562  ing apps and web
-00001cf0: 2061 7070 6c69 6361 7469 6f6e 7320 7769   applications wi
-00001d00: 7468 2046 6c61 736b 2061 6e64 2046 6173  th Flask and Fas
-00001d10: 7441 5049 2e0a 0a23 2320 4665 6174 7572  tAPI...## Featur
-00001d20: 6573 0a0a 2323 2320 2a2a 4c4c 4d73 2a2a  es..### **LLMs**
-00001d30: 0a2d 2055 7469 6c69 7a65 204c 4c4d 7320  .- Utilize LLMs 
-00001d40: 7375 6368 2061 7320 4f70 656e 4149 2773  such as OpenAI's
-00001d50: 2043 6861 7447 5054 2074 6f20 6765 6e65   ChatGPT to gene
-00001d60: 7261 7465 206e 6174 7572 616c 206c 616e  rate natural lan
-00001d70: 6775 6167 6520 7465 7874 2e0a 2d20 436f  guage text..- Co
-00001d80: 6e66 6967 7572 6520 4c4c 4d20 636c 6173  nfigure LLM clas
-00001d90: 7365 7320 6561 7369 6c79 2c20 6368 6f6f  ses easily, choo
-00001da0: 7369 6e67 2073 7065 6369 6669 6320 6d6f  sing specific mo
-00001db0: 6465 6c73 2c20 7061 7261 6d65 7465 7273  dels, parameters
-00001dc0: 2c20 616e 6420 7365 7474 696e 6773 2e0a  , and settings..
-00001dd0: 2d20 4265 6e65 6669 7420 6672 6f6d 2061  - Benefit from a
-00001de0: 7574 6f6d 6174 6963 2072 6574 7269 6573  utomatic retries
-00001df0: 2077 6865 6e20 6d6f 6465 6c20 6361 6c6c   when model call
-00001e00: 7320 6661 696c 2c20 656e 7375 7269 6e67  s fail, ensuring
-00001e10: 2072 656c 6961 626c 6520 4c4c 4d20 0a20   reliable LLM . 
-00001e20: 2069 6e74 6572 6163 7469 6f6e 732e 0a0a   interactions...
-00001e30: 2323 2320 2a2a 5072 6f6d 7074 2054 656d  ### **Prompt Tem
-00001e40: 706c 6174 6573 2a2a 0a2d 2043 7265 6174  plates**.- Creat
-00001e50: 6520 6479 6e61 6d69 6320 7072 6f6d 7074  e dynamic prompt
-00001e60: 7320 7573 696e 6720 5072 6f6d 7074 2054  s using Prompt T
-00001e70: 656d 706c 6174 6573 2c20 7072 6f76 6964  emplates, provid
-00001e80: 696e 6720 666c 6578 6962 6c65 2061 6e64  ing flexible and
-00001e90: 2063 7573 746f 6d69 7a61 626c 6520 0a20   customizable . 
-00001ea0: 2074 6578 7420 6765 6e65 7261 7469 6f6e   text generation
-00001eb0: 2e0a 2d20 4465 6669 6e65 2076 6172 6961  ..- Define varia
-00001ec0: 626c 6573 2077 6974 6869 6e20 7072 6f6d  bles within prom
-00001ed0: 7074 7320 746f 2067 656e 6572 6174 6520  pts to generate 
-00001ee0: 7072 6f6d 7074 2073 7472 696e 6773 2074  prompt strings t
-00001ef0: 6169 6c6f 7265 6420 746f 2073 7065 6369  ailored to speci
-00001f00: 6669 6320 0a20 2069 6e70 7574 732e 0a0a  fic .  inputs...
-00001f10: 2323 2320 2a2a 466c 6f77 7320 616e 6420  ### **Flows and 
-00001f20: 466c 6f77 5374 6570 732a 2a0a 2d20 5374  FlowSteps**.- St
-00001f30: 7275 6374 7572 6520 4c4c 4d20 6170 706c  ructure LLM appl
-00001f40: 6963 6174 696f 6e73 2075 7369 6e67 2046  ications using F
-00001f50: 6c6f 7773 2061 6e64 2046 6c6f 7753 7465  lows and FlowSte
-00001f60: 7073 2c20 7072 6f76 6964 696e 6720 6120  ps, providing a 
-00001f70: 636c 6561 7220 616e 6420 6f72 6761 6e69  clear and organi
-00001f80: 7a65 6420 6672 616d 6577 6f72 6b20 666f  zed framework fo
-00001f90: 7220 6578 6563 7574 696e 6720 4c4c 4d20  r executing LLM 
-00001fa0: 696e 7465 7261 6374 696f 6e73 2e0a 2d20  interactions..- 
-00001fb0: 436f 6e6e 6563 7420 666c 6f77 2073 7465  Connect flow ste
-00001fc0: 7073 2074 6f20 7061 7373 206f 7574 7075  ps to pass outpu
-00001fd0: 7473 2061 7320 696e 7075 7473 2c20 6661  ts as inputs, fa
-00001fe0: 6369 6c69 7461 7469 6e67 2073 6561 6d6c  cilitating seaml
-00001ff0: 6573 7320 6461 7461 2066 6c6f 7720 616e  ess data flow an
-00002000: 640a 2020 2020 6d61 696e 7461 696e 696e  d.    maintainin
-00002010: 6720 6120 7472 616e 7370 6172 656e 7420  g a transparent 
-00002020: 4c4c 4d20 7069 7065 6c69 6e65 2e0a 2d20  LLM pipeline..- 
-00002030: 4c65 7665 7261 6765 2041 7379 6e63 2046  Leverage Async F
-00002040: 6c6f 7773 2074 6f20 7275 6e20 4c4c 4d73  lows to run LLMs
-00002050: 2069 6e20 7061 7261 6c6c 656c 2077 6865   in parallel whe
-00002060: 6e20 616c 6c20 7468 6569 7220 696e 7075  n all their inpu
-00002070: 7473 2061 7265 2061 7661 696c 6162 6c65  ts are available
-00002080: 2c20 0a20 206f 7074 696d 697a 696e 6720  , .  optimizing 
-00002090: 7065 7266 6f72 6d61 6e63 6520 616e 6420  performance and 
-000020a0: 6566 6669 6369 656e 6379 2e0a 2d20 496e  efficiency..- In
-000020b0: 636f 7270 6f72 6174 6520 6375 7374 6f6d  corporate custom
-000020c0: 2073 7472 696e 6720 6d61 6e69 7075 6c61   string manipula
-000020d0: 7469 6f6e 2066 756e 6374 696f 6e73 2064  tion functions d
-000020e0: 6972 6563 746c 7920 696e 746f 2066 6c6f  irectly into flo
-000020f0: 7773 2c20 616c 6c6f 7769 6e67 200a 2020  ws, allowing .  
-00002100: 7370 6563 6961 6c69 7a65 6420 7465 7874  specialized text
-00002110: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
-00002120: 2077 6974 686f 7574 2072 656c 7969 6e67   without relying
-00002130: 2073 6f6c 656c 7920 6f6e 204c 4c4d 2063   solely on LLM c
-00002140: 616c 6c73 2e0a 0a23 2323 202a 2a56 6563  alls...### **Vec
-00002150: 746f 7253 746f 7265 2049 6e74 6567 7261  torStore Integra
-00002160: 7469 6f6e 732a 2a0a 2d20 496e 7465 6772  tions**.- Integr
-00002170: 6174 6520 7769 7468 2076 6563 746f 7220  ate with vector 
-00002180: 6461 7461 6261 7365 7320 6c69 6b65 2050  databases like P
-00002190: 696e 6563 6f6e 6520 7573 696e 6720 7468  inecone using th
-000021a0: 6520 5665 6374 6f72 5374 6f72 6546 6c6f  e VectorStoreFlo
-000021b0: 7753 7465 702c 200a 2020 656d 706f 7765  wStep, .  empowe
-000021c0: 7269 6e67 2065 6666 6963 6965 6e74 2061  ring efficient a
-000021d0: 6e64 2073 6361 6c61 626c 6520 7374 6f72  nd scalable stor
-000021e0: 6167 6520 616e 6420 7265 7472 6965 7661  age and retrieva
-000021f0: 6c20 6f66 2076 6563 746f 7220 656d 6265  l of vector embe
-00002200: 6464 696e 6773 2e0a 2d20 4c65 7665 7261  ddings..- Levera
-00002210: 6765 2076 6563 746f 7220 6461 7461 6261  ge vector databa
-00002220: 7365 7320 666f 7220 7365 616d 6c65 7373  ses for seamless
-00002230: 2073 746f 7261 6765 2061 6e64 2071 7565   storage and que
-00002240: 7279 696e 6720 6f66 2076 6563 746f 7273  rying of vectors
-00002250: 2c20 656e 6162 6c69 6e67 2073 7472 6169  , enabling strai
-00002260: 6768 7466 6f72 7761 7264 2069 6e74 6567  ghtforward integ
-00002270: 7261 7469 6f6e 2077 6974 6820 4c4c 4d2d  ration with LLM-
-00002280: 706f 7765 7265 6420 6170 706c 6963 6174  powered applicat
-00002290: 696f 6e73 2e0a 0a23 2323 202a 2a43 616c  ions...### **Cal
-000022a0: 6c62 6163 6b73 2a2a 0a2d 2045 7865 6375  lbacks**.- Execu
-000022b0: 7465 2063 616c 6c62 6163 6b20 6675 6e63  te callback func
-000022c0: 7469 6f6e 7320 6174 2064 6966 6665 7265  tions at differe
-000022d0: 6e74 2073 7461 6765 7320 7769 7468 696e  nt stages within
-000022e0: 2066 6c6f 7720 7374 6570 732c 2065 6e61   flow steps, ena
-000022f0: 626c 696e 6720 656e 6861 6e63 6564 2063  bling enhanced c
-00002300: 7573 746f 6d69 7a61 7469 6f6e 2c20 6c6f  ustomization, lo
-00002310: 6767 696e 672c 2074 7261 6369 6e67 2c20  gging, tracing, 
-00002320: 6f72 206f 7468 6572 2073 7065 6369 6669  or other specifi
-00002330: 6320 696e 7465 6772 6174 696f 6e73 2e0a  c integrations..
-00002340: 2d20 5574 696c 697a 6520 6361 6c6c 6261  - Utilize callba
-00002350: 636b 7320 746f 2063 6f6d 7072 6568 656e  cks to comprehen
-00002360: 7369 7665 6c79 2063 6f6e 7472 6f6c 2061  sively control a
-00002370: 6e64 206d 6f6e 6974 6f72 204c 4c4d 2d70  nd monitor LLM-p
-00002380: 6f77 6572 6564 2061 7070 732c 2065 6e73  owered apps, ens
-00002390: 7572 696e 6720 0a20 2063 6c65 6172 2076  uring .  clear v
-000023a0: 6973 6962 696c 6974 7920 696e 746f 2074  isibility into t
-000023b0: 6865 2065 7865 6375 7469 6f6e 2070 726f  he execution pro
-000023c0: 6365 7373 2e0a 0a23 2323 202a 2a45 7870  cess...### **Exp
-000023d0: 6c69 6369 7420 4150 4920 616e 6420 4675  licit API and Fu
-000023e0: 6c6c 2054 7261 6e73 7061 7265 6e63 792a  ll Transparency*
-000023f0: 2a0a 5769 7468 204c 4c4d 466c 6f77 7320  *.With LLMFlows 
-00002400: 796f 7520 6861 7665 2074 6865 2066 756c  you have the ful
-00002410: 6c20 636f 6e74 726f 6c20 746f 2063 7265  l control to cre
-00002420: 6174 6520 6578 706c 6963 6974 2061 7070  ate explicit app
-00002430: 6c69 6361 7469 6f6e 7320 7769 7468 6f75  lications withou
-00002440: 7420 616e 7920 6869 6464 656e 2070 726f  t any hidden pro
-00002450: 6d70 7473 206f 7220 7072 6564 6566 696e  mpts or predefin
-00002460: 6564 2062 6568 6176 696f 7273 2e0a 0a49  ed behaviors...I
-00002470: 6e20 6164 6469 7469 6f6e 204c 4c4d 466c  n addition LLMFl
-00002480: 6f77 7320 616c 6c6f 7773 2079 6f75 2074  ows allows you t
-00002490: 6f20 616e 7377 6572 2071 7565 7374 696f  o answer questio
-000024a0: 6e73 2073 7563 6820 6173 3a0a 0a2d 2057  ns such as:..- W
-000024b0: 6865 6e20 7761 7320 6120 7061 7274 6963  hen was a partic
-000024c0: 756c 6172 2066 6c6f 7773 7465 7020 7275  ular flowstep ru
-000024d0: 6e3f 0a2d 2048 6f77 206d 7563 6820 7469  n?.- How much ti
-000024e0: 6d65 2064 6964 2069 7420 7461 6b65 3f0a  me did it take?.
-000024f0: 2d20 5768 6174 2077 6572 6520 7468 6520  - What were the 
-00002500: 696e 7075 7420 7661 7269 6162 6c65 733f  input variables?
-00002510: 0a2d 2057 6861 7420 7761 7320 7468 6520  .- What was the 
-00002520: 7072 6f6d 7074 2074 656d 706c 6174 653f  prompt template?
-00002530: 0a2d 2057 6861 7420 6469 6420 7468 6520  .- What did the 
-00002540: 7072 6f6d 7074 206c 6f6f 6b20 6c69 6b65  prompt look like
-00002550: 3f0a 2d20 5768 6174 2077 6173 2074 6865  ?.- What was the
-00002560: 2065 7861 6374 2063 6f6e 6669 6775 7261   exact configura
-00002570: 7469 6f6e 206f 6620 7468 6520 6d6f 6465  tion of the mode
-00002580: 6c3f 0a2d 2048 6f77 206d 616e 7920 7469  l?.- How many ti
-00002590: 6d65 7320 6469 6420 7765 2072 6574 7279  mes did we retry
-000025a0: 2074 6865 2072 6571 7565 7374 3f0a 2d20   the request?.- 
-000025b0: 5768 6174 2077 6173 2074 6865 2072 6177  What was the raw
-000025c0: 2064 6174 6120 7468 6520 4150 4920 7265   data the API re
-000025d0: 7475 726e 6564 3f0a 2d20 486f 7720 6d61  turned?.- How ma
-000025e0: 6e79 2074 6f6b 656e 7320 7765 7265 2075  ny tokens were u
-000025f0: 7365 643f 0a2d 2057 6861 7420 7761 7320  sed?.- What was 
-00002600: 7468 6520 6669 6e61 6c20 7265 7375 6c74  the final result
-00002610: 3f0a 0a23 2320 4c69 6365 6e73 650a 4c4c  ?..## License.LL
-00002620: 4d46 6c6f 7773 2069 7320 636f 7665 7265  MFlows is covere
-00002630: 6420 6279 2074 6865 204d 4954 206c 6963  d by the MIT lic
-00002640: 656e 7365 2e20 466f 7220 6d6f 7265 2069  ense. For more i
-00002650: 6e66 6f72 6d61 7469 6f6e 2c20 6368 6563  nformation, chec
-00002660: 6b20 604c 4943 454e 4345 2e6d 6460 2e0a  k `LICENCE.md`..
-00002670: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
-00002680: 0a54 6861 6e6b 2079 6f75 2066 6f72 2073  .Thank you for s
-00002690: 7065 6e64 696e 6720 7469 6d65 2067 6f69  pending time goi
-000026a0: 6e67 206f 7665 7220 6f75 7220 5245 4144  ng over our READ
-000026b0: 4d45 2120 4966 2079 6f75 2066 696e 6420  ME! If you find 
-000026c0: 4c4c 4d46 6c6f 7773 2065 7863 6974 696e  LLMFlows excitin
-000026d0: 6720 616e 6420 0a79 6f75 2061 7265 2063  g and .you are c
-000026e0: 6f6e 7369 6465 7269 6e67 2063 6f6e 7472  onsidering contr
-000026f0: 6962 7574 696e 672c 2070 6c65 6173 6520  ibuting, please 
-00002700: 6368 6563 6b20 5b60 434f 4e54 5249 4255  check [`CONTRIBU
-00002710: 5449 4e47 2e6d 6460 5d28 6874 7470 733a  TING.md`](https:
-00002720: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746f  //github.com/sto
-00002730: 7961 6e2d 7374 6f79 616e 6f76 2f6c 6c6d  yan-stoyanov/llm
-00002740: 666c 6f77 732f 626c 6f62 2f6d 6169 6e2f  flows/blob/main/
-00002750: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00002760: 2e0a                                     ..
+00000000: 2320 4c4c 4d46 6c6f 7773 202d 2053 696d  # LLMFlows - Sim
+00000010: 706c 652c 2045 7870 6c69 6369 742c 2061  ple, Explicit, a
+00000020: 6e64 2054 7261 6e73 7061 7265 6e74 204c  nd Transparent L
+00000030: 4c4d 2041 7070 730a 3c62 722f 3e0a 3c62  LM Apps.<br/>.<b
+00000040: 722f 3e0a 3c62 722f 3e0a 3c70 2061 6c69  r/>.<br/>.<p ali
+00000050: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
+00000060: 696d 6720 7374 796c 653d 2277 6964 7468  img style="width
+00000070: 3a20 3830 2522 2073 7263 3d22 6874 7470  : 80%" src="http
+00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000090: 746f 7961 6e2d 7374 6f79 616e 6f76 2f6c  toyan-stoyanov/l
+000000a0: 6c6d 666c 6f77 732f 626c 6f62 2f6d 6169  lmflows/blob/mai
+000000b0: 6e2f 646f 6373 2f6c 6c6d 666c 6f77 735f  n/docs/llmflows_
+000000c0: 6c61 7374 5f6c 6f67 6f2e 706e 6722 2f3e  last_logo.png"/>
+000000d0: 0a3c 2f70 3e0a 3c62 722f 3e0a 3c62 722f  .</p>.<br/>.<br/
+000000e0: 3e0a 3c62 722f 3e0a 0a5b 215b 5477 6974  >.<br/>..[![Twit
+000000f0: 7465 725d 2868 7474 7073 3a2f 2f69 6d67  ter](https://img
+00000100: 2e73 6869 656c 6473 2e69 6f2f 7477 6974  .shields.io/twit
+00000110: 7465 722f 666f 6c6c 6f77 2f4c 4c4d 466c  ter/follow/LLMFl
+00000120: 6f77 733f 7374 796c 653d 736f 6369 616c  ows?style=social
+00000130: 295d 2868 7474 7073 3a2f 2f74 7769 7474  )](https://twitt
+00000140: 6572 2e63 6f6d 2f4c 4c4d 466c 6f77 7329  er.com/LLMFlows)
+00000150: 0a21 5b50 796c 696e 7420 776f 726b 666c  .![Pylint workfl
+00000160: 6f77 5d28 6874 7470 733a 2f2f 6769 7468  ow](https://gith
+00000170: 7562 2e63 6f6d 2f73 746f 7961 6e2d 7374  ub.com/stoyan-st
+00000180: 6f79 616e 6f76 2f6c 6c6d 666c 6f77 732f  oyanov/llmflows/
+00000190: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000001a0: 732f 7079 6c69 6e74 2e79 6d6c 2f62 6164  s/pylint.yml/bad
+000001b0: 6765 2e73 7667 290a 215b 4c69 6365 6e73  ge.svg).![Licens
+000001c0: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+000001d0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+000001e0: 2f6c 6963 656e 7365 2f73 746f 7961 6e2d  /license/stoyan-
+000001f0: 7374 6f79 616e 6f76 2f6c 6c6d 666c 6f77  stoyanov/llmflow
+00000200: 7329 0a21 5b50 7950 695d 2868 7474 7073  s).![PyPi](https
+00000210: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000220: 6f2f 7079 7069 2f76 2f6c 6c6d 666c 6f77  o/pypi/v/llmflow
+00000230: 7329 0a21 5b53 7461 7273 5d28 6874 7470  s).![Stars](http
+00000240: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000250: 696f 2f67 6974 6875 622f 7374 6172 732f  io/github/stars/
+00000260: 7374 6f79 616e 2d73 746f 7961 6e6f 762f  stoyan-stoyanov/
+00000270: 6c6c 6d66 6c6f 7773 3f73 7479 6c65 3d73  llmflows?style=s
+00000280: 6f63 6961 6c29 0a21 5b52 656c 6561 7365  ocial).![Release
+00000290: 2064 6174 655d 2868 7474 7073 3a2f 2f69   date](https://i
+000002a0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+000002b0: 7468 7562 2f72 656c 6561 7365 2d64 6174  thub/release-dat
+000002c0: 652f 7374 6f79 616e 2d73 746f 7961 6e6f  e/stoyan-stoyano
+000002d0: 762f 6c6c 6d66 6c6f 7773 3f73 7479 6c65  v/llmflows?style
+000002e0: 3d73 6f63 6961 6c29 0a0a 446f 6375 6d65  =social)..Docume
+000002f0: 6e74 6174 696f 6e3a 203c 6120 6872 6566  ntation: <a href
+00000300: 3d22 6874 7470 733a 2f2f 6c6c 6d66 6c6f  ="https://llmflo
+00000310: 7773 2e72 6561 6474 6865 646f 6373 2e69  ws.readthedocs.i
+00000320: 6f2f 2220 7461 7267 6574 3d22 5f62 6c61  o/" target="_bla
+00000330: 6e6b 223e 6874 7470 733a 2f2f 6c6c 6d66  nk">https://llmf
+00000340: 6c6f 7773 2e72 6561 6474 6865 646f 6373  lows.readthedocs
+00000350: 2e69 6f3c 2f61 3e3c 2f62 723e 0a50 7950  .io</a></br>.PyP
+00000360: 493a 203c 6120 6872 6566 3d22 6874 7470  I: <a href="http
+00000370: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000380: 6a65 6374 2f6c 6c6d 666c 6f77 732f 2220  ject/llmflows/" 
+00000390: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000003a0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000003b0: 2f70 726f 6a65 6374 2f6c 6c6d 666c 6f77  /project/llmflow
+000003c0: 733c 2f61 3e3c 2f62 723e 0a54 7769 7474  s</a></br>.Twitt
+000003d0: 6572 3a20 3c61 2068 7265 663d 2268 7474  er: <a href="htt
+000003e0: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
+000003f0: 2f4c 4c4d 466c 6f77 732f 2220 7461 7267  /LLMFlows/" targ
+00000400: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
+00000410: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00000420: 4c4c 4d46 6c6f 7773 3c2f 613e 3c2f 6272  LLMFlows</a></br
+00000430: 3e0a 5375 6273 7461 636b 3a20 3c61 2068  >.Substack: <a h
+00000440: 7265 663d 2268 7474 7073 3a2f 2f6c 6c6d  ref="https://llm
+00000450: 666c 6f77 732e 7375 6273 7461 636b 2e63  flows.substack.c
+00000460: 6f6d 2f22 2074 6172 6765 743d 225f 626c  om/" target="_bl
+00000470: 616e 6b22 3e68 7474 7073 3a2f 2f6c 6c6d  ank">https://llm
+00000480: 666c 6f77 732e 7375 6273 7461 636b 2e63  flows.substack.c
+00000490: 6f6d 3c2f 613e 3c2f 6272 3e0a 0a23 2320  om</a></br>..## 
+000004a0: 4162 6f75 740a 4c4c 4d46 6c6f 7773 2069  About.LLMFlows i
+000004b0: 7320 6120 6672 616d 6577 6f72 6b20 666f  s a framework fo
+000004c0: 7220 6275 696c 6469 6e67 2073 696d 706c  r building simpl
+000004d0: 652c 2065 7870 6c69 6369 742c 2061 6e64  e, explicit, and
+000004e0: 2074 7261 6e73 7061 7265 6e74 204c 4c4d   transparent LLM
+000004f0: 284c 6172 6765 200a 4c61 6e67 7561 6765  (Large .Language
+00000500: 204d 6f64 656c 2920 6170 706c 6963 6174   Model) applicat
+00000510: 696f 6e73 2e0a 0a23 2320 496e 7374 616c  ions...## Instal
+00000520: 6c61 7469 6f6e 0a60 6060 0a70 6970 2069  lation.```.pip i
+00000530: 6e73 7461 6c6c 206c 6c6d 666c 6f77 730a  nstall llmflows.
+00000540: 6060 600a 0a23 2320 5068 696c 6f73 6f70  ```..## Philosop
+00000550: 6879 0a0a 2323 2320 2a2a 5369 6d70 6c65  hy..### **Simple
+00000560: 2a2a 0a4f 7572 2067 6f61 6c20 6973 2074  **.Our goal is t
+00000570: 6f20 6275 696c 6420 6120 7369 6d70 6c65  o build a simple
+00000580: 2c20 7765 6c6c 2d64 6f63 756d 656e 7465  , well-documente
+00000590: 6420 6672 616d 6577 6f72 6b20 7769 7468  d framework with
+000005a0: 206d 696e 696d 616c 2061 6273 7472 6163   minimal abstrac
+000005b0: 7469 6f6e 7320 7468 6174 200a 616c 6c6f  tions that .allo
+000005c0: 7720 7573 6572 7320 746f 2062 7569 6c64  w users to build
+000005d0: 2066 6c65 7869 626c 6520 4c4c 4d2d 706f   flexible LLM-po
+000005e0: 7765 7265 6420 6170 7073 2077 6974 686f  wered apps witho
+000005f0: 7574 2063 6f6d 7072 6f6d 6973 696e 6720  ut compromising 
+00000600: 6f6e 2063 6170 6162 696c 6974 6965 732e  on capabilities.
+00000610: 0a0a 2323 2320 2a2a 4578 706c 6963 6974  ..### **Explicit
+00000620: 2a2a 0a57 6520 7761 6e74 2074 6f20 6372  **.We want to cr
+00000630: 6561 7465 2061 6e20 6578 706c 6963 6974  eate an explicit
+00000640: 2041 5049 2065 6e61 626c 696e 6720 7573   API enabling us
+00000650: 6572 7320 746f 2077 7269 7465 2063 6c65  ers to write cle
+00000660: 616e 2061 6e64 2072 6561 6461 626c 6520  an and readable 
+00000670: 636f 6465 2077 6869 6c65 200a 6561 7369  code while .easi
+00000680: 6c79 2063 7265 6174 696e 6720 636f 6d70  ly creating comp
+00000690: 6c65 7820 666c 6f77 7320 6f66 204c 4c4d  lex flows of LLM
+000006a0: 7320 696e 7465 7261 6374 696e 6720 7769  s interacting wi
+000006b0: 7468 2065 6163 6820 6f74 6865 722e 204c  th each other. L
+000006c0: 4c4d 466c 6f77 7327 2063 6c61 7373 6573  LMFlows' classes
+000006d0: 200a 6769 7665 2075 7365 7273 2066 756c   .give users ful
+000006e0: 6c20 636f 6e74 726f 6c20 616e 6420 646f  l control and do
+000006f0: 206e 6f74 2068 6176 6520 616e 7920 6869   not have any hi
+00000700: 6464 656e 2070 726f 6d70 7473 206f 7220  dden prompts or 
+00000710: 4c4c 4d20 6361 6c6c 732e 200a 0a23 2323  LLM calls. ..###
+00000720: 202a 2a54 7261 6e73 7061 7265 6e74 2a2a   **Transparent**
+00000730: 0a57 6520 6169 6d20 746f 2068 656c 7020  .We aim to help 
+00000740: 7573 6572 7320 6861 7665 2066 756c 6c20  users have full 
+00000750: 7472 616e 7370 6172 656e 6379 206f 6e20  transparency on 
+00000760: 7468 6569 7220 4c4c 4d2d 706f 7765 7265  their LLM-powere
+00000770: 6420 6170 7073 2062 7920 7072 6f76 6964  d apps by provid
+00000780: 696e 6720 0a74 7261 6365 6162 6c65 2066  ing .traceable f
+00000790: 6c6f 7773 2061 6e64 2063 6f6d 706c 6574  lows and complet
+000007a0: 6520 696e 666f 726d 6174 696f 6e20 666f  e information fo
+000007b0: 7220 6561 6368 2061 7070 2063 6f6d 706f  r each app compo
+000007c0: 6e65 6e74 2c20 6d61 6b69 6e67 2069 7420  nent, making it 
+000007d0: 6561 7379 2074 6f20 0a6d 6f6e 6974 6f72  easy to .monitor
+000007e0: 2c20 6d61 696e 7461 696e 2c20 616e 6420  , maintain, and 
+000007f0: 6465 6275 672e 0a0a 2323 2047 6574 7469  debug...## Getti
+00000800: 6e67 2053 7461 7274 6564 0a23 2323 204c  ng Started.### L
+00000810: 4c4d 730a 4c4c 4d73 2061 7265 206f 6e65  LMs.LLMs are one
+00000820: 206f 6620 7468 6520 6d61 696e 2061 6273   of the main abs
+00000830: 7472 6163 7469 6f6e 7320 696e 204c 4c4d  tractions in LLM
+00000840: 466c 6f77 732e 204c 4c4d 2063 6c61 7373  Flows. LLM class
+00000850: 6573 2061 7265 2077 7261 7070 6572 7320  es are wrappers 
+00000860: 6172 6f75 6e64 204c 4c4d 200a 4150 4973  around LLM .APIs
+00000870: 2073 7563 6820 6173 204f 7065 6e41 4927   such as OpenAI'
+00000880: 7320 4150 4973 2e20 5468 6579 2070 726f  s APIs. They pro
+00000890: 7669 6465 206d 6574 686f 6473 2066 6f72  vide methods for
+000008a0: 2063 6f6e 6669 6775 7269 6e67 2061 6e64   configuring and
+000008b0: 2063 616c 6c69 6e67 2074 6865 7365 2041   calling these A
+000008c0: 5049 732c 200a 7265 7472 7969 6e67 2066  PIs, .retrying f
+000008d0: 6169 6c65 6420 6361 6c6c 732c 2061 6e64  ailed calls, and
+000008e0: 2066 6f72 6d61 7474 696e 6720 7468 6520   formatting the 
+000008f0: 7265 7370 6f6e 7365 732e 0a0a 6060 6070  responses...```p
+00000900: 7974 686f 6e0a 6672 6f6d 206c 6c6d 666c  ython.from llmfl
+00000910: 6f77 732e 6c6c 6d73 2069 6d70 6f72 7420  ows.llms import 
+00000920: 4f70 656e 4149 0a0a 6c6c 6d20 3d20 4f70  OpenAI..llm = Op
+00000930: 656e 4149 2861 7069 5f6b 6579 3d22 3c79  enAI(api_key="<y
+00000940: 6f75 722d 6f70 656e 6169 2d61 7069 2d6b  our-openai-api-k
+00000950: 6579 3e22 290a 0a72 6573 756c 742c 2063  ey>")..result, c
+00000960: 616c 6c5f 6461 7461 2c20 6d6f 6465 6c5f  all_data, model_
+00000970: 636f 6e66 6967 203d 206c 6c6d 2e67 656e  config = llm.gen
+00000980: 6572 6174 6528 0a20 2020 7072 6f6d 7074  erate(.   prompt
+00000990: 3d22 4765 6e65 7261 7465 2061 2063 6f6f  ="Generate a coo
+000009a0: 6c20 7469 746c 6520 666f 7220 616e 2038  l title for an 8
+000009b0: 3073 2072 6f63 6b20 736f 6e67 220a 290a  0s rock song".).
+000009c0: 6060 600a 0a0a 2323 2320 5072 6f6d 7074  ```...### Prompt
+000009d0: 5465 6d70 6c61 7465 730a 5468 6520 6050  Templates.The `P
+000009e0: 726f 6d70 7454 656d 706c 6174 6560 2063  romptTemplate` c
+000009f0: 6c61 7373 2061 6c6c 6f77 7320 7573 2074  lass allows us t
+00000a00: 6f20 6372 6561 7465 2073 7472 696e 6773  o create strings
+00000a10: 2077 6974 6820 7661 7269 6162 6c65 7320   with variables 
+00000a20: 7468 6174 2077 6520 6361 6e20 6669 6c6c  that we can fill
+00000a30: 200a 696e 2064 796e 616d 6963 616c 6c79   .in dynamically
+00000a40: 206c 6174 6572 206f 6e2e 204f 6e63 6520   later on. Once 
+00000a50: 6120 7072 6f6d 7074 2074 656d 706c 6174  a prompt templat
+00000a60: 6520 6f62 6a65 6374 2069 7320 6372 6561  e object is crea
+00000a70: 7465 6420 616e 2061 6374 7561 6c20 7072  ted an actual pr
+00000a80: 6f6d 7074 2063 616e 200a 6265 2067 656e  ompt can .be gen
+00000a90: 6572 6174 6564 2062 7920 7072 6f76 6964  erated by provid
+00000aa0: 696e 6720 7468 6520 7265 7175 6972 6564  ing the required
+00000ab0: 2076 6172 6961 626c 6573 2e0a 0a60 6060   variables...```
+00000ac0: 7079 7468 6f6e 0a66 726f 6d20 6c6c 6d66  python.from llmf
+00000ad0: 6c6f 7773 2e6c 6c6d 7320 696d 706f 7274  lows.llms import
+00000ae0: 204f 7065 6e41 490a 6672 6f6d 206c 6c6d   OpenAI.from llm
+00000af0: 666c 6f77 732e 7072 6f6d 7074 7320 696d  flows.prompts im
+00000b00: 706f 7274 2050 726f 6d70 7454 656d 706c  port PromptTempl
+00000b10: 6174 650a 0a0a 7072 6f6d 7074 5f74 656d  ate...prompt_tem
+00000b20: 706c 6174 6520 3d20 5072 6f6d 7074 5465  plate = PromptTe
+00000b30: 6d70 6c61 7465 280a 2020 2020 7072 6f6d  mplate(.    prom
+00000b40: 7074 3d22 4765 6e65 7261 7465 2061 2074  pt="Generate a t
+00000b50: 6974 6c65 2066 6f72 2061 2039 3073 2068  itle for a 90s h
+00000b60: 6970 2d68 6f70 2073 6f6e 6720 6162 6f75  ip-hop song abou
+00000b70: 7420 7b74 6f70 6963 7d2e 220a 290a 6c6c  t {topic}.".).ll
+00000b80: 6d5f 7072 6f6d 7074 203d 2070 726f 6d70  m_prompt = promp
+00000b90: 745f 7465 6d70 6c61 7465 2e67 6574 5f70  t_template.get_p
+00000ba0: 726f 6d70 7428 746f 7069 633d 2266 7269  rompt(topic="fri
+00000bb0: 656e 6473 6869 7022 290a 0a70 7269 6e74  endship")..print
+00000bc0: 286c 6c6d 5f70 726f 6d70 7429 0a0a 6c6c  (llm_prompt)..ll
+00000bd0: 6d20 3d20 4f70 656e 4149 2861 7069 5f6b  m = OpenAI(api_k
+00000be0: 6579 3d22 3c79 6f75 722d 6f70 656e 6169  ey="<your-openai
+00000bf0: 2d61 7069 2d6b 6579 3e22 290a 736f 6e67  -api-key>").song
+00000c00: 5f74 6974 6c65 203d 206c 6c6d 2e67 656e  _title = llm.gen
+00000c10: 6572 6174 6528 6c6c 6d5f 7072 6f6d 7074  erate(llm_prompt
+00000c20: 290a 0a70 7269 6e74 2873 6f6e 675f 7469  )..print(song_ti
+00000c30: 746c 6529 0a60 6060 0a0a 2323 2320 4368  tle).```..### Ch
+00000c40: 6174 204c 4c4d 730a 556e 6c69 6b65 2072  at LLMs.Unlike r
+00000c50: 6567 756c 6172 204c 4c4d 7320 7468 6174  egular LLMs that
+00000c60: 206f 6e6c 7920 7265 7175 6972 6520 6120   only require a 
+00000c70: 7072 6f6d 7074 2074 6f20 6765 6e65 7261  prompt to genera
+00000c80: 7465 2074 6578 742c 2063 6861 7420 4c4c  te text, chat LL
+00000c90: 4d73 2072 6571 7569 7265 2061 200a 636f  Ms require a .co
+00000ca0: 6e76 6572 7361 7469 6f6e 2068 6973 746f  nversation histo
+00000cb0: 7279 2e20 5468 6520 636f 6e76 6572 7361  ry. The conversa
+00000cc0: 7469 6f6e 2068 6973 746f 7279 2069 7320  tion history is 
+00000cd0: 7265 7072 6573 656e 7465 6420 0a61 7320  represented .as 
+00000ce0: 6120 6c69 7374 206f 6620 6d65 7373 6167  a list of messag
+00000cf0: 6573 2062 6574 7765 656e 2061 2075 7365  es between a use
+00000d00: 7220 616e 6420 616e 2061 7373 6973 7461  r and an assista
+00000d10: 6e74 2e20 5468 6973 2063 6f6e 7665 7273  nt. This convers
+00000d20: 6174 696f 6e20 6869 7374 6f72 7920 6973  ation history is
+00000d30: 200a 7365 6e74 2074 6f20 7468 6520 6d6f   .sent to the mo
+00000d40: 6465 6c2c 2061 6e64 2061 206e 6577 206d  del, and a new m
+00000d50: 6573 7361 6765 2069 7320 6765 6e65 7261  essage is genera
+00000d60: 7465 6420 6261 7365 6420 6f6e 2069 742e  ted based on it.
+00000d70: 0a0a 4c4c 4d46 6c6f 7773 2070 726f 7669  ..LLMFlows provi
+00000d80: 6465 7320 6120 604d 6573 7361 6765 4869  des a `MessageHi
+00000d90: 7374 6f72 7960 2063 6c61 7373 2074 6f20  story` class to 
+00000da0: 6d61 6e61 6765 2074 6865 2072 6571 7569  manage the requi
+00000db0: 7265 6420 636f 6e76 6572 7361 7469 6f6e  red conversation
+00000dc0: 2068 6973 746f 7279 200a 666f 7220 6368   history .for ch
+00000dd0: 6174 204c 4c4d 732e 0a0a 596f 7520 6361  at LLMs...You ca
+00000de0: 6e20 6275 696c 6420 6120 7369 6d70 6c65  n build a simple
+00000df0: 2063 6861 7462 6f74 2062 7920 7573 696e   chatbot by usin
+00000e00: 6720 7468 6520 604f 7065 6e41 4943 6861  g the `OpenAICha
+00000e10: 7460 2061 6e64 2060 4d65 7373 6167 6548  t` and `MessageH
+00000e20: 6973 746f 7279 6020 636c 6173 7365 733a  istory` classes:
+00000e30: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000e40: 206c 6c6d 666c 6f77 732e 6c6c 6d73 2069   llmflows.llms i
+00000e50: 6d70 6f72 7420 4f70 656e 4149 4368 6174  mport OpenAIChat
+00000e60: 2c20 4d65 7373 6167 6548 6973 746f 7279  , MessageHistory
+00000e70: 0a0a 6c6c 6d20 3d20 4f70 656e 4149 4368  ..llm = OpenAICh
+00000e80: 6174 2861 7069 5f6b 6579 3d22 3c79 6f75  at(api_key="<you
+00000e90: 722d 6f70 656e 6169 2d61 7069 2d6b 6579  r-openai-api-key
+00000ea0: 3e22 290a 6d65 7373 6167 655f 6869 7374  >").message_hist
+00000eb0: 6f72 7920 3d20 4d65 7373 6167 6548 6973  ory = MessageHis
+00000ec0: 746f 7279 2829 0a0a 7768 696c 6520 5472  tory()..while Tr
+00000ed0: 7565 3a0a 2020 2020 7573 6572 5f6d 6573  ue:.    user_mes
+00000ee0: 7361 6765 203d 2069 6e70 7574 2822 596f  sage = input("Yo
+00000ef0: 753a 2229 0a20 2020 206d 6573 7361 6765  u:").    message
+00000f00: 5f68 6973 746f 7279 2e61 6464 5f75 7365  _history.add_use
+00000f10: 725f 6d65 7373 6167 6528 7573 6572 5f6d  r_message(user_m
+00000f20: 6573 7361 6765 290a 0a20 2020 206c 6c6d  essage)..    llm
+00000f30: 5f72 6573 706f 6e73 652c 2063 616c 6c5f  _response, call_
+00000f40: 6461 7461 2c20 6d6f 6465 6c5f 636f 6e66  data, model_conf
+00000f50: 6967 203d 206c 6c6d 2e67 656e 6572 6174  ig = llm.generat
+00000f60: 6528 6d65 7373 6167 655f 6869 7374 6f72  e(message_histor
+00000f70: 7929 0a20 2020 206d 6573 7361 6765 5f68  y).    message_h
+00000f80: 6973 746f 7279 2e61 6464 5f61 695f 6d65  istory.add_ai_me
+00000f90: 7373 6167 6528 6c6c 6d5f 7265 7370 6f6e  ssage(llm_respon
+00000fa0: 7365 290a 0a20 2020 2070 7269 6e74 2866  se)..    print(f
+00000fb0: 224c 4c4d 3a20 7b6c 6c6d 5f72 6573 706f  "LLM: {llm_respo
+00000fc0: 6e73 657d 2229 0a60 6060 0a0a 2323 2320  nse}").```..### 
+00000fd0: 4c4c 4d20 466c 6f77 730a 4f66 7465 6e20  LLM Flows.Often 
+00000fe0: 7469 6d65 732c 2072 6561 6c2d 776f 726c  times, real-worl
+00000ff0: 6420 6170 706c 6963 6174 696f 6e73 2063  d applications c
+00001000: 616e 2062 6520 6d6f 7265 2063 6f6d 706c  an be more compl
+00001010: 6578 2061 6e64 2063 616e 2068 6176 6520  ex and can have 
+00001020: 6465 7065 6e64 656e 6369 6573 200a 6265  dependencies .be
+00001030: 7477 6565 6e20 7072 6f6d 7074 7320 616e  tween prompts an
+00001040: 6420 4c4c 4d20 6361 6c6c 732e 2046 6f72  d LLM calls. For
+00001050: 2065 7861 6d70 6c65 3a0a 0a21 5b43 6f6d   example:..![Com
+00001060: 706c 6578 2066 6c6f 775d 2868 7474 7073  plex flow](https
+00001070: 3a2f 2f67 6974 6875 622e 636f 6d2f 7374  ://github.com/st
+00001080: 6f79 616e 2d73 746f 7961 6e6f 762f 6c6c  oyan-stoyanov/ll
+00001090: 6d66 6c6f 7773 2f62 6c6f 622f 6d61 696e  mflows/blob/main
+000010a0: 2f64 6f63 732f 636f 6d70 6c65 785f 666c  /docs/complex_fl
+000010b0: 6f77 2e70 6e67 290a 0a57 6865 6e20 796f  ow.png)..When yo
+000010c0: 7520 7761 6e74 2074 6f20 6275 696c 6420  u want to build 
+000010d0: 6170 7073 2077 6974 6820 636f 6d70 6c65  apps with comple
+000010e0: 7820 6465 7065 6e64 656e 6369 6573 2079  x dependencies y
+000010f0: 6f75 2063 616e 2075 7365 2074 6865 2060  ou can use the `
+00001100: 466c 6f77 6020 616e 6420 0a60 466c 6f77  Flow` and .`Flow
+00001110: 7374 6570 6020 636c 6173 7365 732e 204c  step` classes. L
+00001120: 4c4d 466c 6f77 7320 7769 6c6c 2066 6967  LMFlows will fig
+00001130: 7572 6520 6f75 7420 7468 6520 6465 7065  ure out the depe
+00001140: 6e64 656e 6369 6573 2061 6e64 206d 616b  ndencies and mak
+00001150: 6520 7375 7265 2065 6163 6820 0a66 6c6f  e sure each .flo
+00001160: 7773 7465 7020 7275 6e73 206f 6e6c 7920  wstep runs only 
+00001170: 7768 656e 2061 6c6c 2069 7473 2064 6570  when all its dep
+00001180: 656e 6465 6e63 6965 7320 6172 6520 6d65  endencies are me
+00001190: 743a 0a0a 6060 6070 7974 686f 6e0a 6672  t:..```python.fr
+000011a0: 6f6d 206c 6c6d 666c 6f77 732e 666c 6f77  om llmflows.flow
+000011b0: 7320 696d 706f 7274 2046 6c6f 772c 2046  s import Flow, F
+000011c0: 6c6f 7753 7465 700a 6672 6f6d 206c 6c6d  lowStep.from llm
+000011d0: 666c 6f77 732e 6c6c 6d73 2069 6d70 6f72  flows.llms impor
+000011e0: 7420 4f70 656e 4149 0a66 726f 6d20 6c6c  t OpenAI.from ll
+000011f0: 6d66 6c6f 7773 2e70 726f 6d70 7473 2069  mflows.prompts i
+00001200: 6d70 6f72 7420 5072 6f6d 7074 5465 6d70  mport PromptTemp
+00001210: 6c61 7465 0a0a 6f70 656e 6169 5f6c 6c6d  late..openai_llm
+00001220: 203d 204f 7065 6e41 4928 6170 695f 6b65   = OpenAI(api_ke
+00001230: 793d 223c 796f 7572 2d6f 7065 6e61 692d  y="<your-openai-
+00001240: 6170 692d 6b65 793e 2229 0a0a 2320 4372  api-key>")..# Cr
+00001250: 6561 7465 2070 726f 6d70 7420 7465 6d70  eate prompt temp
+00001260: 6c61 7465 730a 7469 746c 655f 7465 6d70  lates.title_temp
+00001270: 6c61 7465 203d 2050 726f 6d70 7454 656d  late = PromptTem
+00001280: 706c 6174 6528 2257 6861 7420 6973 2061  plate("What is a
+00001290: 2067 6f6f 6420 7469 746c 6520 6f66 2061   good title of a
+000012a0: 206d 6f76 6965 2061 626f 7574 207b 746f   movie about {to
+000012b0: 7069 637d 3f22 290a 736f 6e67 5f74 656d  pic}?").song_tem
+000012c0: 706c 6174 6520 3d20 5072 6f6d 7074 5465  plate = PromptTe
+000012d0: 6d70 6c61 7465 280a 2020 2020 2257 6861  mplate(.    "Wha
+000012e0: 7420 6973 2061 2067 6f6f 6420 736f 6e67  t is a good song
+000012f0: 2074 6974 6c65 206f 6620 6120 736f 756e   title of a soun
+00001300: 6474 7261 636b 2066 6f72 2061 206d 6f76  dtrack for a mov
+00001310: 6965 2063 616c 6c65 6420 7b6d 6f76 6965  ie called {movie
+00001320: 5f74 6974 6c65 7d3f 220a 290a 6368 6172  _title}?".).char
+00001330: 6163 7465 7273 5f74 656d 706c 6174 6520  acters_template 
+00001340: 3d20 5072 6f6d 7074 5465 6d70 6c61 7465  = PromptTemplate
+00001350: 280a 2020 2020 2257 6861 7420 6172 6520  (.    "What are 
+00001360: 7477 6f20 6d61 696e 2063 6861 7261 6374  two main charact
+00001370: 6572 7320 666f 7220 6120 6d6f 7669 6520  ers for a movie 
+00001380: 6361 6c6c 6564 207b 6d6f 7669 655f 7469  called {movie_ti
+00001390: 746c 657d 3f22 0a29 0a6c 7972 6963 735f  tle}?".).lyrics_
+000013a0: 7465 6d70 6c61 7465 203d 2050 726f 6d70  template = Promp
+000013b0: 7454 656d 706c 6174 6528 0a20 2020 2022  tTemplate(.    "
+000013c0: 5772 6974 6520 6c79 7269 6373 206f 6620  Write lyrics of 
+000013d0: 6120 6d6f 7669 6520 736f 6e67 2063 616c  a movie song cal
+000013e0: 6c65 6420 7b73 6f6e 675f 7469 746c 657d  led {song_title}
+000013f0: 2e20 5468 6520 6d61 696e 2063 6861 7261  . The main chara
+00001400: 6374 6572 7320 6172 6520 220a 2020 2020  cters are ".    
+00001410: 227b 6d61 696e 5f63 6861 7261 6374 6572  "{main_character
+00001420: 737d 220a 290a 0a23 2043 7265 6174 6520  s}".)..# Create 
+00001430: 666c 6f77 7374 6570 730a 6d6f 7669 655f  flowsteps.movie_
+00001440: 7469 746c 655f 666c 6f77 7374 6570 203d  title_flowstep =
+00001450: 2046 6c6f 7753 7465 7028 0a20 2020 206e   FlowStep(.    n
+00001460: 616d 653d 224d 6f76 6965 2054 6974 6c65  ame="Movie Title
+00001470: 2046 6c6f 7773 7465 7022 2c0a 2020 2020   Flowstep",.    
+00001480: 6c6c 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a  llm=openai_llm,.
+00001490: 2020 2020 7072 6f6d 7074 5f74 656d 706c      prompt_templ
+000014a0: 6174 653d 7469 746c 655f 7465 6d70 6c61  ate=title_templa
+000014b0: 7465 2c0a 2020 2020 6f75 7470 7574 5f6b  te,.    output_k
+000014c0: 6579 3d22 6d6f 7669 655f 7469 746c 6522  ey="movie_title"
+000014d0: 2c0a 290a 0a73 6f6e 675f 7469 746c 655f  ,.)..song_title_
+000014e0: 666c 6f77 7374 6570 203d 2046 6c6f 7753  flowstep = FlowS
+000014f0: 7465 7028 0a20 2020 206e 616d 653d 2253  tep(.    name="S
+00001500: 6f6e 6720 5469 746c 6520 466c 6f77 7374  ong Title Flowst
+00001510: 6570 222c 0a20 2020 206c 6c6d 3d6f 7065  ep",.    llm=ope
+00001520: 6e61 695f 6c6c 6d2c 0a20 2020 2070 726f  nai_llm,.    pro
+00001530: 6d70 745f 7465 6d70 6c61 7465 3d73 6f6e  mpt_template=son
+00001540: 675f 7465 6d70 6c61 7465 2c0a 2020 2020  g_template,.    
+00001550: 6f75 7470 7574 5f6b 6579 3d22 736f 6e67  output_key="song
+00001560: 5f74 6974 6c65 222c 0a29 0a0a 6368 6172  _title",.)..char
+00001570: 6163 7465 7273 5f66 6c6f 7773 7465 7020  acters_flowstep 
+00001580: 3d20 466c 6f77 5374 6570 280a 2020 2020  = FlowStep(.    
+00001590: 6e61 6d65 3d22 4368 6172 6163 7465 7273  name="Characters
+000015a0: 2046 6c6f 7773 7465 7022 2c0a 2020 2020   Flowstep",.    
+000015b0: 6c6c 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a  llm=openai_llm,.
+000015c0: 2020 2020 7072 6f6d 7074 5f74 656d 706c      prompt_templ
+000015d0: 6174 653d 6368 6172 6163 7465 7273 5f74  ate=characters_t
+000015e0: 656d 706c 6174 652c 0a20 2020 206f 7574  emplate,.    out
+000015f0: 7075 745f 6b65 793d 226d 6169 6e5f 6368  put_key="main_ch
+00001600: 6172 6163 7465 7273 222c 0a29 0a0a 736f  aracters",.)..so
+00001610: 6e67 5f6c 7972 6963 735f 666c 6f77 7374  ng_lyrics_flowst
+00001620: 6570 203d 2046 6c6f 7753 7465 7028 0a20  ep = FlowStep(. 
+00001630: 2020 206e 616d 653d 2253 6f6e 6720 4c79     name="Song Ly
+00001640: 7269 6373 2046 6c6f 7773 7465 7022 2c0a  rics Flowstep",.
+00001650: 2020 2020 6c6c 6d3d 6f70 656e 6169 5f6c      llm=openai_l
+00001660: 6c6d 2c0a 2020 2020 7072 6f6d 7074 5f74  lm,.    prompt_t
+00001670: 656d 706c 6174 653d 6c79 7269 6373 5f74  emplate=lyrics_t
+00001680: 656d 706c 6174 652c 0a20 2020 206f 7574  emplate,.    out
+00001690: 7075 745f 6b65 793d 2273 6f6e 675f 6c79  put_key="song_ly
+000016a0: 7269 6373 222c 0a29 0a0a 2320 436f 6e6e  rics",.)..# Conn
+000016b0: 6563 7420 666c 6f77 7374 6570 730a 6d6f  ect flowsteps.mo
+000016c0: 7669 655f 7469 746c 655f 666c 6f77 7374  vie_title_flowst
+000016d0: 6570 2e63 6f6e 6e65 6374 2873 6f6e 675f  ep.connect(song_
+000016e0: 7469 746c 655f 666c 6f77 7374 6570 2c20  title_flowstep, 
+000016f0: 6368 6172 6163 7465 7273 5f66 6c6f 7773  characters_flows
+00001700: 7465 702c 2073 6f6e 675f 6c79 7269 6373  tep, song_lyrics
+00001710: 5f66 6c6f 7773 7465 7029 0a73 6f6e 675f  _flowstep).song_
+00001720: 7469 746c 655f 666c 6f77 7374 6570 2e63  title_flowstep.c
+00001730: 6f6e 6e65 6374 2873 6f6e 675f 6c79 7269  onnect(song_lyri
+00001740: 6373 5f66 6c6f 7773 7465 7029 0a63 6861  cs_flowstep).cha
+00001750: 7261 6374 6572 735f 666c 6f77 7374 6570  racters_flowstep
+00001760: 2e63 6f6e 6e65 6374 2873 6f6e 675f 6c79  .connect(song_ly
+00001770: 7269 6373 5f66 6c6f 7773 7465 7029 0a0a  rics_flowstep)..
+00001780: 2320 4372 6561 7465 2061 6e64 2072 756e  # Create and run
+00001790: 2046 6c6f 770a 736f 756e 6474 7261 636b   Flow.soundtrack
+000017a0: 5f66 6c6f 7720 3d20 466c 6f77 2874 6974  _flow = Flow(tit
+000017b0: 6c65 5f66 6c6f 7773 7465 7029 0a72 6573  le_flowstep).res
+000017c0: 756c 7473 203d 2073 6f75 6e64 7472 6163  ults = soundtrac
+000017d0: 6b5f 666c 6f77 2e73 7461 7274 2874 6f70  k_flow.start(top
+000017e0: 6963 3d22 6672 6965 6e64 7368 6970 222c  ic="friendship",
+000017f0: 2076 6572 626f 7365 3d54 7275 6529 0a60   verbose=True).`
+00001800: 6060 0a0a 2323 2320 4173 796e 6320 466c  ``..### Async Fl
+00001810: 6f77 730a 536f 6d65 7469 6d65 7320 6d75  ows.Sometimes mu
+00001820: 6c74 6970 6c65 2066 6c6f 7720 7374 6570  ltiple flow step
+00001830: 7320 6361 6e20 7275 6e20 696e 2070 6172  s can run in par
+00001840: 616c 6c65 6c20 6966 2061 6c6c 2074 6865  allel if all the
+00001850: 6972 2064 6570 656e 6465 6e63 6965 7320  ir dependencies 
+00001860: 6172 6520 6d65 742e 200a 466f 7220 6361  are met. .For ca
+00001870: 7365 7320 6c69 6b65 2074 6869 732c 204c  ses like this, L
+00001880: 4c4d 466c 6f77 7320 7072 6f76 6964 6573  LMFlows provides
+00001890: 2061 7379 6e63 2063 6c61 7373 6573 2074   async classes t
+000018a0: 6f20 696d 7072 6f76 6520 7468 6520 7275  o improve the ru
+000018b0: 6e74 696d 6520 6f66 2061 6e79 200a 636f  ntime of any .co
+000018c0: 6d70 6c65 7820 666c 6f77 2062 7920 7275  mplex flow by ru
+000018d0: 6e6e 696e 6720 666c 6f77 2073 7465 7073  nning flow steps
+000018e0: 2074 6861 7420 616c 7265 6164 7920 6861   that already ha
+000018f0: 7665 2061 6c6c 2074 6865 6972 2072 6571  ve all their req
+00001900: 7569 7265 6420 696e 7075 7473 2069 6e20  uired inputs in 
+00001910: 0a70 6172 616c 6c65 6c2e 0a0a 6060 6070  .parallel...```p
+00001920: 7974 686f 6e0a 0a2e 2e2e 0a0a 6d6f 7669  ython.......movi
+00001930: 655f 7469 746c 655f 666c 6f77 7374 6570  e_title_flowstep
+00001940: 203d 2041 7379 6e63 466c 6f77 5374 6570   = AsyncFlowStep
+00001950: 280a 2020 2020 6e61 6d65 3d22 466c 6f77  (.    name="Flow
+00001960: 7374 6570 2031 222c 0a20 2020 206c 6c6d  step 1",.    llm
+00001970: 3d6f 7065 6e61 695f 6c6c 6d2c 0a20 2020  =openai_llm,.   
+00001980: 2070 726f 6d70 745f 7465 6d70 6c61 7465   prompt_template
+00001990: 3d74 6974 6c65 5f74 656d 706c 6174 652c  =title_template,
+000019a0: 0a20 2020 206f 7574 7075 745f 6b65 793d  .    output_key=
+000019b0: 226d 6f76 6965 5f74 6974 6c65 222c 0a29  "movie_title",.)
+000019c0: 0a0a 736f 6e67 5f74 6974 6c65 5f66 6c6f  ..song_title_flo
+000019d0: 7773 7465 7020 3d20 466c 6f77 5374 6570  wstep = FlowStep
+000019e0: 280a 2020 2020 6e61 6d65 3d22 466c 6f77  (.    name="Flow
+000019f0: 7374 6570 2032 222c 0a20 2020 206c 6c6d  step 2",.    llm
+00001a00: 3d6f 7065 6e61 695f 6c6c 6d2c 0a20 2020  =openai_llm,.   
+00001a10: 2070 726f 6d70 745f 7465 6d70 6c61 7465   prompt_template
+00001a20: 3d73 6f6e 675f 7465 6d70 6c61 7465 2c0a  =song_template,.
+00001a30: 2020 2020 6f75 7470 7574 5f6b 6579 3d22      output_key="
+00001a40: 736f 6e67 5f74 6974 6c65 222c 0a29 0a0a  song_title",.)..
+00001a50: 6368 6172 6163 7465 7273 5f66 6c6f 7773  characters_flows
+00001a60: 7465 7020 3d20 4173 796e 6346 6c6f 7753  tep = AsyncFlowS
+00001a70: 7465 7028 0a20 2020 206e 616d 653d 2246  tep(.    name="F
+00001a80: 6c6f 7773 7465 7020 3322 2c0a 2020 2020  lowstep 3",.    
+00001a90: 6c6c 6d3d 6f70 656e 6169 5f6c 6c6d 2c0a  llm=openai_llm,.
+00001aa0: 2020 2020 7072 6f6d 7074 5f74 656d 706c      prompt_templ
+00001ab0: 6174 653d 6368 6172 6163 7465 7273 5f74  ate=characters_t
+00001ac0: 656d 706c 6174 652c 0a20 2020 206f 7574  emplate,.    out
+00001ad0: 7075 745f 6b65 793d 226d 6169 6e5f 6368  put_key="main_ch
+00001ae0: 6172 6163 7465 7273 222c 0a29 0a0a 736f  aracters",.)..so
+00001af0: 6e67 5f6c 7972 6963 735f 666c 6f77 7374  ng_lyrics_flowst
+00001b00: 6570 203d 2041 7379 6e63 466c 6f77 5374  ep = AsyncFlowSt
+00001b10: 6570 280a 2020 2020 6e61 6d65 3d22 466c  ep(.    name="Fl
+00001b20: 6f77 7374 6570 2034 222c 0a20 2020 206c  owstep 4",.    l
+00001b30: 6c6d 3d6f 7065 6e61 695f 6c6c 6d2c 0a20  lm=openai_llm,. 
+00001b40: 2020 2070 726f 6d70 745f 7465 6d70 6c61     prompt_templa
+00001b50: 7465 3d6c 7972 6963 735f 7465 6d70 6c61  te=lyrics_templa
+00001b60: 7465 2c0a 2020 2020 6f75 7470 7574 5f6b  te,.    output_k
+00001b70: 6579 3d22 736f 6e67 5f6c 7972 6963 7322  ey="song_lyrics"
+00001b80: 2c0a 290a 0a2e 2e2e 0a0a 6060 600a 0a43  ,.).......```..C
+00001b90: 6865 636b 206f 7572 2064 6f63 756d 656e  heck our documen
+00001ba0: 7461 7469 6f6e 2066 6f72 206d 6f72 6520  tation for more 
+00001bb0: 6578 616d 706c 6573 2c20 7375 6368 2061  examples, such a
+00001bc0: 7320 696e 7465 6772 6174 696e 6720 7665  s integrating ve
+00001bd0: 6374 6f72 2064 6174 6162 6173 6573 2c20  ctor databases, 
+00001be0: 0a63 7265 6174 696e 6720 7175 6573 7469  .creating questi
+00001bf0: 6f6e 2d61 6e73 7765 7269 6e67 2061 7070  on-answering app
+00001c00: 7320 616e 6420 7765 6220 6170 706c 6963  s and web applic
+00001c10: 6174 696f 6e73 2077 6974 6820 466c 6173  ations with Flas
+00001c20: 6b20 616e 6420 4661 7374 4150 492e 0a0a  k and FastAPI...
+00001c30: 2323 2046 6561 7475 7265 730a 0a23 2323  ## Features..###
+00001c40: 202a 2a4c 4c4d 732a 2a0a 2d20 5574 696c   **LLMs**.- Util
+00001c50: 697a 6520 4c4c 4d73 2073 7563 6820 6173  ize LLMs such as
+00001c60: 204f 7065 6e41 4927 7320 4368 6174 4750   OpenAI's ChatGP
+00001c70: 5420 746f 2067 656e 6572 6174 6520 6e61  T to generate na
+00001c80: 7475 7261 6c20 6c61 6e67 7561 6765 2074  tural language t
+00001c90: 6578 742e 0a2d 2043 6f6e 6669 6775 7265  ext..- Configure
+00001ca0: 204c 4c4d 2063 6c61 7373 6573 2065 6173   LLM classes eas
+00001cb0: 696c 792c 2063 686f 6f73 696e 6720 7370  ily, choosing sp
+00001cc0: 6563 6966 6963 206d 6f64 656c 732c 2070  ecific models, p
+00001cd0: 6172 616d 6574 6572 732c 2061 6e64 2073  arameters, and s
+00001ce0: 6574 7469 6e67 732e 0a2d 2042 656e 6566  ettings..- Benef
+00001cf0: 6974 2066 726f 6d20 6175 746f 6d61 7469  it from automati
+00001d00: 6320 7265 7472 6965 7320 7768 656e 206d  c retries when m
+00001d10: 6f64 656c 2063 616c 6c73 2066 6169 6c2c  odel calls fail,
+00001d20: 2065 6e73 7572 696e 6720 7265 6c69 6162   ensuring reliab
+00001d30: 6c65 204c 4c4d 200a 2020 696e 7465 7261  le LLM .  intera
+00001d40: 6374 696f 6e73 2e0a 0a23 2323 202a 2a50  ctions...### **P
+00001d50: 726f 6d70 7420 5465 6d70 6c61 7465 732a  rompt Templates*
+00001d60: 2a0a 2d20 4372 6561 7465 2064 796e 616d  *.- Create dynam
+00001d70: 6963 2070 726f 6d70 7473 2075 7369 6e67  ic prompts using
+00001d80: 2050 726f 6d70 7420 5465 6d70 6c61 7465   Prompt Template
+00001d90: 732c 2070 726f 7669 6469 6e67 2066 6c65  s, providing fle
+00001da0: 7869 626c 6520 616e 6420 6375 7374 6f6d  xible and custom
+00001db0: 697a 6162 6c65 200a 2020 7465 7874 2067  izable .  text g
+00001dc0: 656e 6572 6174 696f 6e2e 0a2d 2044 6566  eneration..- Def
+00001dd0: 696e 6520 7661 7269 6162 6c65 7320 7769  ine variables wi
+00001de0: 7468 696e 2070 726f 6d70 7473 2074 6f20  thin prompts to 
+00001df0: 6765 6e65 7261 7465 2070 726f 6d70 7420  generate prompt 
+00001e00: 7374 7269 6e67 7320 7461 696c 6f72 6564  strings tailored
+00001e10: 2074 6f20 7370 6563 6966 6963 200a 2020   to specific .  
+00001e20: 696e 7075 7473 2e0a 0a23 2323 202a 2a46  inputs...### **F
+00001e30: 6c6f 7773 2061 6e64 2046 6c6f 7753 7465  lows and FlowSte
+00001e40: 7073 2a2a 0a2d 2053 7472 7563 7475 7265  ps**.- Structure
+00001e50: 204c 4c4d 2061 7070 6c69 6361 7469 6f6e   LLM application
+00001e60: 7320 7573 696e 6720 466c 6f77 7320 616e  s using Flows an
+00001e70: 6420 466c 6f77 5374 6570 732c 2070 726f  d FlowSteps, pro
+00001e80: 7669 6469 6e67 2061 2063 6c65 6172 2061  viding a clear a
+00001e90: 6e64 206f 7267 616e 697a 6564 2066 7261  nd organized fra
+00001ea0: 6d65 776f 726b 2066 6f72 2065 7865 6375  mework for execu
+00001eb0: 7469 6e67 204c 4c4d 2069 6e74 6572 6163  ting LLM interac
+00001ec0: 7469 6f6e 732e 0a2d 2043 6f6e 6e65 6374  tions..- Connect
+00001ed0: 2066 6c6f 7720 7374 6570 7320 746f 2070   flow steps to p
+00001ee0: 6173 7320 6f75 7470 7574 7320 6173 2069  ass outputs as i
+00001ef0: 6e70 7574 732c 2066 6163 696c 6974 6174  nputs, facilitat
+00001f00: 696e 6720 7365 616d 6c65 7373 2064 6174  ing seamless dat
+00001f10: 6120 666c 6f77 2061 6e64 0a20 2020 206d  a flow and.    m
+00001f20: 6169 6e74 6169 6e69 6e67 2061 2074 7261  aintaining a tra
+00001f30: 6e73 7061 7265 6e74 204c 4c4d 2070 6970  nsparent LLM pip
+00001f40: 656c 696e 652e 0a2d 204c 6576 6572 6167  eline..- Leverag
+00001f50: 6520 4173 796e 6320 466c 6f77 7320 746f  e Async Flows to
+00001f60: 2072 756e 204c 4c4d 7320 696e 2070 6172   run LLMs in par
+00001f70: 616c 6c65 6c20 7768 656e 2061 6c6c 2074  allel when all t
+00001f80: 6865 6972 2069 6e70 7574 7320 6172 6520  heir inputs are 
+00001f90: 6176 6169 6c61 626c 652c 200a 2020 6f70  available, .  op
+00001fa0: 7469 6d69 7a69 6e67 2070 6572 666f 726d  timizing perform
+00001fb0: 616e 6365 2061 6e64 2065 6666 6963 6965  ance and efficie
+00001fc0: 6e63 792e 0a2d 2049 6e63 6f72 706f 7261  ncy..- Incorpora
+00001fd0: 7465 2063 7573 746f 6d20 7374 7269 6e67  te custom string
+00001fe0: 206d 616e 6970 756c 6174 696f 6e20 6675   manipulation fu
+00001ff0: 6e63 7469 6f6e 7320 6469 7265 6374 6c79  nctions directly
+00002000: 2069 6e74 6f20 666c 6f77 732c 2061 6c6c   into flows, all
+00002010: 6f77 696e 6720 0a20 2073 7065 6369 616c  owing .  special
+00002020: 697a 6564 2074 6578 7420 7472 616e 7366  ized text transf
+00002030: 6f72 6d61 7469 6f6e 7320 7769 7468 6f75  ormations withou
+00002040: 7420 7265 6c79 696e 6720 736f 6c65 6c79  t relying solely
+00002050: 206f 6e20 4c4c 4d20 6361 6c6c 732e 0a0a   on LLM calls...
+00002060: 2323 2320 2a2a 5665 6374 6f72 5374 6f72  ### **VectorStor
+00002070: 6520 496e 7465 6772 6174 696f 6e73 2a2a  e Integrations**
+00002080: 0a2d 2049 6e74 6567 7261 7465 2077 6974  .- Integrate wit
+00002090: 6820 7665 6374 6f72 2064 6174 6162 6173  h vector databas
+000020a0: 6573 206c 696b 6520 5069 6e65 636f 6e65  es like Pinecone
+000020b0: 2075 7369 6e67 2074 6865 2056 6563 746f   using the Vecto
+000020c0: 7253 746f 7265 466c 6f77 5374 6570 2c20  rStoreFlowStep, 
+000020d0: 0a20 2065 6d70 6f77 6572 696e 6720 6566  .  empowering ef
+000020e0: 6669 6369 656e 7420 616e 6420 7363 616c  ficient and scal
+000020f0: 6162 6c65 2073 746f 7261 6765 2061 6e64  able storage and
+00002100: 2072 6574 7269 6576 616c 206f 6620 7665   retrieval of ve
+00002110: 6374 6f72 2065 6d62 6564 6469 6e67 732e  ctor embeddings.
+00002120: 0a2d 204c 6576 6572 6167 6520 7665 6374  .- Leverage vect
+00002130: 6f72 2064 6174 6162 6173 6573 2066 6f72  or databases for
+00002140: 2073 6561 6d6c 6573 7320 7374 6f72 6167   seamless storag
+00002150: 6520 616e 6420 7175 6572 7969 6e67 206f  e and querying o
+00002160: 6620 7665 6374 6f72 732c 2065 6e61 626c  f vectors, enabl
+00002170: 696e 6720 7374 7261 6967 6874 666f 7277  ing straightforw
+00002180: 6172 6420 696e 7465 6772 6174 696f 6e20  ard integration 
+00002190: 7769 7468 204c 4c4d 2d70 6f77 6572 6564  with LLM-powered
+000021a0: 2061 7070 6c69 6361 7469 6f6e 732e 0a0a   applications...
+000021b0: 2323 2320 2a2a 4361 6c6c 6261 636b 732a  ### **Callbacks*
+000021c0: 2a0a 2d20 4578 6563 7574 6520 6361 6c6c  *.- Execute call
+000021d0: 6261 636b 2066 756e 6374 696f 6e73 2061  back functions a
+000021e0: 7420 6469 6666 6572 656e 7420 7374 6167  t different stag
+000021f0: 6573 2077 6974 6869 6e20 666c 6f77 2073  es within flow s
+00002200: 7465 7073 2c20 656e 6162 6c69 6e67 2065  teps, enabling e
+00002210: 6e68 616e 6365 6420 6375 7374 6f6d 697a  nhanced customiz
+00002220: 6174 696f 6e2c 206c 6f67 6769 6e67 2c20  ation, logging, 
+00002230: 7472 6163 696e 672c 206f 7220 6f74 6865  tracing, or othe
+00002240: 7220 7370 6563 6966 6963 2069 6e74 6567  r specific integ
+00002250: 7261 7469 6f6e 732e 0a2d 2055 7469 6c69  rations..- Utili
+00002260: 7a65 2063 616c 6c62 6163 6b73 2074 6f20  ze callbacks to 
+00002270: 636f 6d70 7265 6865 6e73 6976 656c 7920  comprehensively 
+00002280: 636f 6e74 726f 6c20 616e 6420 6d6f 6e69  control and moni
+00002290: 746f 7220 4c4c 4d2d 706f 7765 7265 6420  tor LLM-powered 
+000022a0: 6170 7073 2c20 656e 7375 7269 6e67 200a  apps, ensuring .
+000022b0: 2020 636c 6561 7220 7669 7369 6269 6c69    clear visibili
+000022c0: 7479 2069 6e74 6f20 7468 6520 6578 6563  ty into the exec
+000022d0: 7574 696f 6e20 7072 6f63 6573 732e 0a0a  ution process...
+000022e0: 2323 2320 2a2a 4578 706c 6963 6974 2041  ### **Explicit A
+000022f0: 5049 2061 6e64 2046 756c 6c20 5472 616e  PI and Full Tran
+00002300: 7370 6172 656e 6379 2a2a 0a57 6974 6820  sparency**.With 
+00002310: 4c4c 4d46 6c6f 7773 2079 6f75 2068 6176  LLMFlows you hav
+00002320: 6520 7468 6520 6675 6c6c 2063 6f6e 7472  e the full contr
+00002330: 6f6c 2074 6f20 6372 6561 7465 2065 7870  ol to create exp
+00002340: 6c69 6369 7420 6170 706c 6963 6174 696f  licit applicatio
+00002350: 6e73 2077 6974 686f 7574 2061 6e79 2068  ns without any h
+00002360: 6964 6465 6e20 7072 6f6d 7074 7320 6f72  idden prompts or
+00002370: 2070 7265 6465 6669 6e65 6420 6265 6861   predefined beha
+00002380: 7669 6f72 732e 0a0a 496e 2061 6464 6974  viors...In addit
+00002390: 696f 6e20 4c4c 4d46 6c6f 7773 2061 6c6c  ion LLMFlows all
+000023a0: 6f77 7320 796f 7520 746f 2061 6e73 7765  ows you to answe
+000023b0: 7220 7175 6573 7469 6f6e 7320 7375 6368  r questions such
+000023c0: 2061 733a 0a0a 2d20 5768 656e 2077 6173   as:..- When was
+000023d0: 2061 2070 6172 7469 6375 6c61 7220 666c   a particular fl
+000023e0: 6f77 7374 6570 2072 756e 3f0a 2d20 486f  owstep run?.- Ho
+000023f0: 7720 6d75 6368 2074 696d 6520 6469 6420  w much time did 
+00002400: 6974 2074 616b 653f 0a2d 2057 6861 7420  it take?.- What 
+00002410: 7765 7265 2074 6865 2069 6e70 7574 2076  were the input v
+00002420: 6172 6961 626c 6573 3f0a 2d20 5768 6174  ariables?.- What
+00002430: 2077 6173 2074 6865 2070 726f 6d70 7420   was the prompt 
+00002440: 7465 6d70 6c61 7465 3f0a 2d20 5768 6174  template?.- What
+00002450: 2064 6964 2074 6865 2070 726f 6d70 7420   did the prompt 
+00002460: 6c6f 6f6b 206c 696b 653f 0a2d 2057 6861  look like?.- Wha
+00002470: 7420 7761 7320 7468 6520 6578 6163 7420  t was the exact 
+00002480: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
+00002490: 2074 6865 206d 6f64 656c 3f0a 2d20 486f   the model?.- Ho
+000024a0: 7720 6d61 6e79 2074 696d 6573 2064 6964  w many times did
+000024b0: 2077 6520 7265 7472 7920 7468 6520 7265   we retry the re
+000024c0: 7175 6573 743f 0a2d 2057 6861 7420 7761  quest?.- What wa
+000024d0: 7320 7468 6520 7261 7720 6461 7461 2074  s the raw data t
+000024e0: 6865 2041 5049 2072 6574 7572 6e65 643f  he API returned?
+000024f0: 0a2d 2048 6f77 206d 616e 7920 746f 6b65  .- How many toke
+00002500: 6e73 2077 6572 6520 7573 6564 3f0a 2d20  ns were used?.- 
+00002510: 5768 6174 2077 6173 2074 6865 2066 696e  What was the fin
+00002520: 616c 2072 6573 756c 743f 0a0a 2323 204c  al result?..## L
+00002530: 6963 656e 7365 0a4c 4c4d 466c 6f77 7320  icense.LLMFlows 
+00002540: 6973 2063 6f76 6572 6564 2062 7920 7468  is covered by th
+00002550: 6520 4d49 5420 6c69 6365 6e73 652e 2046  e MIT license. F
+00002560: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00002570: 696f 6e2c 2063 6865 636b 2060 4c49 4345  ion, check `LICE
+00002580: 4e43 452e 6d64 602e 0a0a 2323 2043 6f6e  NCE.md`...## Con
+00002590: 7472 6962 7574 696e 670a 5468 616e 6b20  tributing.Thank 
+000025a0: 796f 7520 666f 7220 7370 656e 6469 6e67  you for spending
+000025b0: 2074 696d 6520 676f 696e 6720 6f76 6572   time going over
+000025c0: 206f 7572 2052 4541 444d 4521 2049 6620   our README! If 
+000025d0: 796f 7520 6669 6e64 204c 4c4d 466c 6f77  you find LLMFlow
+000025e0: 7320 6578 6369 7469 6e67 2061 6e64 200a  s exciting and .
+000025f0: 796f 7520 6172 6520 636f 6e73 6964 6572  you are consider
+00002600: 696e 6720 636f 6e74 7269 6275 7469 6e67  ing contributing
+00002610: 2c20 706c 6561 7365 2063 6865 636b 205b  , please check [
+00002620: 6043 4f4e 5452 4942 5554 494e 472e 6d64  `CONTRIBUTING.md
+00002630: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+00002640: 622e 636f 6d2f 7374 6f79 616e 2d73 746f  b.com/stoyan-sto
+00002650: 7961 6e6f 762f 6c6c 6d66 6c6f 7773 2f62  yanov/llmflows/b
+00002660: 6c6f 622f 6d61 696e 2f43 4f4e 5452 4942  lob/main/CONTRIB
+00002670: 5554 494e 472e 6d64 292e 0a              UTING.md)..
```

### Comparing `llmflows-0.0.8/llmflows.egg-info/SOURCES.txt` & `llmflows-0.0.9/llmflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.8/pyproject.toml` & `llmflows-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
 description = "LLMFlows - Simple, Explicit and Transparent LLM Apps"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

