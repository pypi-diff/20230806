# Comparing `tmp/langport-0.3.2.tar.gz` & `tmp/langport-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.3.2.tar", last modified: Wed Jul 19 09:19:59 2023, max compression
+gzip compressed data, was "langport-0.3.3.tar", last modified: Sun Aug  6 16:13:55 2023, max compression
```

## Comparing `langport-0.3.2.tar` & `langport-0.3.3.tar`

### file list

```diff
@@ -1,157 +1,159 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.2/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5999 2023-07-19 09:19:59.248772 langport-0.3.2/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5499 2023-07-19 09:19:34.000000 langport-0.3.2/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.2/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.3.2/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.2/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.2/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.2/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.3.2/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.2/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.2/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     8139 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-07-14 07:42:48.000000 langport-0.3.2/langport/data/conversation/settings/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      274 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/settings/firefly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      354 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/settings/internlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-07-19 09:19:34.000000 langport-0.3.2/langport/data/conversation/settings/llama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/mpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      286 2023-07-14 07:42:48.000000 langport-0.3.2/langport/data/conversation/settings/ningyu.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-07-14 07:42:48.000000 langport-0.3.2/langport/data/conversation/settings/wizardlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.2/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.2/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.2/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/baichuan.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/changgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/codegen.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/adapters/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      761 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/firefly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/internlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1528 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/llama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/longchat.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      840 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/ningyu.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/robin.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      635 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/snoozy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/starcoder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/text2vec.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      651 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/adapters/tigerbot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/adapters/wizardlm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    14471 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1756 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.244772 langport-0.3.2/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5837 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.2/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5276 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/executor/generation/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    20892 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-07-14 07:42:48.000000 langport-0.3.2/langport/model/executor/generation/optimum.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2358 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     8620 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1584 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/executor/optimum.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-30 05:32:15.000000 langport-0.3.2/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1461 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.2/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.2/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.2/langport/model/monkey_patch_non_inplace.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2973 2023-07-19 09:19:34.000000 langport-0.3.2/langport/model/svd.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.2/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.2/langport/protocol/huggingface_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4665 2023-07-14 07:42:48.000000 langport-0.3.2/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.2/langport/protocol/tabby_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2948 2023-07-14 07:42:48.000000 langport-0.3.2/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.3.2/langport/routers/gateway/common.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16352 2023-07-19 09:19:34.000000 langport-0.3.2/langport/routers/gateway/openai_compatible.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.2/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.2/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3580 2023-07-14 07:42:48.000000 langport-0.3.2/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.2/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/cluster_monitor.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/cluster_monitor_app.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/graphite_feeder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/huggingface_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-25 16:41:24.000000 langport-0.3.2/langport/service/gateway/openai_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/gateway/tabby_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2220 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.2/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2766 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3184 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/ggml_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2731 2023-07-19 09:19:34.000000 langport-0.3.2/langport/service/server/optimum_generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-07-14 07:42:48.000000 langport-0.3.2/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.3.2/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.2/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.2/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.3.2/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-07-19 09:19:34.000000 langport-0.3.2/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.248772 langport-0.3.2/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.2/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.3.2/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3175 2023-07-14 07:42:48.000000 langport-0.3.2/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-07-19 09:19:59.240772 langport-0.3.2/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5999 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4994 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-07-19 09:19:59.000000 langport-0.3.2/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-07-19 09:19:34.000000 langport-0.3.2/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-07-19 09:19:59.248772 langport-0.3.2/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.657075 langport-0.3.3/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.3/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6186 2023-08-06 16:13:55.657075 langport-0.3.3/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5686 2023-08-03 20:25:36.000000 langport-0.3.3/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.645075 langport-0.3.3/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.3/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-08-03 12:08:25.000000 langport-0.3.3/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.649075 langport-0.3.3/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.3/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.3/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.3/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6343 2023-08-03 18:02:48.000000 langport-0.3.3/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.3/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.649075 langport-0.3.3/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.3/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.649075 langport-0.3.3/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     8911 2023-08-04 14:51:31.000000 langport-0.3.3/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.649075 langport-0.3.3/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-07-14 07:42:48.000000 langport-0.3.3/langport/data/conversation/settings/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      274 2023-07-20 08:27:07.000000 langport-0.3.3/langport/data/conversation/settings/firefly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      354 2023-07-20 08:27:07.000000 langport-0.3.3/langport/data/conversation/settings/internlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-07-20 08:27:07.000000 langport-0.3.3/langport/data/conversation/settings/llama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      286 2023-07-14 07:42:48.000000 langport-0.3.3/langport/data/conversation/settings/ningyu.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      313 2023-08-04 15:02:22.000000 langport-0.3.3/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      253 2023-08-04 14:59:44.000000 langport-0.3.3/langport/data/conversation/settings/qwen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-07-14 07:42:48.000000 langport-0.3.3/langport/data/conversation/settings/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.3/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.649075 langport-0.3.3/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.3/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.3/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-07-14 07:42:48.000000 langport-0.3.3/langport/model/adapters/baichuan.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/changgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-14 07:42:48.000000 langport-0.3.3/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      761 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/firefly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/internlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1764 2023-08-04 06:28:18.000000 langport-0.3.3/langport/model/adapters/llama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      643 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/longchat.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      840 2023-07-14 07:42:48.000000 langport-0.3.3/langport/model/adapters/ningyu.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      871 2023-08-04 13:30:11.000000 langport-0.3.3/langport/model/adapters/qwen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/robin.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      635 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/snoozy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      651 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/adapters/tigerbot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-07-14 07:42:48.000000 langport-0.3.3/langport/model/adapters/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15022 2023-08-05 19:36:27.000000 langport-0.3.3/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1752 2023-07-20 09:31:24.000000 langport-0.3.3/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5837 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.3/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5276 2023-07-14 07:42:48.000000 langport-0.3.3/langport/model/executor/generation/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    26425 2023-08-06 15:27:12.000000 langport-0.3.3/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-07-14 07:42:48.000000 langport-0.3.3/langport/model/executor/generation/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2358 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/executor/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     9777 2023-08-05 16:15:24.000000 langport-0.3.3/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1584 2023-07-20 08:27:07.000000 langport-0.3.3/langport/model/executor/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-07-23 15:24:32.000000 langport-0.3.3/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1670 2023-08-05 16:13:46.000000 langport-0.3.3/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.3/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.3/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.3/langport/model/monkey_patch_non_inplace.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.3/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.3/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5186 2023-07-24 10:02:51.000000 langport-0.3.3/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.3/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2948 2023-07-14 07:42:48.000000 langport-0.3.3/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7997 2023-08-04 09:51:30.000000 langport-0.3.3/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    17665 2023-08-04 14:24:42.000000 langport-0.3.3/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.3/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.3/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3576 2023-07-24 11:26:02.000000 langport-0.3.3/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.653075 langport-0.3.3/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.3/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.657075 langport-0.3.3/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-08-04 09:01:15.000000 langport-0.3.3/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5231 2023-08-04 09:45:33.000000 langport-0.3.3/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.657075 langport-0.3.3/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2220 2023-07-20 08:27:07.000000 langport-0.3.3/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.3/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2811 2023-08-05 16:14:11.000000 langport-0.3.3/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3184 2023-07-20 08:27:07.000000 langport-0.3.3/langport/service/server/ggml_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2731 2023-07-20 08:27:07.000000 langport-0.3.3/langport/service/server/optimum_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.657075 langport-0.3.3/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-07-14 07:42:48.000000 langport-0.3.3/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1205 2023-08-03 14:44:38.000000 langport-0.3.3/langport/utils/cache.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      506 2023-07-20 09:34:45.000000 langport-0.3.3/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.3/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.3/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-08-06 13:40:01.000000 langport-0.3.3/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-08-03 16:42:56.000000 langport-0.3.3/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.657075 langport-0.3.3/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.3/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3046 2023-08-06 13:47:58.000000 langport-0.3.3/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3152 2023-08-06 15:16:39.000000 langport-0.3.3/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-08-06 16:13:55.649075 langport-0.3.3/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6186 2023-08-06 16:13:55.000000 langport-0.3.3/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5072 2023-08-06 16:13:55.000000 langport-0.3.3/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-08-06 16:13:55.000000 langport-0.3.3/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-08-06 16:13:55.000000 langport-0.3.3/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-08-06 16:13:55.000000 langport-0.3.3/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-08-03 16:43:02.000000 langport-0.3.3/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-08-06 16:13:55.657075 langport-0.3.3/setup.cfg
```

### Comparing `langport-0.3.2/LICENSE` & `langport-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/PKG-INFO` & `langport-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: langport
-Version: 0.3.2
-Summary: A large language model serving platform.
-Project-URL: Homepage, https://github.com/vtuber-plan/langport
-Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: ggml
-Provides-Extra: optimum
-License-File: LICENSE
-
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/vtuber-plan/langport?style=social">
 </a>
@@ -55,14 +40,15 @@
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/08/04] Dynamic batch inference.
 - [2023/07/16] Support int4 quantization.
 - [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
@@ -147,14 +133,20 @@
 
 Run text generation with ggml worker:
 
 ```bash
 python -m langport.service.server.ggml_generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
+Run OpenAI forward server: 
+```bash
+python -m langport.service.server.chatgpt_generation_worker --port 21001 --api-url <url> --api-key <key>
+```
+
+
 ## License
 
 langport is released under the Apache Software License.
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: langport Version: 0.3.2 Summary: A large language
-model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
-langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
-Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
 training and evaluation make it complicated. The core features include: -
@@ -22,30 +15,30 @@
 Tested Models * NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon,
 Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV,
 StableLM and so on. ## Benchmark We use single RTX3090 to run a finetuned 7B
 LLaMA model (OpenBuddy V0.9) under the bf16 setting. We create 32 threads to
 submit chat tasks to the server, and the following figure shows the Queries Per
 Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with
 different max model concurrency settings. ![benchmark_chat](assets/
-benchmark_chat.jpg) ## News - [2023/07/16] Support int4 quantization. - [2023/
-07/13] Support generation logprobs parameter. - [2023/06/18] Add ggml
-(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
-LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
-support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
-06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
-[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
-supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
-With pip ```bash pip install langport ``` or: ```bash pip install git+https://
-github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
-this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
-```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
-Clone this repository ```bash git clone https://github.com/vtuber-plan/
-langport.git cd langport ``` 2. Install the Package ```bash pip install --
-upgrade pip pip install -e . ``` ## Start the server It is simple to start a
-single node chat API service: ``` bash python -
+benchmark_chat.jpg) ## News - [2023/08/04] Dynamic batch inference. - [2023/07/
+16] Support int4 quantization. - [2023/07/13] Support generation logprobs
+parameter. - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.)
+worker support. - [2023/06/09] Add LLama.cpp worker support. - [2023/06/01] Add
+HuggingFace Bert embedding worker support. - [2023/06/01] Add HuggingFace text
+generation API support. - [2023/06/01] Add tabby API support. - [2023/05/23]
+Add chat throughput test script. - [2023/05/22] New distributed architecture. -
+[2023/05/14] Batch inference supported. - [2023/05/10] Langport project
+started. ## Install ### Method 1: With pip ```bash pip install langport ``` or:
+```bash pip install git+https://github.com/vtuber-plan/langport.git ``` If you
+need ggml generation worker, use this command: ```bash pip install langport
+[ggml] ``` If you wanna use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml]
+``` ### Method 2: From source 1. Clone this repository ```bash git clone https:
+//github.com/vtuber-plan/langport.git cd langport ``` 2. Install the Package
+```bash pip install --upgrade pip pip install -e . ``` ## Start the server It
+is simple to start a single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
 localhost:21001 python -m langport.service.server.embedding_worker --model-path
 --neighbors http://localhost:21001 python -
@@ -65,13 +58,14 @@
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
 generation with ggml worker: ```bash python -
 m langport.service.server.ggml_generation_worker --port 21001 --model-path  --
 gpu-layers
-resize this for your VRAM)> ``` ## License langport is released under the
-Apache Software License. ## See also - [langport-docs](https://github.com/
-vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
-vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
-history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
-history.com/#vtuber-plan/langport&Date)
+resize this for your VRAM)> ``` Run OpenAI forward server: ```bash python -
+m langport.service.server.chatgpt_generation_worker --port 21001 --api-url  --
+api-key  ``` ## License langport is released under the Apache Software License.
+## See also - [langport-docs](https://github.com/vtuber-plan/langport/tree/
+main/docs) - [langport-source](https://github.com/vtuber-plan/langport) ## Star
+History [![Star History Chart](https://api.star-history.com/svg?repos=vtuber-
+plan/langport&type=Date)](https://star-history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.3.2/README.md` & `langport-0.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: langport
+Version: 0.3.3
+Summary: A large language model serving platform.
+Project-URL: Homepage, https://github.com/vtuber-plan/langport
+Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: ggml
+Provides-Extra: optimum
+License-File: LICENSE
+
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/vtuber-plan/langport?style=social">
 </a>
@@ -40,14 +55,15 @@
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/08/04] Dynamic batch inference.
 - [2023/07/16] Support int4 quantization.
 - [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
@@ -132,14 +148,20 @@
 
 Run text generation with ggml worker:
 
 ```bash
 python -m langport.service.server.ggml_generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
+Run OpenAI forward server: 
+```bash
+python -m langport.service.server.chatgpt_generation_worker --port 21001 --api-url <url> --api-key <key>
+```
+
+
 ## License
 
 langport is released under the Apache Software License.
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1 Name: langport Version: 0.3.3 Summary: A large language
+model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
+langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
+Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
 training and evaluation make it complicated. The core features include: -
@@ -15,30 +22,30 @@
 Tested Models * NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon,
 Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV,
 StableLM and so on. ## Benchmark We use single RTX3090 to run a finetuned 7B
 LLaMA model (OpenBuddy V0.9) under the bf16 setting. We create 32 threads to
 submit chat tasks to the server, and the following figure shows the Queries Per
 Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with
 different max model concurrency settings. ![benchmark_chat](assets/
-benchmark_chat.jpg) ## News - [2023/07/16] Support int4 quantization. - [2023/
-07/13] Support generation logprobs parameter. - [2023/06/18] Add ggml
-(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
-LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
-support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
-06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
-[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
-supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
-With pip ```bash pip install langport ``` or: ```bash pip install git+https://
-github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
-this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
-```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
-Clone this repository ```bash git clone https://github.com/vtuber-plan/
-langport.git cd langport ``` 2. Install the Package ```bash pip install --
-upgrade pip pip install -e . ``` ## Start the server It is simple to start a
-single node chat API service: ``` bash python -
+benchmark_chat.jpg) ## News - [2023/08/04] Dynamic batch inference. - [2023/07/
+16] Support int4 quantization. - [2023/07/13] Support generation logprobs
+parameter. - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.)
+worker support. - [2023/06/09] Add LLama.cpp worker support. - [2023/06/01] Add
+HuggingFace Bert embedding worker support. - [2023/06/01] Add HuggingFace text
+generation API support. - [2023/06/01] Add tabby API support. - [2023/05/23]
+Add chat throughput test script. - [2023/05/22] New distributed architecture. -
+[2023/05/14] Batch inference supported. - [2023/05/10] Langport project
+started. ## Install ### Method 1: With pip ```bash pip install langport ``` or:
+```bash pip install git+https://github.com/vtuber-plan/langport.git ``` If you
+need ggml generation worker, use this command: ```bash pip install langport
+[ggml] ``` If you wanna use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml]
+``` ### Method 2: From source 1. Clone this repository ```bash git clone https:
+//github.com/vtuber-plan/langport.git cd langport ``` 2. Install the Package
+```bash pip install --upgrade pip pip install -e . ``` ## Start the server It
+is simple to start a single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
 localhost:21001 python -m langport.service.server.embedding_worker --model-path
 --neighbors http://localhost:21001 python -
@@ -58,13 +65,14 @@
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
 generation with ggml worker: ```bash python -
 m langport.service.server.ggml_generation_worker --port 21001 --model-path  --
 gpu-layers
-resize this for your VRAM)> ``` ## License langport is released under the
-Apache Software License. ## See also - [langport-docs](https://github.com/
-vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
-vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
-history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
-history.com/#vtuber-plan/langport&Date)
+resize this for your VRAM)> ``` Run OpenAI forward server: ```bash python -
+m langport.service.server.chatgpt_generation_worker --port 21001 --api-url  --
+api-key  ``` ## License langport is released under the Apache Software License.
+## See also - [langport-docs](https://github.com/vtuber-plan/langport/tree/
+main/docs) - [langport-source](https://github.com/vtuber-plan/langport) ## Star
+History [![Star History Chart](https://api.star-history.com/svg?repos=vtuber-
+plan/langport&type=Date)](https://star-history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.3.2/langport/constants.py` & `langport-0.3.3/langport/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import IntEnum
 
 
 HEART_BEAT_EXPIRATION = 90
 WORKER_HEART_BEAT_INTERVAL = 30
 EMBEDDING_INFERENCE_INTERVAL = 0.1
-GENERATION_INFERENCE_INTERVAL = 0.3
+GENERATION_INFERENCE_INTERVAL = 0.5
 WORKER_API_TIMEOUT = 20
 
 LOGDIR = "./logs"
 
 class ErrorCode(IntEnum):
     OK = 200
     VALIDATION_TYPE_ERROR = 40001
```

### Comparing `langport-0.3.2/langport/core/base_node.py` & `langport-0.3.3/langport/core/base_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/core/cluster_node.py` & `langport-0.3.3/langport/core/cluster_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/core/cluster_worker.py` & `langport-0.3.3/langport/core/cluster_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,19 @@
                 raise ValueError("Bad chunk type.")
 
         del self.output_queue[task_id]
 
     def get_num_tasks(self) -> int:
         return self.task_queue.qsize()
 
-    def fetch_tasks(self) -> List[BaseWorkerResult]:
+    def fetch_tasks(self, task_num: Optional[int]=None) -> List[BaseWorkerResult]:
+        if task_num is None:
+            task_num = self.max_batch
         task_batch = []
-        while len(task_batch) < self.max_batch:
+        while len(task_batch) < task_num:
             try:
                 task = self.task_queue.get(block=False, timeout=None)
             except queue.Empty:
                 break
             task_batch.append(task)
         return task_batch
```

### Comparing `langport-0.3.2/langport/data/conversation/__init__.py` & `langport-0.3.3/langport/data/conversation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     NO_COLON_SINGLE = auto()
     ADD_NEW_LINE_SINGLE = auto()
     DOLLY = auto()
     RWKV = auto()
     PHOENIX = auto()
     CHATGLM = auto()
     LLAMA = auto()
+    CHATLM = auto()
 
 
 @dataclasses.dataclass
 class ConversationSettings:
     # The name of this settings
     name: str
     # Two roles
@@ -176,23 +177,39 @@
         elif self.settings.sep_style == SeparatorStyle.LLAMA:
             B_INST, E_INST = "[INST]", "[/INST]"
             B_SYS, E_SYS = "<<SYS>>\n", "\n<</SYS>>\n\n"
             system_q = B_SYS + self.system + E_SYS
             system_a = ""
             ret = f"{B_INST} {system_q} {E_INST} {system_a}"
             for i, (role, message) in enumerate(self.messages):
-                if i % 2 == 0:
-                    inst = B_INST
+                if role == self.settings.roles[0]:
+                    if not(i != 0 and self.messages[i - 1][0] == self.settings.roles[0]):
+                        inst = B_INST
                 else:
                     inst = E_INST
                 if message:
                     ret += inst + " " + message.strip() + " "
                 else:
                     ret += inst + " "
             return ret
+        elif self.settings.sep_style == SeparatorStyle.CHATLM:
+            im_start, im_end = "<|im_start|>", "<|im_end|>"
+            ret = im_start + "system" + "\n" + self.system + im_end
+            if self.settings.system_sep is not None:
+                ret += self.settings.system_sep
+            else:
+                ret += self.settings.sep
+
+            for i, (role, message) in enumerate(self.messages):
+                ret += im_start
+                if message:
+                    ret += role + "\n" + message + im_end + self.settings.sep
+                else:
+                    ret += role + "\n"
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.settings.sep_style}")
 
     def append_message(self, role: str, message: str):
         """Append a new message."""
         self.messages.append([role, message])
```

### Comparing `langport-0.3.2/langport/data/conversation/conversation_settings.py` & `langport-0.3.3/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/baichuan.py` & `langport-0.3.3/langport/model/adapters/baichuan.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/baize.py` & `langport-0.3.3/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/bard.py` & `langport-0.3.3/langport/model/adapters/bard.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/billa.py` & `langport-0.3.3/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/changgpt.py` & `langport-0.3.3/langport/model/adapters/changgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/chatglm.py` & `langport-0.3.3/langport/model/adapters/chatglm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/chatgpt.py` & `langport-0.3.3/langport/model/adapters/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/claude.py` & `langport-0.3.3/langport/model/adapters/claude.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/dolly_v2.py` & `langport-0.3.3/langport/model/adapters/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/falcon.py` & `langport-0.3.3/langport/model/adapters/falcon.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/firefly.py` & `langport-0.3.3/langport/model/adapters/firefly.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/internlm.py` & `langport-0.3.3/langport/model/adapters/internlm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/koala.py` & `langport-0.3.3/langport/model/adapters/koala.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/longchat.py` & `langport-0.3.3/langport/model/adapters/longchat.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/ningyu.py` & `langport-0.3.3/langport/model/adapters/ningyu.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/oasst_pythia.py` & `langport-0.3.3/langport/model/adapters/oasst_pythia.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/openbuddy.py` & `langport-0.3.3/langport/model/adapters/openbuddy.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/phoenix.py` & `langport-0.3.3/langport/model/adapters/phoenix.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/robin.py` & `langport-0.3.3/langport/model/adapters/robin.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/rwkv.py` & `langport-0.3.3/langport/model/adapters/rwkv.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/snoozy.py` & `langport-0.3.3/langport/model/adapters/snoozy.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/stable_lm.py` & `langport-0.3.3/langport/model/adapters/stable_lm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/tigerbot.py` & `langport-0.3.3/langport/model/adapters/tigerbot.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/vicuna.py` & `langport-0.3.3/langport/model/adapters/vicuna.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/adapters/wizardlm.py` & `langport-0.3.3/langport/model/adapters/wizardlm.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/compression.py` & `langport-0.3.3/langport/model/compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 import dataclasses
 import gc
 import glob
 import os
-from typing import Tuple, Union
+from typing import List, Tuple, Union
 
 from accelerate import init_empty_weights
 from accelerate.utils import set_module_tensor_to_device
 import torch
 from torch import Tensor
 import torch.nn as nn
 from torch.nn import functional as F
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModelForCausalLM, AutoConfig
 
+try:
+    import cupy
+    cupy_available = True
+except ImportError:
+    cupy_available = False
+    print("Info: Install cupy to get better quantization performance.")
+
 @dataclasses.dataclass
 class CompressionConfig:
     """Group-wise quantization."""
 
     num_bits: int
     group_size: int
     group_dim: int
     symmetric: bool
     enabled: bool = True
 
-
+# Symmetric False need small group_size
 default_compression_config = CompressionConfig(
     num_bits=8, group_size=256, group_dim=1, symmetric=True, enabled=True
 )
 
 bit4_compression_config = CompressionConfig(
-    num_bits=4, group_size=256, group_dim=1, symmetric=True, enabled=True
+    num_bits=4, group_size=32, group_dim=1, symmetric=True, enabled=True
 )
 
 bit2_compression_config = CompressionConfig(
-    num_bits=2, group_size=64, group_dim=1, symmetric=False, enabled=True
+    num_bits=2, group_size=4, group_dim=1, symmetric=False, enabled=True
 )
 
 class CLinear(nn.Module):
     """Compressed Linear Layer."""
     __constants__ = ['config']
     config: CompressionConfig
     weight: Union[Tensor, Tuple]
     bias: Tensor
+
     def __init__(self, compression_config: CompressionConfig, weight=None, bias=None, device=None):
         super().__init__()
         self.config = compression_config
         if weight is None:
             self.weight = None
         elif isinstance(weight, Tensor):
             self.weight = compress(weight.data.to(device), self.config)
         else:
             self.weight = weight
         self.bias = bias
+        self.bias_dtype = {}
 
     def forward(self, input: Tensor) -> Tensor:
         weight = decompress(self.weight, self.config, input.dtype)
-        if self.bias is not None:
-            bias = self.bias.to(input.dtype)
+        if input.dtype in self.bias_dtype:
+            bias = self.bias_dtype[input.dtype]
         else:
-            bias = self.bias
+            if self.bias is not None:
+                bias = self.bias.to(input.dtype)
+                self.bias_dtype[input.dtype] = bias
+            else:
+                bias = self.bias
         return F.linear(input, weight, bias)
     
     def extra_repr(self) -> str:
         return 'num_bits={}, group_size={}, group_dim={}, symmetric={}, bias={}'.format(
             self.config.num_bits,
             self.config.group_size,
             self.config.group_dim,
@@ -144,15 +157,16 @@
                     tensor, compression_config
                 )
             else:
                 compressed_state_dict[name] = tmp_state_dict[name].to(device)
             tmp_state_dict[name] = None
             tensor = None
             gc.collect()
-            torch.cuda.empty_cache()
+            if torch.cuda.is_available():
+                torch.cuda.empty_cache()
 
     for name in model.state_dict():
         if name not in linear_weights:
             set_module_tensor_to_device(
                 model, name, device, value=compressed_state_dict[name]
             )
     apply_compressed_weight(model, compressed_state_dict, device, compression_config)
@@ -205,77 +219,73 @@
         final_shape[group_dim + 1] = final_shape[group_dim + 1] // 4
         final_data = torch.zeros(size=final_shape, dtype=torch.uint8, device=data.device)
 
     # Quantize
     B = 2 ** (num_bits - 1) - 1
     if num_bits >= 8:
         if symmetric:
-            scale = B / torch.max(data.abs(), dim=group_dim + 1, keepdim=True)[0]
+            mn = None
+            scale = B * torch.max(data.abs(), dim=group_dim + 1, keepdim=True)[0].pow_(-1)
             data = data * scale
-            data = data.clamp_(-B, B).round_().to(torch.int8)
-
-            inv_scale = 1.0 / scale
-            return data, None, scale, inv_scale, original_shape
+            data = data.clamp_(-B, B).round_().type(torch.int8)
         else:
             mn = torch.min(data, dim=group_dim + 1, keepdim=True)[0]
             mx = torch.max(data, dim=group_dim + 1, keepdim=True)[0]
 
             scale = B / (mx - mn)
             data = data - mn
             data.mul_(scale)
+            data = data.clamp_(0, B).round_().type(torch.uint8)
 
-            data = data.clamp_(0, B).round_().to(torch.uint8)
-
-            inv_scale = 1.0 / scale
-            return data, mn, scale, inv_scale, original_shape
+        inv_scale = 1.0 / scale
+        return data, mn, inv_scale, original_shape
     elif num_bits > 2:
         if symmetric:
+            mn = None
             scale = B / torch.max(data.abs(), dim=group_dim + 1, keepdim=True)[0]
             data = data * scale
             data = data.clamp_(-B, B).round_().to(torch.int16)
             data = (data + B).to(torch.uint8)
-
-            left_half = [slice(None) for i in new_shape]
-            left_half[group_dim + 1] = slice(0, group_size//2)
-            final_data = torch.bitwise_left_shift(data[left_half], 4)
-
-            right_half = [slice(None) for i in new_shape]
-            right_half[group_dim + 1] = slice(group_size//2, group_size)
-            final_data = final_data.bitwise_or_(data[right_half])
-
-            inv_scale = 1.0 / scale
-            return final_data, None, scale, inv_scale, original_shape
         else:
             mn = torch.min(data, dim=group_dim + 1, keepdim=True)[0]
             mx = torch.max(data, dim=group_dim + 1, keepdim=True)[0]
 
             scale = B / (mx - mn)
             data = data - mn
             data.mul_(scale)
 
             data = data.clamp_(0, B).round_().to(torch.uint8)
-            left_half = [slice(None) for i in new_shape]
-            left_half[group_dim + 1] = slice(0, group_size//2)
-            final_data = torch.bitwise_left_shift(data[left_half], 4)
-
-            right_half = [slice(None) for i in new_shape]
-            right_half[group_dim + 1] = slice(group_size//2, group_size)
-            final_data = final_data.bitwise_or_(data[right_half])
-            
-            inv_scale = 1.0 / scale
-            return final_data, mn, scale, inv_scale, original_shape
+        
+        left_half = [slice(None) for i in new_shape]
+        left_half[group_dim + 1] = slice(0, group_size//2)
+        final_data.bitwise_or_(torch.bitwise_left_shift(data[left_half], 4))
+
+        right_half = [slice(None) for i in new_shape]
+        right_half[group_dim + 1] = slice(group_size//2, group_size)
+        final_data.bitwise_or_(data[right_half])
+
+        inv_scale = 1.0 / scale
+        return final_data, mn, inv_scale, original_shape
     else:
-        mn = torch.min(data, dim=group_dim + 1, keepdim=True)[0]
-        mx = torch.max(data, dim=group_dim + 1, keepdim=True)[0]
+        if symmetric:
+            mn = None
+            scale = B / torch.max(data.abs(), dim=group_dim + 1, keepdim=True)[0]
+            data = data * scale
+            data = data.clamp_(-B, B).round_().to(torch.int16)
+            data = (data + B).to(torch.uint8)
+        else:
+            mn = torch.min(data, dim=group_dim + 1, keepdim=True)[0]
+            mx = torch.max(data, dim=group_dim + 1, keepdim=True)[0]
 
-        scale = B / (mx - mn)
-        data = data - mn
-        data.mul_(scale)
+            scale = B / (mx - mn)
+            data = data - mn
+            data.mul_(scale)
+
+            data = data.clamp_(0, B).round_().to(torch.uint8)
 
-        data = data.clamp_(0, B).round_().to(torch.uint8)
         first_half = [slice(None) for i in new_shape]
         first_half[group_dim + 1] = slice(0, group_size//4)
         final_data = torch.bitwise_left_shift(data[first_half], 6)
 
         second_half = [slice(None) for i in new_shape]
         second_half[group_dim + 1] = slice(group_size//4, group_size//4*2)
         final_data = final_data.bitwise_or_(torch.bitwise_left_shift(data[second_half], 4))
@@ -285,89 +295,98 @@
         final_data = final_data.bitwise_or_(torch.bitwise_left_shift(data[third_half], 2))
 
         fourth_half = [slice(None) for i in new_shape]
         fourth_half[group_dim + 1] = slice(group_size//4*3, group_size)
         final_data = final_data.bitwise_or_(data[fourth_half])
 
         inv_scale = 1.0 / scale
-        return final_data, mn, scale, inv_scale, original_shape
+        return final_data, mn, inv_scale, original_shape
+
+@torch.jit.script
+def unpack_int4(data: torch.Tensor, group_dim: int, group_size: int, new_shape: List[int], dtype: torch.dtype):
+    left_half = torch.bitwise_right_shift(data, 4)
+    right_half = torch.bitwise_and(data, 0b00001111)
+    float_data = torch.concat((left_half, right_half), dim=group_dim + 1).to(dtype)
+    return float_data
 
 def decompress(packed_data, config, dtype=torch.float32):
     """Simulate group-wise dequantization."""
     if not config.enabled:
         return packed_data
 
     group_size, num_bits, group_dim, symmetric = (
         config.group_size,
         config.num_bits,
         config.group_dim,
         config.symmetric,
     )
 
-    data, mn, scale, inv_scale, original_shape = packed_data
+    data, mn, inv_scale, original_shape = packed_data
+    num_groups = (original_shape[group_dim] + group_size - 1) // group_size
     B = 2 ** (num_bits - 1) - 1
     if num_bits >= 8:
         # Dequantize
         if symmetric:
             # data = data.to(dtype) * inv_scale.to(dtype)
-            data = data.to(dtype)
-            data = data.mul_(inv_scale)
+            data = data.type(dtype)
+            data.mul_(inv_scale)
         else:
             data = data.to(dtype)
             data = data.mul_(inv_scale).add_(mn)
     elif num_bits > 2:
         new_shape = [i for i in data.shape]
-        new_shape[group_dim + 1] = 2 * new_shape[group_dim + 1]
+        new_shape[group_dim + 1] = group_size
 
         float_data = torch.empty(size=new_shape, dtype=dtype, device=data.device)
-
         left_half = [slice(None) for i in new_shape]
         left_half[group_dim + 1] = slice(0, group_size//2)
-        float_data[left_half] = torch.bitwise_and(data, 0b11110000).bitwise_right_shift_(4)
-
+        float_data[left_half] = torch.bitwise_right_shift(data, 4)
+        
         right_half = [slice(None) for i in new_shape]
         right_half[group_dim + 1] = slice(group_size//2, group_size)
         float_data[right_half] = torch.bitwise_and(data, 0b00001111)
 
-        # left_half = torch.bitwise_and(data, 0b11110000).bitwise_right_shift_(4)
-        # right_half = torch.bitwise_and(data, 0b00001111)
-        # float_data = torch.concat((left_half, right_half), dim=group_dim + 1).to(dtype)
+        # float_data = unpack_int4(data, group_dim, group_size, new_shape, dtype)
 
         if symmetric:
             float_data = float_data.sub_(B)
             data = float_data.mul_(inv_scale)
         else:
-            data = float_data.mul_(inv_scale).add_(mn)
+            # data = float_data.mul_(inv_scale).add_(mn)
+            data = torch.addcmul(mn, float_data, inv_scale, value=1.0)
     else:
         new_shape = [i for i in data.shape]
         new_shape[group_dim + 1] = 4 * new_shape[group_dim + 1]
-        int8_data = torch.zeros(size=new_shape, dtype=torch.uint8, device=data.device)
+        float_data = torch.empty(size=new_shape, dtype=dtype, device=data.device)
 
         first_half = [slice(None) for i in new_shape]
         first_half[group_dim + 1] = slice(0, group_size//4)
         first_mask = torch.tensor([0b11000000], dtype=torch.uint8, device=data.device)
-        int8_data[first_half] = torch.bitwise_right_shift(torch.bitwise_and(data, first_mask), 6)
+        float_data[first_half] = torch.bitwise_right_shift(torch.bitwise_and(data, first_mask), 6)
 
         second_half = [slice(None) for i in new_shape]
         second_half[group_dim + 1] = slice(group_size//4, group_size//4*2)
         second_mask = torch.tensor([0b00110000], dtype=torch.uint8, device=data.device)
-        int8_data[second_half] = torch.bitwise_right_shift(torch.bitwise_and(data, second_mask), 4)
+        float_data[second_half] = torch.bitwise_right_shift(torch.bitwise_and(data, second_mask), 4)
         
         third_half = [slice(None) for i in new_shape]
         third_half[group_dim + 1] = slice(group_size//4*2, group_size//4*3)
         third_mask = torch.tensor([0b00001100], dtype=torch.uint8, device=data.device)
-        int8_data[third_half] = torch.bitwise_right_shift(torch.bitwise_and(data, third_mask), 2)
+        float_data[third_half] = torch.bitwise_right_shift(torch.bitwise_and(data, third_mask), 2)
 
         fourth_half = [slice(None) for i in new_shape]
         fourth_half[group_dim + 1] = slice(group_size//4*3, group_size)
         fourth_mask = torch.tensor([0b00000011], dtype=torch.uint8, device=data.device)
-        int8_data[fourth_half] = torch.bitwise_and(data, fourth_mask)
+        float_data[fourth_half] = torch.bitwise_and(data, fourth_mask)
         
-        data = int8_data.to(dtype)
-        data = data.mul_(inv_scale).add_(mn)
+        if symmetric:
+            float_data = float_data.sub_(B)
+            data = float_data.mul_(inv_scale)
+        else:
+            data = float_data.mul_(inv_scale).add_(mn)
     
     # Unpad
     pad_len = (group_size - original_shape[group_dim] % group_size) % group_size
     if pad_len:
         padded_original_shape = (
             original_shape[:group_dim]
             + (original_shape[group_dim] + pad_len,)
```

### Comparing `langport-0.3.2/langport/model/executor/base.py` & `langport-0.3.3/langport/model/executor/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-
 from typing import List, Optional
 
-
 class BaseModelExecutor(object):
     def __init__(
         self,
         model_name: str,
     ) -> None:
         self.model_name = model_name
 
     @property
     def context_length(self) -> int:
         return 2048
 
     def tokenize(self, text: str) -> List[int]:
         raise NotImplementedError("executor tokenizer method is not implemented.")
 
-
-
 class LocalModelExecutor(BaseModelExecutor):
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
@@ -43,15 +39,14 @@
     @property
     def context_length(self) -> int:
         return 2048
 
     def tokenize(self, text: str) -> List[int]:
         raise NotImplementedError("executor tokenizer method is not implemented.")
 
-
 class RemoteModelExecutor(BaseModelExecutor):
     def __init__(
         self,
         model_name: str,
         api_url: str,
         api_key: str,
     ) -> None:
@@ -62,8 +57,8 @@
         self.api_key = api_key
 
     @property
     def context_length(self) -> int:
         return 2048
 
     def tokenize(self, text: str) -> List[int]:
-        raise NotImplementedError("executor tokenizer method is not implemented.")
+        raise NotImplementedError("executor tokenizer method is not implemented.")
```

### Comparing `langport-0.3.2/langport/model/executor/embedding/__init__.py` & `langport-0.3.3/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/embedding/huggingface.py` & `langport-0.3.3/langport/model/executor/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/generation/__init__.py` & `langport-0.3.3/langport/model/executor/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/generation/chatgpt.py` & `langport-0.3.3/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/generation/ggml.py` & `langport-0.3.3/langport/model/executor/generation/ggml.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/generation/huggingface.py` & `langport-0.3.3/langport/model/executor/generation/huggingface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 from langport.model.executor.generation import BaseStreamer
 
 from langport.model.executor.huggingface import HuggingfaceExecutor
 
 from langport.protocol.worker_protocol import (
     BaseWorkerResult,
     GenerationTask,
@@ -10,14 +10,15 @@
     GenerationWorkerResult,
     UsageInfo,
 )
 
 import torch
 
 from transformers import PreTrainedModel, PreTrainedTokenizer
+from transformers.utils import is_optimum_available
 from transformers.generation.logits_process import (
     LogitsProcessor,
     LogitsProcessorList,
     TemperatureLogitsWarper,
     RepetitionPenaltyLogitsProcessor,
     TopPLogitsWarper,
     TopKLogitsWarper,
@@ -84,28 +85,36 @@
             )
             self.logits_processor_list.append(logits_processor)
         
         # variables used in the streaming process
         self.batch_tokens_cache: List[List[int]] = [[] for i in range(self.batch_size)]
         self.batch_tokens_probs_cache: List[List[float]] = [[] for i in range(self.batch_size)]
         self.batch_top_logprobs_cache: List[List[Dict[str, float]]] = [[] for i in range(self.batch_size)]
-        self.stop = [False for i in range(self.batch_size)]
+        self.stop: List[bool] = [False for i in range(self.batch_size)]
 
     def __len__(self):
         return self.batch_size
     
-    def __call__(self, return_attention_mask=True) -> Any:
-        ids = [torch.cat((self.prompts_ids[i], torch.LongTensor(self.batch_tokens_cache[i])))
-                         for i in range(self.batch_size)]
-        length = [len(i) for i in ids]
+    def __call__(self, return_attention_mask=True, full_batch=False) -> Any:
+        ids: List[torch.LongTensor] = []
+        length: List[int] = []
+        for i in range(self.batch_size):
+            if not full_batch and self.is_stop(i):
+                continue
+            input_ids = torch.cat((self.prompts_ids[i], torch.LongTensor(self.batch_tokens_cache[i])))
+            ids.append(input_ids)
+            length.append(len(input_ids))
+        
+        dyn_batch_size = len(ids)
         # padding to max(length)
-        full_input_ids = torch.full(
-            (self.batch_size, max(length)), self.pad_fill_id, dtype=torch.long, device=self.device
+        full_input_ids: torch.LongTensor = torch.full(
+            (dyn_batch_size, max(length)), self.pad_fill_id,
+            dtype=torch.long, device=self.device
         )
-        for i in range(self.batch_size):
+        for i in range(dyn_batch_size):
             if self.is_encoder_decoder:
                 full_input_ids[i, :length[i]] = ids[i]
             else:
                 full_input_ids[i, -length[i]:] = ids[i] # padding side left
         if not return_attention_mask:
             return full_input_ids
         return full_input_ids, self._gen_attention_mask(length)
@@ -188,40 +197,49 @@
         self._check_idx(idx)
         self.stop[idx] = True
     
     def is_stop(self, idx:int):
         self._check_idx(idx)
         return self.stop[idx]
 
-
 class GenerationModel:
     def __init__(self, model: PreTrainedModel) -> None:
         self.model = model
     
     @torch.inference_mode()
     def generate(self, inputs: BatchingTask, 
                  max_new_tokens: int,
                  streamer: Optional[BaseStreamer]=None) -> torch.Tensor:
 
         if inputs.batch_size == 0:
             return
 
-        full_input_ids, attention_mask = inputs()
+        full_input_ids, full_attention_mask = inputs(return_attention_mask=True, full_batch=True)
         if self.model.config.is_encoder_decoder:
-            encoder_outputs = self.model.encoder(input_ids=full_input_ids, attention_mask=attention_mask)
-            decoder_input_ids_list = [torch.full(
+            full_encoder_outputs = self.model.encoder(
+                input_ids=full_input_ids,
+                attention_mask=full_attention_mask,
+                output_attentions=False,
+                output_hidden_states=False,
+                return_dict=False,
+            )
+            decoder_input_ids_list: List[torch.LongTensor] = [torch.full(
                 (inputs.batch_size, 1),
                 self.model.generation_config.decoder_start_token_id,
                 dtype=torch.long,
                 device=self.model.device,
             )]
         else:
-            encoder_outputs = None
-            decoder_input_ids_list = [full_input_ids]
-        past_key_values = None
+            full_encoder_outputs = None
+            decoder_input_ids_list: List[torch.LongTensor] = [full_input_ids]
+        
+        encoder_outputs = full_encoder_outputs
+        attention_mask = full_attention_mask
+        past_key_values: Optional[List[Tuple[torch.Tensor, torch.Tensor]]] = None
+        bacth_mapping: List[int] = list(range(inputs.batch_size)) # dynamic batch
 
         # step by step
         for step in range(max_new_tokens):
             # inference a step
             if len(decoder_input_ids_list) > 1:
                 decoder_input_ids = torch.stack(decoder_input_ids_list, dim=1)
             elif len(decoder_input_ids_list) == 1:
@@ -236,15 +254,15 @@
                     past_key_values=past_key_values,
                 )
             else:
                 if step > 0:
                     dynamic_attention_mask = torch.cat(
                         (attention_mask, 
                         torch.ones(
-                            inputs.batch_size, step,
+                            attention_mask.shape[0], step,
                             dtype=torch.long, device=decoder_input_ids.device
                         )), dim=1
                     )
                 else:
                     dynamic_attention_mask = attention_mask
                 out = self.model(
                     input_ids=decoder_input_ids,
@@ -257,62 +275,120 @@
             decoder_input_ids_list = []
 
             new_ids = []
             # logprobs
             token_probs = [None] * inputs.batch_size
             top_logprobs = [None] * inputs.batch_size
 
-            for i, task in enumerate(inputs.tasks):
-                if inputs.is_stop(i):
+            for task_i, task in enumerate(inputs.tasks):
+                if inputs.is_stop(task_i):
                     new_ids.append(inputs.pad_fill_id)
                     continue
-                each_logits = logits[i, -1, :].unsqueeze(0)
+                batch_i = bacth_mapping[task_i]
+                each_logits = logits[batch_i, -1, :].unsqueeze(0)
 
-                logits_processor = inputs.get_logits_processor_list(i)
+                logits_processor = inputs.get_logits_processor_list(task_i)
                 if logits_processor:
                     if task.repetition_penalty > 1.0:
-                        tmp_output_ids = decoder_input_ids[i, :].unsqueeze(0)
+                        tmp_output_ids = decoder_input_ids[batch_i, :].unsqueeze(0)
                     else:
                         tmp_output_ids = None
                     last_token_logits = logits_processor(tmp_output_ids, each_logits)[0]
                 else:
                     last_token_logits = each_logits
 
                 if self.model.device.type == "mps":
                     # Switch to CPU by avoiding some bugs in mps backend.
                     last_token_logits = last_token_logits.float().to("cpu")
 
                 if task.temperature < 1e-5 or task.top_p < 1e-8:  # greedy
                     token = int(torch.argmax(last_token_logits))
                 else:
                     probs = torch.softmax(last_token_logits, dim=-1)
-                    token = int(torch.multinomial(probs, num_samples=1))
+                    token = int(torch.multinomial(probs, num_samples=1, replacement=True).item())
                 
                 if task.logprobs is not None:
-                    token_probs[i] = each_logits[0, token].item()
+                    token_probs[task_i] = each_logits[0, token].item()
                     top_values, top_indices = torch.topk(each_logits[0, :], task.logprobs, dim=-1, largest=True, sorted=True)
                     item = {}
                     for top_i in range(len(top_values)):
                         item[top_indices[top_i].item()] = top_values[top_i].item()
-                    top_logprobs[i] = item
+                    top_logprobs[task_i] = item
                 new_ids.append(token)
             
+            is_stop_before = [s for s in inputs.stop]
             # update state
             inputs.update_new_token(new_ids, token_probs=token_probs, top_logprobs=top_logprobs)
             if streamer:
                 streamer.put(new_ids)
-
+            is_stop_after = [s for s in inputs.stop]
+            stop_event = is_stop_before != is_stop_after
+            
+            # setup next step input and cache
             if self.model.config.is_encoder_decoder or self.model.generation_config.use_cache:
                 # print("use cache!")
-                new_ids_tensor = torch.tensor(
-                    new_ids, dtype=torch.long, device=decoder_input_ids.device).unsqueeze(1)
+                dynamic_new_ids = [d for i, d in enumerate(new_ids) if not inputs.is_stop(i)]
+                new_ids_tensor = torch.tensor(dynamic_new_ids, dtype=torch.long, device=decoder_input_ids.device).unsqueeze(1)
                 decoder_input_ids_list = [new_ids_tensor]
             else:
-                decoder_input_ids = inputs(return_attention_mask=False)
+                decoder_input_ids = inputs(return_attention_mask=False, full_batch=False)
                 decoder_input_ids_list = [decoder_input_ids]
+            
+            # shrink encoder_outputs
+            if self.model.config.is_encoder_decoder and stop_event:
+                last_hidden_state = encoder_outputs[0]
+                new_pos = 0
+                for task_i in range(inputs.batch_size):
+                    if inputs.is_stop(task_i):
+                        continue
+                    src_pos = bacth_mapping[task_i]
+                    if src_pos != new_pos:
+                        last_hidden_state[new_pos, ...] = last_hidden_state[src_pos,...]
+                    new_pos += 1
+                last_hidden_state = last_hidden_state[:new_pos,...]
+                encoder_outputs = (last_hidden_state, )
+            
+            # clip cache
+            if stop_event:
+                shrink_past_key_values = []
+                for layer_i, layer in enumerate(past_key_values):
+                    layer_cache = []
+                    for cache_i, cache in enumerate(layer):
+                        new_pos = 0
+                        for task_i in range(inputs.batch_size):
+                            if inputs.is_stop(task_i):
+                                continue
+                            src_pos = bacth_mapping[task_i]
+                            if src_pos != new_pos:
+                                cache[new_pos, ...] = cache[src_pos,...]
+                            new_pos += 1
+                        layer_cache.append(cache[:new_pos,...])
+                    
+                    shrink_past_key_values.append(tuple(layer_cache))
+                past_key_values = tuple(shrink_past_key_values)
+            # clip attention_mask
+            if stop_event:
+                new_pos = 0
+                for task_i in range(inputs.batch_size):
+                    if inputs.is_stop(task_i):
+                        continue
+                    src_pos = bacth_mapping[task_i]
+                    if src_pos != new_pos:
+                        attention_mask[new_pos,...] = attention_mask[src_pos,...]
+                    new_pos += 1
+                attention_mask = attention_mask[:new_pos,...]
+            # update bacth mapping
+            if stop_event:
+                new_pos = 0
+                for task_i in range(inputs.batch_size):
+                    if inputs.is_stop(task_i):
+                        bacth_mapping[task_i] = -1
+                    else:
+                        bacth_mapping[task_i] = new_pos
+                        new_pos += 1
 
             if all(inputs.stop):
                 break
         
         # stop all
         for i in range(inputs.batch_size):
             if not inputs.is_stop(i):
@@ -329,79 +405,99 @@
                  worker: "GenerationModelWorker") -> None:
         self.task_batch = task_batch
         self.tokenizer = tokenizer
         self.worker = worker
         self.stream_interval = worker.stream_interval
 
         self.done = [False for i in range(task_batch.batch_size)]
-
-    def put(self, value):
-        for i in range(self.task_batch.batch_size):
-            generated_len = self.task_batch.get_generated_length(i)
-            if (self.done[i] or generated_len % self.stream_interval != 0) and self.done[i]==self.task_batch.is_stop(i):
-                continue
-            task = self.task_batch.tasks[i]
-
-            token_ids = self.task_batch.get_generated_ids(i)
-
-            # text = self.tokenizer.decode(token_ids, skip_special_tokens=True)
-            tokens = self.tokenizer.convert_ids_to_tokens(token_ids, skip_special_tokens=True)
-            text = self.tokenizer.convert_tokens_to_string(tokens)
-
-            # get offset mapping from token to text
+    
+    @cached(cache=LRUCache(maxsize=8192))
+    def convert_tokens_to_string(self, tokens: List[str]) -> str:
+        return self.tokenizer.convert_tokens_to_string(tokens)
+    
+    def get_text_offset(self, text: str, tokens: List[str]):
+        if self.tokenizer.is_fast:
+            text_offset = [-1] * len(tokens)
+            batch_encoding = self.tokenizer([text])
+            for token_i in range(len(tokens)):
+                span = batch_encoding.token_to_chars(0, token_i)
+                if span is None:
+                    continue
+                start, end = span
+                text_offset[token_i] = start
+        else:
             text_offset = []
             for token_i in range(0, len(tokens)):
                 if token_i == 0:
                     text_offset.append(-1)
                     continue
-                prefix_text = self.tokenizer.convert_tokens_to_string(tokens[:token_i])
+                prefix_text = self.convert_tokens_to_string(tuple(tokens[:token_i]))
                 if text.startswith(prefix_text):
                     text_offset.append(len(prefix_text))
                 else:
                     text_offset.append(-1)
             
             last_id = len(text)
             for token_i in reversed(range(0, len(tokens))):
                 if text_offset[token_i] == -1:
                     text_offset[token_i] = last_id
                 else:
                     last_id = text_offset[token_i]
-            
+        return text_offset
+    
+    def put(self, value):
+        for i in range(self.task_batch.batch_size):
+            generated_len = self.task_batch.get_generated_length(i)
+            if (self.done[i] or generated_len % self.stream_interval != 0) and self.done[i]==self.task_batch.is_stop(i):
+                continue
+            task = self.task_batch.tasks[i]
+
+            token_ids = self.task_batch.get_generated_ids(i)
+
+            text = self.tokenizer.decode(token_ids, skip_special_tokens=False)
+            # text = self.convert_tokens_to_string(tuple(tokens))
+
+            # get logprobs
             token_logprobs = self.task_batch.get_generated_token_probs(i)
             top_logprobs = self.task_batch.get_generated_top_logprobs(i)
             if top_logprobs is not None:
                 top_logprobs_new = []
                 for prob in top_logprobs:
                     top_logprobs_new.append({self.tokenizer.convert_ids_to_tokens(k): v for k, v in prob.items()})
                 top_logprobs = top_logprobs_new
 
             # remove stop words
             stop_pos = stop_by_stopwords(text, 0, task.stop)
             if stop_pos != -1:
-                token_stop_pos = len(tokens)
-                for token_i in reversed(range(0, len(text_offset))):
-                    if text_offset[token_i] < stop_pos:
-                        token_stop_pos = token_i + 1
-                        break
-    
                 self.task_batch.set_stop(i)
 
                 # remove tokens after stop pos
                 text = text[:stop_pos]
-                tokens = tokens[:token_stop_pos]
-                if token_logprobs is not None:
-                    token_logprobs = token_logprobs[:token_stop_pos]
-                if top_logprobs is not None:
-                    top_logprobs = top_logprobs[:token_stop_pos]
-                text_offset = text_offset[:token_stop_pos]
             
             prompt_len = self.task_batch.get_prompt_length(i)
             
             # logprobs
             if self.task_batch.tasks[i].logprobs is not None:
+                tokens = self.tokenizer.convert_ids_to_tokens(token_ids, skip_special_tokens=True)
+                # get offset mapping from token to text
+                text_offset = self.get_text_offset(text, tokens)
+                if stop_pos != -1:
+                    token_stop_pos = len(tokens)
+                    for token_i in reversed(range(0, len(text_offset))):
+                        if text_offset[token_i] < stop_pos:
+                            token_stop_pos = token_i + 1
+                            break
+                    # remove tokens after stop pos
+                    tokens = tokens[:token_stop_pos]
+                    if token_logprobs is not None:
+                        token_logprobs = token_logprobs[:token_stop_pos]
+                    if top_logprobs is not None:
+                        top_logprobs = top_logprobs[:token_stop_pos]
+                    text_offset = text_offset[:token_stop_pos]
+
                 logprobs = GenerationWorkerLogprobs(
                     tokens=tokens,
                     token_logprobs=token_logprobs,
                     top_logprobs=top_logprobs,
                     text_offset=text_offset,
                 )
             else:
@@ -476,57 +572,80 @@
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
         quantization: Optional[str],
         cpu_offloading: bool,
         deepspeed: bool = False,
-        trust_remote_code: bool = False
+        trust_remote_code: bool = False,
+        offload_folder: Optional[str] = None,
     ) -> None:
         super(HuggingfaceGenerationExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device=device,
             num_gpus=num_gpus,
             max_gpu_memory=max_gpu_memory,
             quantization=quantization,
             cpu_offloading=cpu_offloading
         )
         self.adapter = None
         self.model = None
         self.tokenizer = None
         self.adapter, self.model, self.tokenizer = self.load_model(
-            model_path, device, num_gpus, max_gpu_memory, quantization, cpu_offloading, deepspeed, trust_remote_code
+            model_path, device, num_gpus, max_gpu_memory, quantization, cpu_offloading, deepspeed, trust_remote_code, offload_folder
         )
 
         # self.model = torch.compile(self.model)
 
         if hasattr(self.model.config, "max_sequence_length"):
             self._context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self._context_len = self.model.config.max_position_embeddings
         else:
             self._context_len = 2048
+        
+        self.current_batch = 2
 
     @property
     def context_length(self) -> int:
         return self._context_len
     
     def tokenize(self, text: str) -> List[int]:
         input_ids = self.tokenizer(text).input_ids
         return input_ids
     
     def inference(self, worker: "GenerationModelWorker"):
         if not worker.online:
             return
 
-        tasks = worker.fetch_tasks()
+        tasks = worker.fetch_tasks(task_num=self.current_batch)
 
+        if len(tasks) == 0:
+            return
+        
         # batch inference
+        tasks = sorted(tasks, key=lambda x:len(x.prompt), reverse=True)
         inputs = BatchingTask(tasks, self.tokenizer, self.device, self.model.config.is_encoder_decoder)
-        if inputs.batch_size == 0:
-            return
+        
+        if torch.cuda.is_available() and "cuda" in self.device:
+            if self.device == "cuda":
+                device = "cuda:0"
+            else:
+                device = self.device
+            free_mem, total_mem = torch.cuda.mem_get_info(device)
+            if free_mem < total_mem * 0.3:
+                new_batch = self.current_batch * 2
+            elif free_mem < total_mem * 0.8:
+                new_batch = self.current_batch + 1
+            elif free_mem > total_mem * 0.95:
+                new_batch = self.current_batch - 1
+            if len(tasks) == self.current_batch:
+                self.current_batch = new_batch
+        else:
+            self.current_batch = worker.max_batch
+
         streamer = GenerationWorkerStreamer(inputs, self.tokenizer, worker)
         model = GenerationModel(self.model)
         max_new_tokens = max(inputs.max_tokens)
         model.generate(inputs, max_new_tokens, streamer)
```

### Comparing `langport-0.3.2/langport/model/executor/generation/optimum.py` & `langport-0.3.3/langport/model/executor/generation/optimum.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/ggml.py` & `langport-0.3.3/langport/model/executor/ggml.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/executor/huggingface.py` & `langport-0.3.3/langport/model/executor/huggingface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from functools import partial
 from typing import Optional
 
 from langport.model.adapters.dolly_v2 import DollyV2Adapter
+from langport.model.adapters.openbuddy import OpenBuddyAdapter
+from langport.model.adapters.qwen import QwenAdapter
 from langport.model.adapters.rwkv import RwkvAdapter
 from langport.model.adapters.t5 import T5Adapter
 from langport.model.adapters.text2vec import BertAdapter
 from langport.model.adapters.chatglm import ChatGLMAdapter
 
 from langport.model.executor.base import LocalModelExecutor
 
@@ -24,15 +27,14 @@
 import math
 from typing import Optional
 import warnings
 import psutil
 
 import torch
 from langport.model.compression import load_compress_model, default_compression_config, bit4_compression_config
-from langport.model.svd import load_svd_model
 from langport.model.executor.base import BaseModelExecutor
 from langport.model.model_adapter import get_model_adapter, raise_warning_for_incompatible_cpu_offloading_configuration
 from langport.model.monkey_patch_non_inplace import replace_llama_attn_with_non_inplace_operations
 from langport.utils import get_gpu_memory
 
 
 
@@ -84,17 +86,31 @@
         elif isinstance(adapter, ChatGLMAdapter):
             tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False, trust_remote_code=True)
             if "trust_remote_code" in from_pretrained_kwargs:
                 from_pretrained_kwargs.pop("trust_remote_code")
             model = AutoModel.from_pretrained(
                 model_path, low_cpu_mem_usage=True, trust_remote_code=True, **from_pretrained_kwargs
             )
+        elif isinstance(adapter, QwenAdapter):
+            trust_remote_code = from_pretrained_kwargs.get("trust_remote_code", False)
+            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True, trust_remote_code=trust_remote_code)
+            model = AutoModelForCausalLM.from_pretrained(
+                model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
+            )
+            # allowed_special work around
+            tokenizer.tokenize = partial(tokenizer.tokenize, allowed_special="all")
+        elif isinstance(adapter, OpenBuddyAdapter):
+            trust_remote_code = from_pretrained_kwargs.get("trust_remote_code", False)
+            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True, trust_remote_code=trust_remote_code)
+            model = AutoModelForCausalLM.from_pretrained(
+                model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
+            ) # , offload_folder="offload"
         else:
             trust_remote_code = from_pretrained_kwargs.get("trust_remote_code", False)
-            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False, trust_remote_code=trust_remote_code)
+            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True, trust_remote_code=trust_remote_code)
             model = AutoModelForCausalLM.from_pretrained(
                 model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
             )
 
         return model, tokenizer
 
     def load_model(
@@ -103,14 +119,15 @@
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str] = None,
         quantization: Optional[str] = None,
         cpu_offloading: bool = False,
         deepspeed: bool = False,
         trust_remote_code: bool = False,
+        offload_folder: Optional[str] = None,
         debug: bool = False,
     ):
         """Load a model from Hugging Face."""
         adapter = get_model_adapter(model_path)
 
         # Handle device mapping
         cpu_offloading = raise_warning_for_incompatible_cpu_offloading_configuration(
@@ -137,14 +154,15 @@
             kwargs = {"torch_dtype": torch.float16}
             # Avoid bugs in mps backend by not using in-place operations.
             replace_llama_attn_with_non_inplace_operations()
         else:
             raise ValueError(f"Invalid device: {device}")
 
         kwargs["trust_remote_code"] = trust_remote_code
+        kwargs["offload_folder"] = offload_folder
 
         if cpu_offloading:
             # raises an error on incompatible platforms
             from transformers import BitsAndBytesConfig
 
             if "max_memory" in kwargs:
                 kwargs["max_memory"]["cpu"] = (
```

### Comparing `langport-0.3.2/langport/model/executor/optimum.py` & `langport-0.3.3/langport/model/executor/optimum.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/model_adapter.py` & `langport-0.3.3/langport/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/model_args.py` & `langport-0.3.3/langport/model/model_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,25 @@
     parser.add_argument(
         "--load-8bit", action="store_true", help="Use 8-bit quantization"
     )
     parser.add_argument(
         "--load-4bit", action="store_true", help="Use 4-bit quantization"
     )
     parser.add_argument(
-        "--svd", action="store_true", help="Use SVD"
-    )
-    parser.add_argument(
         "--cpu-offloading",
         action="store_true",
         help="Only when using 8-bit quantization: Offload excess weights to the CPU that don't fit on the GPU",
     )
     parser.add_argument(
+        "--offload-folder",
+        type=str, default=None,
+        help="If the device_map contains any value \"disk\", the folder where we will offload weights",
+    )
+    parser.add_argument(
         "--deepspeed", action="store_true", help="Use deepspeed"
     )
     parser.add_argument(
         "--trust-remote-code", action="store_true", help="Trust remote code"
+    )
+    parser.add_argument(
+        "--sleep", type=int, default=0, help="Sleep after seconds"
     )
```

### Comparing `langport-0.3.2/langport/model/models/rwkv_model.py` & `langport-0.3.3/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/model/monkey_patch_non_inplace.py` & `langport-0.3.3/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/protocol/huggingface_api_protocol.py` & `langport-0.3.3/langport/protocol/huggingface_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/protocol/openai_api_protocol.py` & `langport-0.3.3/langport/protocol/openai_api_protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,25 +40,45 @@
     data: List[ModelCard] = []
 
 class UsageInfo(BaseModel):
     prompt_tokens: int = 0
     total_tokens: int = 0
     completion_tokens: Optional[int] = 0
 
+class FunctionProperty(BaseModel):
+    type: str
+    description: Optional[str]
+    enum: Optional[List[str]]
+
+class FunctionParameters(BaseModel):
+    type: str
+    properties: Dict[str, FunctionProperty]
+    required: List[str]
+
+class FunctionDefinition(BaseModel):
+    name: str
+    description: Optional[str]
+    parameters: FunctionParameters
+
+class FunctionEntry(BaseModel):
+    name: str
+
 class ChatCompletionRequest(BaseModel):
     model: str
     messages: List[Dict[str, str]]
     temperature: Optional[float] = 0.7
     top_p: Optional[float] = 1.0
     n: Optional[int] = 1
     max_tokens: Optional[int] = None
     stop: Optional[Union[str, List[str]]] = None
     stream: Optional[bool] = False
     presence_penalty: Optional[float] = 0.0
     frequency_penalty: Optional[float] = 0.0
+    functions: Optional[List[FunctionDefinition]]
+    function_call: Optional[Union[Literal["none", "auto"], FunctionEntry]]
     user: Optional[str] = None
 
 
 class ChatMessage(BaseModel):
     role: str
     content: str
```

### Comparing `langport-0.3.2/langport/protocol/tabby_api_protocol.py` & `langport-0.3.3/langport/protocol/tabby_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/protocol/worker_protocol.py` & `langport-0.3.3/langport/protocol/worker_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/routers/gateway/common.py` & `langport-0.3.3/langport/routers/gateway/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,15 +115,16 @@
         return []
     response = WorkerAddressResponse.parse_obj(ret.json())
     
     address_list = response.address_list
     models = [json.loads(obj) for obj in response.values]
     # No available worker
     if address_list == []:
-        raise ValueError(f"No available worker for feature {feature}")
+        # raise ValueError(f"No available worker for feature {feature}")
+        return []
 
     return models
 
 async def check_model(app_settings: AppSettings, request, feature: str, model_name: str) -> Optional[JSONResponse]:
     ret = None
     async with httpx.AsyncClient() as client:
         try:
@@ -176,10 +177,30 @@
     if request.stop is not None and (
         not isinstance(request.stop, str) and not isinstance(request.stop, list)
     ):
         return create_error_response(
             ErrorCode.PARAM_OUT_OF_RANGE,
             f"{request.stop} is not valid under any of the given schemas - 'stop'",
         )
+    if request.presence_penalty is not None and request.presence_penalty < -2.0:
+        return create_error_response(
+            ErrorCode.PARAM_OUT_OF_RANGE,
+            f"{request.presence_penalty} is less than the minimum of -2.0 - 'presence_penalty'",
+        )
+    if request.presence_penalty is not None and request.presence_penalty > 2.0:
+        return create_error_response(
+            ErrorCode.PARAM_OUT_OF_RANGE,
+            f"{request.presence_penalty} is less than the maximum of 2.0 - 'presence_penalty'",
+        )
+    if request.frequency_penalty is not None and request.frequency_penalty < -2.0:
+        return create_error_response(
+            ErrorCode.PARAM_OUT_OF_RANGE,
+            f"{request.frequency_penalty} is less than the minimum of -2.0 - 'frequency_penalty'",
+        )
+    if request.frequency_penalty is not None and request.frequency_penalty > 2.0:
+        return create_error_response(
+            ErrorCode.PARAM_OUT_OF_RANGE,
+            f"{request.frequency_penalty} is less than the maximum of 2.0 - 'frequency_penalty'",
+        )
 
     return None
```

### Comparing `langport-0.3.2/langport/routers/gateway/openai_compatible.py` & `langport-0.3.3/langport/routers/gateway/openai_compatible.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 
 import asyncio
 import json
 
-from typing import Generator, Optional, Union, Dict, List, Any
+from typing import Coroutine, Generator, Optional, Union, Dict, List, Any
 
 from fastapi.responses import StreamingResponse
 import httpx
 import shortuuid
 
 from langport.constants import WORKER_API_TIMEOUT, ErrorCode
 from langport.model.model_adapter import get_conversation_template
@@ -37,33 +37,50 @@
     BaseWorkerResult,
     EmbeddingWorkerResult,
     GenerationWorkerResult,
 )
 from langport.core.dispatch import DispatchMethod
 from langport.routers.gateway.common import LANGPORT_HEADER, AppSettings, _get_worker_address, _list_models, check_model, check_requests, create_error_response
 
+def clean_system_prompts(messages: List[Dict[str, str]]):
+    system_prompt = ""
+    result = []
+    for i, message in enumerate(messages):
+        if i != 0 and message["role"] == "system":
+            system_prompt += message["content"] + "\n"
+            continue
+        result.append(message)
+    system_prompt = system_prompt.rstrip("\n")
+    if len(messages) > 0 and messages[0]["role"] == "system":
+        messages[0]["content"] += "\n" + system_prompt
+    else:
+        messages.insert(0, {"role": "system", "content": system_prompt})
+    return result
 
 def get_gen_params(
     model_name: str,
     messages: Union[str, List[Dict[str, str]]],
     *,
     temperature: float,
     top_p: float,
     max_tokens: Optional[int],
     echo: Optional[bool],
     stream: Optional[bool],
     stop: Optional[Union[str, List[str]]],
     logprobs: Optional[int]=None,
+    presence_penalty: Optional[float]=0.0,
+    frequency_penalty: Optional[float]=0.0,
 ) -> Dict[str, Any]:
     # is_chatglm = "chatglm" in model_name.lower()
     conv = get_conversation_template(model_name)
 
     if isinstance(messages, str):
         prompt = messages
     else:
+        messages = clean_system_prompts(messages)
         for message in messages:
             msg_role = message["role"]
             if msg_role == "system":
                 conv.system = message["content"]
             elif msg_role == "user":
                 conv.append_message(conv.settings.roles[0], message["content"])
             elif msg_role == "assistant":
@@ -94,20 +111,28 @@
         gen_params.update(
             {"stop": conv.settings.stop_str}
         )
     elif isinstance(stop, str):
         gen_params.update({"stop": [stop, conv.settings.stop_str]})
     else:
         gen_params.update({"stop": stop + [conv.settings.stop_str]})
+    
+    if presence_penalty is not None:
+        gen_params["presence_penalty"] = presence_penalty
+    if frequency_penalty is not None:
+        gen_params["frequency_penalty"] = frequency_penalty
 
     return gen_params
 
 async def api_models(app_settings: AppSettings):
     async with httpx.AsyncClient() as client:
-        models = await _list_models(app_settings, None, client)
+        generation_models = await _list_models(app_settings, "generation", client)
+    async with httpx.AsyncClient() as client:
+        embedding_models = await _list_models(app_settings, "embedding", client)
+    models = generation_models + embedding_models
     models.sort()
     # TODO: return real model permission details
     model_cards = []
     for m in models:
         model_cards.append(ModelCard(id=m, root=m, permission=[ModelPermission()]))
     return ModelList(data=model_cards)
 
@@ -369,14 +394,16 @@
         temperature=request.temperature,
         top_p=request.top_p,
         max_tokens=request.max_tokens,
         echo=request.echo,
         stream=request.stream,
         stop=request.stop,
         logprobs=request.logprobs,
+        presence_penalty=request.presence_penalty,
+        frequency_penalty=request.frequency_penalty,
     )
 
     if request.stream:
         return await completions_stream(app_settings, payload, request)
     else:
         return await completions_non_stream(app_settings, payload, request)
 
@@ -395,14 +422,16 @@
         request.messages,
         temperature=request.temperature,
         top_p=request.top_p,
         max_tokens=request.max_tokens,
         echo=False,
         stream=request.stream,
         stop=request.stop,
+        presence_penalty=request.presence_penalty,
+        frequency_penalty=request.frequency_penalty,
     )
     if request.stream:
         return await chat_completions_stream(app_settings, payload, request)
     else:
         return await chat_completions_non_stream(app_settings, payload, request)
 
 async def api_embeddings(app_settings: AppSettings, request: EmbeddingsRequest):
```

### Comparing `langport-0.3.2/langport/routers/server/core_node.py` & `langport-0.3.3/langport/routers/server/core_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/routers/server/embedding_node.py` & `langport-0.3.3/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/routers/server/generation_node.py` & `langport-0.3.3/langport/routers/server/generation_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 @app.post("/completion_stream")
 async def api_completion_stream(request: Request):
     params = await request.json()
     await app.node.acquire_model_semaphore()
     generator = app.node.generation_bytes_stream(GenerationTask(
         prompt=params["prompt"],
         temperature=params.get("temperature", 1.0),
-        repetition_penalty=params.get("repetition_penalty", 0.0),
+        repetition_penalty=params.get("presence_penalty", 0.0),
         top_p=params.get("top_p", 1.0),
         top_k=params.get("top_k", 1),
         max_tokens=params.get("max_tokens", 512),
         stop=params.get("stop", None),
         echo=params.get("echo", False),
         stop_token_ids=params.get("stop_token_ids", None),
         logprobs=params.get("logprobs", None),
@@ -69,15 +69,15 @@
 @app.post("/completion")
 async def api_completion(request: Request):
     params = await request.json()
     await app.node.acquire_model_semaphore()
     generator = await app.node.generation_stream(GenerationTask(
         prompt=params["prompt"],
         temperature=params.get("temperature", 1.0),
-        repetition_penalty=params.get("repetition_penalty", 0.0),
+        repetition_penalty=params.get("presence_penalty", 0.0),
         top_p=params.get("top_p", 1.0),
         top_k=params.get("top_k", 1),
         max_tokens=params.get("max_tokens", 512),
         stop=params.get("stop", None),
         echo=params.get("echo", False),
         stop_token_ids=params.get("stop_token_ids", None),
         logprobs=params.get("logprobs", None),
```

### Comparing `langport-0.3.2/langport/service/gateway/cluster_monitor.py` & `langport-0.3.3/langport/service/gateway/cluster_monitor.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/gateway/cluster_monitor_app.py` & `langport-0.3.3/langport/service/gateway/cluster_monitor_app.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/gateway/fauxpilot_api.py` & `langport-0.3.3/langport/service/gateway/fauxpilot_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/gateway/graphite_feeder.py` & `langport-0.3.3/langport/service/gateway/graphite_feeder.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/gateway/huggingface_api.py` & `langport-0.3.3/langport/service/gateway/huggingface_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         OpenAICompletionRequest(
             model=app.model_name,
             prompt=request.inputs,
             n=N,
         )
     )
     if isinstance(response, JSONResponse):
-        print(response.body)
         return Response(generated_text="", details=Details(
             finish_reason=FinishReason.EndOfSequenceToken,
             generated_tokens=0,
         ))
 
     # print(response.choices[0].text.replace("\n", "\\n"))
     return Response(generated_text=response.choices[0].text,
```

### Comparing `langport-0.3.2/langport/service/gateway/openai_api.py` & `langport-0.3.3/langport/service/gateway/openai_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import argparse
+import datetime
 import json
 import logging
+import os
 
 from typing import Optional
 
 import fastapi
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse
 from starlette.middleware.base import BaseHTTPMiddleware, DispatchFunction
 from starlette.types import ASGIApp
 import uvicorn
 
-from langport.constants import ErrorCode
+from langport.constants import LOGDIR, ErrorCode
 from fastapi.exceptions import RequestValidationError
 from langport.protocol.openai_api_protocol import (
     ChatCompletionRequest,
     CompletionRequest,
     EmbeddingsRequest,
 )
 from langport.routers.gateway.common import AppSettings, create_error_response
 from langport.routers.gateway.openai_compatible import api_chat_completions, api_completions, api_embeddings, api_models
+from langport.utils import build_logger
 
-logger = logging.getLogger(__name__)
-
+current_time = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+logger = build_logger("openai_api", f"openai_api_{current_time}.log")
 app = fastapi.FastAPI(debug=False)
 
 class BaseAuthorizationMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, sk:str, dispatch: Optional[DispatchFunction] = None) -> None:
         super().__init__(app, dispatch)
         self.sk = sk
 
@@ -65,26 +68,31 @@
 async def models():
     return await api_models(app.app_settings)
 
 
 @app.post("/v1/chat/completions")
 async def chat_completions(request: ChatCompletionRequest):
     request.model = redirect_model_name(request.model)
-    return await api_chat_completions(app.app_settings, request)
+    response = await api_chat_completions(app.app_settings, request)
+    logger.info(request.json())
+    return response
 
 @app.post("/v1/completions")
 async def completions(request: CompletionRequest):
     request.model = redirect_model_name(request.model)
-    return await api_completions(app.app_settings, request)
+    response = await api_completions(app.app_settings, request)
+    logger.info(request.json())
+    return response
 
 
 @app.post("/v1/embeddings")
 async def embeddings(request: EmbeddingsRequest):
     request.model = redirect_model_name(request.model)
-    return await api_embeddings(app.app_settings, request)
+    response = await api_embeddings(app.app_settings, request)
+    return response
 
 
 if __name__ in ["__main__", "langport.service.gateway.openai_api"]:
     parser = argparse.ArgumentParser(
         description="Langport openai-compatible RESTful API server."
     )
     parser.add_argument("--host", type=str, default="localhost", help="host name")
```

### Comparing `langport-0.3.2/langport/service/gateway/tabby_api.py` & `langport-0.3.3/langport/service/gateway/tabby_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/server/chatgpt_generation_worker.py` & `langport-0.3.3/langport/service/server/chatgpt_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/server/dummy_worker.py` & `langport-0.3.3/langport/service/server/dummy_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/server/embedding_worker.py` & `langport-0.3.3/langport/service/server/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/server/generation_worker.py` & `langport-0.3.3/langport/service/server/generation_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=None)
     parser.add_argument("--worker-address", type=str, default=None)
     parser.add_argument("--neighbors", type=str, nargs="*", default=[])
 
     add_model_args(parser)
     parser.add_argument("--model-name", type=str, help="Optional display name")
-    parser.add_argument("--limit-model-concurrency", type=int, default=8)
-    parser.add_argument("--batch", type=int, default=4)
+    parser.add_argument("--limit-model-concurrency", type=int, default=4)
+    parser.add_argument("--batch", type=int, default=8)
     parser.add_argument("--stream-interval", type=int, default=2)
     args = parser.parse_args()
 
     node_id = str(uuid.uuid4())
     logger = build_logger("generation_worker", f"generation_worker_{node_id}.log")
     logger.info(f"args: {args}")
 
@@ -58,15 +58,16 @@
         model_path=args.model_path,
         device=args.device,
         num_gpus=args.num_gpus,
         max_gpu_memory=args.max_gpu_memory,
         quantization=quantization,
         cpu_offloading=args.cpu_offloading,
         deepspeed=args.deepspeed,
-        trust_remote_code=args.trust_remote_code
+        trust_remote_code=args.trust_remote_code,
+        offload_folder=args.offload_folder,
     )
     
     app.node = GenerationModelWorker(
         node_addr=args.worker_address,
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         executor=executor,
```

### Comparing `langport-0.3.2/langport/service/server/ggml_generation_worker.py` & `langport-0.3.3/langport/service/server/ggml_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/service/server/optimum_generation_worker.py` & `langport-0.3.3/langport/service/server/optimum_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/utils/__init__.py` & `langport-0.3.3/langport/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/utils/evaluation.py` & `langport-0.3.3/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/utils/http_pool.py` & `langport-0.3.3/langport/utils/http_pool.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/utils/interval_timer.py` & `langport-0.3.3/langport/utils/interval_timer.py`

 * *Files identical despite different names*

### Comparing `langport-0.3.2/langport/workers/embedding_worker.py` & `langport-0.3.3/langport/workers/embedding_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             init_neighborhoods_addr=init_neighborhoods_addr,
             limit_model_concurrency=limit_model_concurrency,
             max_batch=max_batch,
             stream_interval=stream_interval,
             logger=logger,
         )
         self.executor = executor
-        workers = max(1, 2 * self.limit_model_concurrency // self.max_batch)
+        workers = max(1, self.limit_model_concurrency)
         self.add_timer(
             "embeddings_inference", 
             EMBEDDING_INFERENCE_INTERVAL, 
             executor.inference, 
             args=(self,), 
             kwargs=None, 
             workers=workers
```

### Comparing `langport-0.3.2/langport/workers/generation_worker.py` & `langport-0.3.3/langport/workers/generation_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     GENERATION_INFERENCE_INTERVAL,
     WORKER_API_TIMEOUT,
     WORKER_HEART_BEAT_INTERVAL,
     ErrorCode,
 )
 from langport.utils import server_error_msg, pretty_print_semaphore
 
-
 class GenerationModelWorker(ClusterWorker):
     def __init__(
         self,
         node_addr: str,
         node_id: str,
         init_neighborhoods_addr: List[str],
         executor: GenerationExecutor,
@@ -38,15 +37,15 @@
             init_neighborhoods_addr=init_neighborhoods_addr,
             limit_model_concurrency=limit_model_concurrency,
             max_batch=max_batch,
             stream_interval=stream_interval,
             logger=logger,
         )
         self.executor = executor
-        workers = max(1, 2 * self.limit_model_concurrency // self.max_batch)
+        workers = max(1, self.limit_model_concurrency)
         self.add_timer(
             "generation_inference",
             GENERATION_INFERENCE_INTERVAL,
             self.executor.inference,
             args=[self,],
             kwargs=None,
             workers=workers,
```

### Comparing `langport-0.3.2/langport.egg-info/PKG-INFO` & `langport-0.3.3/langport.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.3.2
+Version: 0.3.3
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -55,14 +55,15 @@
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
 ## News
+- [2023/08/04] Dynamic batch inference.
 - [2023/07/16] Support int4 quantization.
 - [2023/07/13] Support generation logprobs parameter.
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
@@ -147,14 +148,20 @@
 
 Run text generation with ggml worker:
 
 ```bash
 python -m langport.service.server.ggml_generation_worker --port 21001 --model-path <your model path> --gpu-layers <num layer to gpu (resize this for your VRAM)>
 ```
 
+Run OpenAI forward server: 
+```bash
+python -m langport.service.server.chatgpt_generation_worker --port 21001 --api-url <url> --api-key <key>
+```
+
+
 ## License
 
 langport is released under the Apache Software License.
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langport Version: 0.3.2 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.3.3 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
 Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
@@ -22,30 +22,30 @@
 Tested Models * NingYu, LLaMa, LLaMa2-chat, Vicuna, ChatGLM, ChatGLM2, Falcon,
 Starcoder, WizardLM, InternLM, OpenBuddy, FireFly, CodeGen, Phoenix, RWKV,
 StableLM and so on. ## Benchmark We use single RTX3090 to run a finetuned 7B
 LLaMA model (OpenBuddy V0.9) under the bf16 setting. We create 32 threads to
 submit chat tasks to the server, and the following figure shows the Queries Per
 Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with
 different max model concurrency settings. ![benchmark_chat](assets/
-benchmark_chat.jpg) ## News - [2023/07/16] Support int4 quantization. - [2023/
-07/13] Support generation logprobs parameter. - [2023/06/18] Add ggml
-(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
-LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
-support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
-06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
-[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
-supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
-With pip ```bash pip install langport ``` or: ```bash pip install git+https://
-github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
-this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
-```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
-Clone this repository ```bash git clone https://github.com/vtuber-plan/
-langport.git cd langport ``` 2. Install the Package ```bash pip install --
-upgrade pip pip install -e . ``` ## Start the server It is simple to start a
-single node chat API service: ``` bash python -
+benchmark_chat.jpg) ## News - [2023/08/04] Dynamic batch inference. - [2023/07/
+16] Support int4 quantization. - [2023/07/13] Support generation logprobs
+parameter. - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.)
+worker support. - [2023/06/09] Add LLama.cpp worker support. - [2023/06/01] Add
+HuggingFace Bert embedding worker support. - [2023/06/01] Add HuggingFace text
+generation API support. - [2023/06/01] Add tabby API support. - [2023/05/23]
+Add chat throughput test script. - [2023/05/22] New distributed architecture. -
+[2023/05/14] Batch inference supported. - [2023/05/10] Langport project
+started. ## Install ### Method 1: With pip ```bash pip install langport ``` or:
+```bash pip install git+https://github.com/vtuber-plan/langport.git ``` If you
+need ggml generation worker, use this command: ```bash pip install langport
+[ggml] ``` If you wanna use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml]
+``` ### Method 2: From source 1. Clone this repository ```bash git clone https:
+//github.com/vtuber-plan/langport.git cd langport ``` 2. Install the Package
+```bash pip install --upgrade pip pip install -e . ``` ## Start the server It
+is simple to start a single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
 localhost:21001 python -m langport.service.server.embedding_worker --model-path
 --neighbors http://localhost:21001 python -
@@ -65,13 +65,14 @@
 controller-address http://localhost:21002 # Any worker is also OK! ``` Run text
 generation with multi GPUs: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  --gpus
 0,1 --num-gpus 2 python -m langport.service.gateway.openai_api ``` Run text
 generation with ggml worker: ```bash python -
 m langport.service.server.ggml_generation_worker --port 21001 --model-path  --
 gpu-layers
-resize this for your VRAM)> ``` ## License langport is released under the
-Apache Software License. ## See also - [langport-docs](https://github.com/
-vtuber-plan/langport/tree/main/docs) - [langport-source](https://github.com/
-vtuber-plan/langport) ## Star History [![Star History Chart](https://api.star-
-history.com/svg?repos=vtuber-plan/langport&type=Date)](https://star-
-history.com/#vtuber-plan/langport&Date)
+resize this for your VRAM)> ``` Run OpenAI forward server: ```bash python -
+m langport.service.server.chatgpt_generation_worker --port 21001 --api-url  --
+api-key  ``` ## License langport is released under the Apache Software License.
+## See also - [langport-docs](https://github.com/vtuber-plan/langport/tree/
+main/docs) - [langport-source](https://github.com/vtuber-plan/langport) ## Star
+History [![Star History Chart](https://api.star-history.com/svg?repos=vtuber-
+plan/langport&type=Date)](https://star-history.com/#vtuber-plan/langport&Date)
```

### Comparing `langport-0.3.2/langport.egg-info/SOURCES.txt` & `langport-0.3.3/langport.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 langport/data/conversation/settings/llama.py
 langport/data/conversation/settings/mpt.py
 langport/data/conversation/settings/ningyu.py
 langport/data/conversation/settings/oasst_pythia.py
 langport/data/conversation/settings/one_shot.py
 langport/data/conversation/settings/openbuddy.py
 langport/data/conversation/settings/phoenix.py
+langport/data/conversation/settings/qwen.py
 langport/data/conversation/settings/redpajama.py
 langport/data/conversation/settings/rwkv.py
 langport/data/conversation/settings/stablelm.py
 langport/data/conversation/settings/vicuna.py
 langport/data/conversation/settings/wizardlm.py
 langport/data/conversation/settings/zero_shot.py
 langport/model/__init__.py
 langport/model/compression.py
 langport/model/model_adapter.py
 langport/model/model_args.py
 langport/model/monkey_patch_non_inplace.py
-langport/model/svd.py
 langport/model/adapters/__init__.py
 langport/model/adapters/baichuan.py
 langport/model/adapters/baize.py
 langport/model/adapters/bard.py
 langport/model/adapters/billa.py
 langport/model/adapters/changgpt.py
 langport/model/adapters/chatglm.py
@@ -66,14 +66,15 @@
 langport/model/adapters/koala.py
 langport/model/adapters/llama.py
 langport/model/adapters/longchat.py
 langport/model/adapters/ningyu.py
 langport/model/adapters/oasst_pythia.py
 langport/model/adapters/openbuddy.py
 langport/model/adapters/phoenix.py
+langport/model/adapters/qwen.py
 langport/model/adapters/robin.py
 langport/model/adapters/rwkv.py
 langport/model/adapters/snoozy.py
 langport/model/adapters/stable_lm.py
 langport/model/adapters/starcoder.py
 langport/model/adapters/t5.py
 langport/model/adapters/text2vec.py
@@ -120,14 +121,15 @@
 langport/service/server/chatgpt_generation_worker.py
 langport/service/server/dummy_worker.py
 langport/service/server/embedding_worker.py
 langport/service/server/generation_worker.py
 langport/service/server/ggml_generation_worker.py
 langport/service/server/optimum_generation_worker.py
 langport/utils/__init__.py
+langport/utils/cache.py
 langport/utils/cache_state.py
 langport/utils/evaluation.py
 langport/utils/http_pool.py
 langport/utils/interval_timer.py
 langport/workers/__init__.py
 langport/workers/embedding_worker.py
 langport/workers/generation_worker.py
```

### Comparing `langport-0.3.2/pyproject.toml` & `langport-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.3.2"
+version = "0.3.3"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

