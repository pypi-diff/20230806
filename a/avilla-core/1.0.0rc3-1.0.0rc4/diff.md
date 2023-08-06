# Comparing `tmp/avilla-core-1.0.0rc3.tar.gz` & `tmp/avilla-core-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla-core-1.0.0rc3.tar", last modified: Sun Aug  7 08:07:36 2022, max compression
+gzip compressed data, was "avilla-core-1.0.0rc4.tar", last modified: Wed Aug 31 04:40:23 2022, max compression
```

## Comparing `avilla-core-1.0.0rc3.tar` & `avilla-core-1.0.0rc4.tar`

### file list

```diff
@@ -1,45 +1,52 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     6469 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/action/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/action/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/application.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/builtins/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/event/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/event/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/event/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/event/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/message.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/metadata/cells.py
--rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/metadata/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/querier.py
--rw-r--r--   0 runner    (1001) docker     (121)    16041 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/relationship.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/resource/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/service.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5262 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/tools/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/action_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/event_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/message_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4525 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/metadata_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     8278 2022-08-07 08:07:22.179967 avilla-core-1.0.0rc3/avilla/core/utilles/selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-08-07 08:07:22.183967 avilla-core-1.0.0rc3/pyproject.toml
--rw-------   0 runner    (1001) docker     (121)     6387 2022-08-07 08:07:36.785258 avilla-core-1.0.0rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     5093 2022-08-31 04:32:04.243299 avilla-core-1.0.0rc4/avilla/core/__init__.py
+-rw-rw-rw-   0        0        0     1615 2022-08-31 04:32:04.245252 avilla-core-1.0.0rc4/avilla/core/account.py
+-rw-rw-rw-   0        0        0     7073 2022-08-31 04:32:04.246228 avilla-core-1.0.0rc4/avilla/core/application.py
+-rw-rw-rw-   0        0        0        0 2022-08-31 04:32:04.249165 avilla-core-1.0.0rc4/avilla/core/builtins/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-08-31 04:32:04.250135 avilla-core-1.0.0rc4/avilla/core/builtins/extension.py
+-rw-rw-rw-   0        0        0     4123 2022-08-31 04:32:04.251118 avilla-core-1.0.0rc4/avilla/core/cell/__init__.py
+-rw-rw-rw-   0        0        0      996 2022-08-31 04:32:04.252088 avilla-core-1.0.0rc4/avilla/core/cell/cells.py
+-rw-rw-rw-   0        0        0     1608 2022-08-31 04:32:04.254041 avilla-core-1.0.0rc4/avilla/core/context.py
+-rw-rw-rw-   0        0        0     2906 2022-08-31 04:32:04.255020 avilla-core-1.0.0rc4/avilla/core/dispatchers.py
+-rw-rw-rw-   0        0        0     2560 2022-08-31 04:32:04.256971 avilla-core-1.0.0rc4/avilla/core/elements.py
+-rw-rw-rw-   0        0        0     2640 2022-08-31 04:32:04.258925 avilla-core-1.0.0rc4/avilla/core/event/__init__.py
+-rw-rw-rw-   0        0        0      727 2022-08-31 04:32:04.260877 avilla-core-1.0.0rc4/avilla/core/event/activity.py
+-rw-rw-rw-   0        0        0     1950 2022-08-31 04:32:04.261855 avilla-core-1.0.0rc4/avilla/core/event/lifecycle.py
+-rw-rw-rw-   0        0        0     2752 2022-08-31 04:32:04.263810 avilla-core-1.0.0rc4/avilla/core/event/message.py
+-rw-rw-rw-   0        0        0     1239 2022-08-31 04:32:04.264785 avilla-core-1.0.0rc4/avilla/core/event/request.py
+-rw-rw-rw-   0        0        0     1919 2022-08-31 04:32:04.266738 avilla-core-1.0.0rc4/avilla/core/event/resource.py
+-rw-rw-rw-   0        0        0     1388 2022-08-31 04:32:04.267714 avilla-core-1.0.0rc4/avilla/core/exceptions.py
+-rw-rw-rw-   0        0        0      726 2022-08-31 04:32:04.269668 avilla-core-1.0.0rc4/avilla/core/message.py
+-rw-rw-rw-   0        0        0     1232 2022-08-31 04:32:04.270645 avilla-core-1.0.0rc4/avilla/core/platform.py
+-rw-rw-rw-   0        0        0     3060 2022-08-31 04:32:04.272605 avilla-core-1.0.0rc4/avilla/core/protocol.py
+-rw-rw-rw-   0        0        0        0 2022-02-26 15:50:19.540808 avilla-core-1.0.0rc4/avilla/core/py.typed
+-rw-rw-rw-   0        0        0     1692 2022-08-31 04:32:04.273575 avilla-core-1.0.0rc4/avilla/core/querier.py
+-rw-rw-rw-   0        0        0    13224 2022-08-31 04:32:04.276004 avilla-core-1.0.0rc4/avilla/core/relationship.py
+-rw-rw-rw-   0        0        0     1395 2022-08-31 04:32:04.277477 avilla-core-1.0.0rc4/avilla/core/request.py
+-rw-rw-rw-   0        0        0      794 2022-08-31 04:32:04.278458 avilla-core-1.0.0rc4/avilla/core/resource.py
+-rw-rw-rw-   0        0        0     1306 2022-08-31 04:32:04.279435 avilla-core-1.0.0rc4/avilla/core/service.py
+-rw-rw-rw-   0        0        0        0 2022-08-31 04:32:04.280412 avilla-core-1.0.0rc4/avilla/core/skeleton/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-08-31 04:32:04.281388 avilla-core-1.0.0rc4/avilla/core/skeleton/message.py
+-rw-rw-rw-   0        0        0      635 2022-08-31 04:32:04.282364 avilla-core-1.0.0rc4/avilla/core/skeleton/nick.py
+-rw-rw-rw-   0        0        0     1043 2022-08-31 04:32:04.283341 avilla-core-1.0.0rc4/avilla/core/skeleton/privilege.py
+-rw-rw-rw-   0        0        0      411 2022-08-31 04:32:04.284318 avilla-core-1.0.0rc4/avilla/core/skeleton/request.py
+-rw-rw-rw-   0        0        0      454 2022-08-31 04:32:04.286279 avilla-core-1.0.0rc4/avilla/core/skeleton/scene.py
+-rw-rw-rw-   0        0        0      448 2022-08-31 04:32:04.287247 avilla-core-1.0.0rc4/avilla/core/skeleton/summary.py
+-rw-rw-rw-   0        0        0        0 2022-02-26 15:50:19.551550 avilla-core-1.0.0rc4/avilla/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     5621 2022-08-31 04:32:04.297501 avilla-core-1.0.0rc4/avilla/core/tools/filter.py
+-rw-rw-rw-   0        0        0     8726 2022-08-31 04:32:04.298973 avilla-core-1.0.0rc4/avilla/core/trait/__init__.py
+-rw-rw-rw-   0        0        0     1833 2022-08-31 04:32:04.299944 avilla-core-1.0.0rc4/avilla/core/trait/context.py
+-rw-rw-rw-   0        0        0     5597 2022-08-31 04:32:04.300917 avilla-core-1.0.0rc4/avilla/core/trait/recorder.py
+-rw-rw-rw-   0        0        0     1189 2022-08-31 04:32:04.301894 avilla-core-1.0.0rc4/avilla/core/trait/signature.py
+-rw-rw-rw-   0        0        0      598 2022-08-31 04:32:04.303845 avilla-core-1.0.0rc4/avilla/core/typing.py
+-rw-rw-rw-   0        0        0      743 2022-08-31 04:32:04.306780 avilla-core-1.0.0rc4/avilla/core/utilles/__init__.py
+-rw-rw-rw-   0        0        0     2089 2022-08-31 04:32:04.308733 avilla-core-1.0.0rc4/avilla/core/utilles/event_parser.py
+-rw-rw-rw-   0        0        0     2261 2022-08-31 04:32:04.310684 avilla-core-1.0.0rc4/avilla/core/utilles/message_deserializer.py
+-rw-rw-rw-   0        0        0     1828 2022-08-31 04:32:04.311663 avilla-core-1.0.0rc4/avilla/core/utilles/message_serializer.py
+-rw-rw-rw-   0        0        0     1185 2022-08-31 04:32:04.312638 avilla-core-1.0.0rc4/avilla/core/utilles/promise.py
+-rw-rw-rw-   0        0        0     9868 2022-08-31 04:32:04.322882 avilla-core-1.0.0rc4/avilla/core/utilles/selector.py
+-rw-rw-rw-   0        0        0     1471 2022-07-06 11:17:51.497052 avilla-core-1.0.0rc4/avilla/core/utilles/selector_new.py
+-rw-rw-rw-   0        0        0     1080 2022-08-31 04:32:04.325334 avilla-core-1.0.0rc4/avilla/core/utilles/stream.py
+-rw-rw-rw-   0        0        0     1091 2022-02-26 15:50:19.520302 avilla-core-1.0.0rc4/LICENSE
+-rw-rw-rw-   0        0        0     2168 2022-08-31 04:36:38.408969 avilla-core-1.0.0rc4/pyproject.toml
+-rw-rw-rw-   0        0        0     7166 2022-08-31 04:32:04.240367 avilla-core-1.0.0rc4/README.md
+-rw-rw-rw-   0        0        0     7366 2022-08-31 04:40:23.300146 avilla-core-1.0.0rc4/PKG-INFO
```

### Comparing `avilla-core-1.0.0rc3/LICENSE` & `avilla-core-1.0.0rc4/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Graia Project
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Graia Project
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `avilla-core-1.0.0rc3/README.md` & `avilla-core-1.0.0rc4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: avilla-core
+Version: 1.0.0rc4
+License: MIT
+Author-email: GreyElaina <GreyElaina@outlook.com>
+Requires-Python: >=3.9
+Project-URL: homepage, https://github.com/GraiaProject/Avilla
+Project-URL: repository, https://github.com/GraiaProject/Avilla
+Description-Content-Type: text/markdown
+
 <div align="center">
 
 # Avilla
 
 _The next-gen framework for IM development._
 
 > 即刻动身, 踏上寻找第二个故乡的旅程.
@@ -18,26 +28,28 @@
 通过对 [ `OneBot` ](https://github.com/botuniverse/onebot), [ `Telegram Bot API` ](https://core.telegram.org/bots) 及其他的基于不同即时通讯软件实现的各式对接接口,
 以及其他具有相应概念的 "异步消息流" 实例进行总结, 抽象其中最为基本的各式模型, 构造了一个理论上可以实现零成本切换对接平台的框架.
 
 **该框架目前处于快速迭代状态, API 可能会发生 _剧烈_ 变化, 可能还不适合进行生产性的开发与运维**
 
 > 项目名称取自日本轻小说 《魔女之旅》 的角色 "艾维莉亚(Avilla)".
 
-## Roadmap
+|Docs|[![docs](https://img.shields.io/badge/docs%20on-readthedocs-black)](https://graia.readthedocs.io/)|[![docs](https://img.shields.io/badge/docs%20on-netlify-informational)](https://graia.netlify.app/)|[![docs](https://img.shields.io/badge/docs%20on-cloudflare-orange)](https://graia.pages.dev/)|
+|:-:|:-:|:-:|:-:|
+
+## Notable Features
 
-* `Avilla Protocol` : 对各式常见的行为进行抽象, 并通过可扩展的模型, 实现尽可能的功能可迁移性.
-  - 使用 [Launart](https://github.com/GraiaProject/Launart) 调度启动任务与应用实例的生命周期;
-  - 创新性的 Relationship 模型, 携带有进行任意操作所需的基本信息, 规范化行为模式与实现的编写;
-  - 使用 `Selector`, 实现了信息与对象本身的解耦, 减少平台实现的负担;
-  - 规范化的 `Resource` 抽象优化了对不同资源与资源类型的操作, 尤其是其内容的获取与其元信息的操作;
-  - 规范各式请求为 `Request`;
-  - 将各式元信息放缩为各个最小功能单元及其之间的组合, 不失表现性和可扩展性;
-  - 使用各式如 `Broadcast Control` 的注入入口, 极大简化了接口的使用;
-  - 复用来自 `Amnesia` 的通用接口;
-* And more...
+ - **原生跨平台**: 开创性的 Relationship 操作模型, 配合最小功能单元, 行为扩展等诸多独特设计, 无论是简单的消息收发还是平台设计的独特交互, Avilla 都能处理地得心应手.
+ - **原生多账号**: Avilla 在设计之初, 就考虑了同时管理多个账号, 甚至是多个平台上的多个账号这些问题, 并加以研究与解决. 而现在, 账号管理本应如此简单便捷而收放自如.
+ - **一次编写, 多平台可用**: 得益于 Avilla 的强大抽象, 开发者只需面向 Avilla 就能完成核心业务的开发, 显著的减少了维护成本.
+ - **平台特性友好**: Avilla 以 Activity, Reaction, Extension 等诸项设计, 使得开发者在运用平台特性的方式更加规范而不失表达性. 担心平台间特性的不通用? 你可以同时为多个平台编写不同的特性用例, Avilla 会自动应用可用的适配, 不改动核心逻辑的同时保证基本特性的可用!
+  > 担心可用性? 我们同样提供了一些核心的非平台依赖实现, 例如 `TextCommand`, 这些组件仅要求平台实现最基本的交互实现, 剩下的一切交给 Avilla 处理!
+ - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
+ - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
+
+## Quick Start
 
 ```py
 from creart import create
 from graia.amnesia.builtins.aiohttp import AiohttpService
 from graia.broadcast import Broadcast
 
 from avilla.core import Avilla, MessageReceived, Relationship, Selector
@@ -57,22 +69,22 @@
         await rs.send_message("Hello, Avilla!")
 
 avilla.launch_manager.launch_blocking(loop=broadcast.loop)
 ```
 
 ## 部件发布情况
 
-|代号|协议|开发进度|PyPI|维护者|
-| :-: | :-: | :-: | :-: | :-: |
-|      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |
-| [Elizabeth](avilla/elizabeth) | `mirai-api-http` |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official |
-|    [-](avilla/onebot/v11)     |   `OneBot v11`   |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official |
-|    [-](avilla/onebot/v12)     |   `OneBot v12`   | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) | Official |
-|     [-](avilla/telegram)      |    `Telegram`    | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     |
-| [Nightcord](avilla/nightcord) |  `Discord Bots`  | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  | Official |
+|代号|协议|开发进度|PyPI|维护者|开源协议|
+| :-: | :-: | :-: | :-: | :-: | :-: |
+|      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |MIT|
+| [Elizabeth](avilla/elizabeth) | `mirai-api-http` |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official |AGPLv3|
+|    [-](avilla/onebot/v11)     |   `OneBot v11`   |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official | - |
+|    [-](avilla/onebot/v12)     |   `OneBot v12`   | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) | Official | - |
+|     [-](avilla/telegram)      |    `Telegram`    | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     | - |
+| [Nightcord](avilla/nightcord) |  `Discord Bots`  | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  | Official | - |
 
 ## 我们的愿景
 
 创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
 助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
 
 ## 相关项目
@@ -104,7 +116,8 @@
 
 </div>
 
 
 ## 开源协议
 
 若非特殊说明, Avilla 及其子包默认使用 MIT 作为开源协议, 但如果你若引用到了使用 GPL/AGPL/LGPL 等具有传染性开源协议的项目, 无论是对 Avilla 实现或是使用了相应 Avilla 实现的项目仍需要遵循相关规则.
+
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/application.py` & `avilla-core-1.0.0rc4/avilla/core/application.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,198 @@
-from __future__ import annotations
-
-import importlib.metadata
-import re
-from inspect import cleandoc
-from typing import cast
-
-from graia.broadcast import Broadcast
-from launart import Launart, Service
-from loguru import logger
-
-from avilla.core.account import AbstractAccount
-from avilla.core.action.extension import ActionExtension
-from avilla.core.action.middleware import ActionMiddleware
-from avilla.core.context import get_current_avilla
-from avilla.core.dispatchers import (
-    AvillaBuiltinDispatcher,
-    MetadataDispatcher,
-    RelationshipDispatcher,
-)
-from avilla.core.platform import Land
-from avilla.core.protocol import BaseProtocol
-from avilla.core.resource import ResourceProvider
-from avilla.core.service import AvillaService
-from avilla.core.typing import ActionExtensionImpl
-from avilla.core.utilles.selector import Selector
-
-AVILLA_ASCII_LOGO = cleandoc(
-    r"""
-    [bold]Avilla[/]: a universal asynchronous message flow solution, powered by [blue]Graia Project[/].
-        _        _ _ _
-       / \__   _(_) | | __ _
-      / _ \ \ / / | | |/ _` |
-     / ___ \ V /| | | | (_| |
-    /_/   \_\_/ |_|_|_|\__,_|
-    """
-)
-AVILLA_ASCII_RAW_LOGO = re.sub(r"\[.*?\]", "", AVILLA_ASCII_LOGO)
-
-
-GRAIA_PROJECT_REPOS = [
-    "avilla-core",
-    "graia-broadcast",
-    "graia-saya",
-    "graia-scheduler",
-    "graia-ariadne" "statv",
-    "launart",
-    "creart",
-    "creart-graia",
-    "kayaku",
-]
-
-
-def _log_telemetry():
-    for telemetry in GRAIA_PROJECT_REPOS:
-        try:
-            version = importlib.metadata.version(telemetry)
-        except Exception:
-            version = "unknown / not-installed"
-        logger.info(
-            f"{telemetry} version: {version}",
-            alt=f"[b cornflower_blue]{telemetry}[/] version: [cyan3]{version}[/]",
-        )
-
-
-class Avilla:
-    broadcast: Broadcast
-    launch_manager: Launart
-    protocols: list[BaseProtocol]
-    action_middlewares: list[ActionMiddleware]
-    resource_providers: dict[str, ResourceProvider]
-    extension_impls: dict[type[ActionExtension], ActionExtensionImpl]
-    accounts: list[AbstractAccount]
-    service: AvillaService
-
-    # NOTE: configuration is done by kayaku.
-    def __init__(
-        self,
-        broadcast: Broadcast,
-        protocols: list[BaseProtocol],
-        services: list[Service],
-        middlewares: list[ActionMiddleware] | None = None,
-        launch_manager: Launart | None = None,
-    ):
-        if len({type(i) for i in protocols}) != len(protocols):
-            raise ValueError("protocol must be unique, and the config should be passed by config.")
-
-        self.broadcast = broadcast
-        self.launch_manager = launch_manager or Launart()
-        self.protocols = protocols
-        self._protocol_map = {type(i): i for i in protocols}
-        self.action_middlewares = middlewares or []
-        self.accounts = []
-        self.resource_providers = {}
-        self.extension_impls = {}
-        self.service = AvillaService(self)
-
-        for service in services:
-            self.launch_manager.add_service(service)
-
-        self.launch_manager.add_service(self.service)
-
-        for protocol in self.protocols:
-            # Ensureable 用于注册各种东西, 包括 Service, ResourceProvider 等.
-            protocol.ensure(self)
-
-        self.broadcast.finale_dispatchers.append(MetadataDispatcher())
-        self.broadcast.finale_dispatchers.append(AvillaBuiltinDispatcher(self))
-        self.broadcast.finale_dispatchers.append(RelationshipDispatcher())
-
-    @classmethod
-    def current(cls) -> "Avilla":
-        return get_current_avilla()
-
-    @property
-    def loop(self):
-        return self.broadcast.loop
-
-    def add_action_middleware(self, middleware: ActionMiddleware):
-        self.action_middlewares.append(middleware)
-
-    def remove_action_middleware(self, middleware: ActionMiddleware):
-        self.action_middlewares.remove(middleware)
-
-    def get_resource_provider(self, resource: Selector) -> ResourceProvider | None:
-        return self.resource_providers.get(cast(str, resource.latest_key))
-
-    def add_resource_provider(self, provider: ResourceProvider, *resource_types: str):
-        for resource_type in resource_types:
-            self.resource_providers[resource_type] = provider
-
-    def remove_resource_provider(self, provider: ResourceProvider):
-        for resource_type in self.resource_providers:
-            if self.resource_providers[resource_type] is provider:
-                del self.resource_providers[resource_type]
-
-    def add_account(self, account: AbstractAccount):
-        if account in self.accounts:
-            raise ValueError("account already exists.")
-        self.accounts.append(account)
-
-    def remove_account(self, account: AbstractAccount):
-        if account not in self.accounts:
-            raise ValueError("account not exists.")
-        self.accounts.remove(account)
-
-    def get_account(
-        self, account_id: str | None = None, selector: Selector | None = None, land: Land | None = None
-    ) -> AbstractAccount | None:
-        for account in self.accounts:
-            if account_id is not None and account.id != account_id:
-                continue
-            if selector is not None and not selector.match(account.to_selector()):
-                continue
-            if land is not None and account.land != land:
-                continue
-            return account
-
-    def get_accounts(
-        self, account_id: str | None = None, selector: Selector | None = None, land: Land | None = None
-    ) -> list[AbstractAccount]:
-        result = []
-        for account in self.accounts:
-            if account_id is not None and account.id != account_id:
-                continue
-            if selector is not None and not selector.match(account.to_selector()):
-                continue
-            if land is not None and account.land != land:
-                continue
-            result.append(account)
-        return result
-
-    async def launch(self):
-        logger.info(AVILLA_ASCII_RAW_LOGO, alt=AVILLA_ASCII_LOGO)
-        _log_telemetry()
-
-        for protocol in self.protocols:
-            if protocol.__class__.platform is not BaseProtocol.platform:
-                logger.info(
-                    f"Using platform: {protocol.__class__.platform}",
-                    alt=f"[magenta]Using platform: [/][dark_orange]{protocol.__class__.platform}[/]",
-                )
-
-        await self.launch_manager.launch()
+from __future__ import annotations
+
+import importlib.metadata
+import re
+from inspect import cleandoc
+from typing import TYPE_CHECKING, Any, cast
+
+from graia.broadcast import Broadcast
+from launart import Launart, Service
+from loguru import logger
+
+from avilla.core.account import AbstractAccount
+from avilla.core.context import get_current_avilla
+from avilla.core.dispatchers import AvillaBuiltinDispatcher, RelationshipDispatcher
+from avilla.core.platform import Land
+from avilla.core.protocol import BaseProtocol
+from avilla.core.resource import LocalFileResource
+from avilla.core.service import AvillaService
+from avilla.core.trait.signature import ResourceFetch
+from avilla.core.utilles.selector import Selector
+
+if TYPE_CHECKING:
+    from avilla.core.trait.signature import ArtifactSignature
+
+AVILLA_ASCII_LOGO = cleandoc(
+    r"""
+    [bold]Avilla[/]: a universal asynchronous message flow solution, powered by [blue]Graia Project[/].
+        _        _ _ _
+       / \__   _(_) | | __ _
+      / _ \ \ / / | | |/ _` |
+     / ___ \ V /| | | | (_| |
+    /_/   \_\_/ |_|_|_|\__,_|
+    """
+)
+AVILLA_ASCII_RAW_LOGO = re.sub(r"\[.*?\]", "", AVILLA_ASCII_LOGO)
+
+
+GRAIA_PROJECT_REPOS = [
+    "avilla-core",
+    "graia-broadcast",
+    "graia-saya",
+    "graia-scheduler",
+    "graia-ariadne",
+    "statv",
+    "launart",
+    "creart",
+    "creart-graia",
+    "kayaku",
+]
+
+
+def _log_telemetry():
+    for telemetry in GRAIA_PROJECT_REPOS:
+        try:
+            version = importlib.metadata.version(telemetry)
+        except Exception:
+            version = "unknown / not-installed"
+        logger.info(
+            f"{telemetry} version: {version}",
+            alt=f"[b cornflower_blue]{telemetry}[/] version: [cyan3]{version}[/]",
+        )
+
+
+class Avilla:
+    broadcast: Broadcast
+    launch_manager: Launart
+    protocols: list[BaseProtocol]
+    # action_middlewares: list[ActionMiddleware]
+    # resource_providers: dict[str, ResourceProvider]
+    # extension_impls: dict[type[ActionExtension], ActionExtensionImpl]
+    accounts: list[AbstractAccount]
+    service: AvillaService
+    global_artifacts: dict[ArtifactSignature, Any]
+
+    # NOTE: configuration is done by kayaku.
+    def __init__(
+        self,
+        broadcast: Broadcast,
+        protocols: list[BaseProtocol],
+        services: list[Service],
+        # middlewares: list[ActionMiddleware] | None = None,
+        launch_manager: Launart | None = None,
+    ):
+        if len({type(i) for i in protocols}) != len(protocols):
+            raise ValueError("protocol must be unique, and the config should be passed by config.")
+
+        self.broadcast = broadcast
+        self.launch_manager = launch_manager or Launart()
+        self.protocols = protocols
+        self._protocol_map = {type(i): i for i in protocols}
+        # self.action_middlewares = middlewares or []
+        self.accounts = []
+        # self.resource_providers = {}
+        # self.extension_impls = {}
+        self.global_artifacts = {}
+        self.service = AvillaService(self)
+
+        for service in services:
+            self.launch_manager.add_service(service)
+
+        self.launch_manager.add_service(self.service)
+
+        for protocol in self.protocols:
+            # Ensureable 用于注册各种东西, 包括 Service, ResourceProvider 等.
+            protocol.ensure(self)
+
+        # self.broadcast.finale_dispatchers.append(MetadataDispatcher())
+        self.broadcast.finale_dispatchers.append(AvillaBuiltinDispatcher(self))
+        self.broadcast.finale_dispatchers.append(RelationshipDispatcher())
+
+        @self.register_global_artifact(ResourceFetch(LocalFileResource))
+        async def _fetch_local_file(_, res: LocalFileResource):
+            return res.file.read_bytes()
+
+    @classmethod
+    def current(cls) -> "Avilla":
+        return get_current_avilla()
+
+    @property
+    def loop(self):
+        return self.broadcast.loop
+
+    def register_global_artifact(self, signature: ArtifactSignature):
+        def warpper(v):
+            self.global_artifacts[signature] = v
+            return v
+
+        return warpper
+
+    """
+    def add_action_middleware(self, middleware: ActionMiddleware):
+        self.action_middlewares.append(middleware)
+
+    def remove_action_middleware(self, middleware: ActionMiddleware):
+        self.action_middlewares.remove(middleware)
+
+    def get_resource_provider(self, resource: Selector) -> ResourceProvider | None:
+        return self.resource_providers.get(cast(str, resource.latest_key))
+
+    def add_resource_provider(self, provider: ResourceProvider, *resource_types: str):
+        for resource_type in resource_types:
+            self.resource_providers[resource_type] = provider
+
+    def remove_resource_provider(self, provider: ResourceProvider):
+        for resource_type in self.resource_providers:
+            if self.resource_providers[resource_type] is provider:
+                del self.resource_providers[resource_type]
+
+    """
+
+    def add_account(self, account: AbstractAccount):
+        if account in self.accounts:
+            raise ValueError("account already exists.")
+        self.accounts.append(account)
+
+    def remove_account(self, account: AbstractAccount):
+        if account not in self.accounts:
+            raise ValueError("account not exists.")
+        self.accounts.remove(account)
+
+    def get_account(
+        self, account_id: str | None = None, selector: Selector | None = None, land: Land | None = None
+    ) -> AbstractAccount | None:
+        for account in self.accounts:
+            if account_id is not None and account.id != account_id:
+                continue
+            if selector is not None and not selector.match(account.to_selector()):
+                continue
+            if land is not None and account.land != land:
+                continue
+            return account
+
+    def get_accounts(
+        self, account_id: str | None = None, selector: Selector | None = None, land: Land | None = None
+    ) -> list[AbstractAccount]:
+        result = []
+        for account in self.accounts:
+            if account_id is not None and account.id != account_id:
+                continue
+            if selector is not None and not selector.match(account.to_selector()):
+                continue
+            if land is not None and account.land != land:
+                continue
+            result.append(account)
+        return result
+
+    async def launch(self):
+        logger.info(AVILLA_ASCII_RAW_LOGO, alt=AVILLA_ASCII_LOGO)
+        _log_telemetry()
+
+        for protocol in self.protocols:
+            if protocol.__class__.platform is not BaseProtocol.platform:
+                logger.info(
+                    f"Using platform: {protocol.__class__.platform}",
+                    alt=f"[magenta]Using platform: [/][dark_orange]{protocol.__class__.platform}[/]",
+                )
+
+        await self.launch_manager.launch()
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/context.py` & `avilla-core-1.0.0rc4/avilla/core/context.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from __future__ import annotations
-
-import functools
-from typing import TYPE_CHECKING, Any
-
-from graia.broadcast.utilles import Ctx
-
-if TYPE_CHECKING:
-    from graia.broadcast.entities.event import Dispatchable
-
-    from avilla.core.application import Avilla
-    from avilla.core.protocol import BaseProtocol
-    from avilla.core.relationship import Relationship
-
-
-ctx_avilla: Ctx[Avilla] = Ctx("avilla")
-ctx_protocol: Ctx[BaseProtocol] = Ctx("protocol")
-ctx_relationship: Ctx[Relationship] = Ctx("relationship")
-
-
-def get_current_avilla() -> Avilla:
-    avilla = ctx_avilla.get()
-    if avilla:
-        return avilla
-    protocol = ctx_protocol.get()
-    if protocol:
-        return protocol.avilla
-    relationship = ctx_relationship.get()
-    if relationship:
-        return relationship.protocol.avilla
-    raise RuntimeError("no any current avilla")
-
-
-def get_current_protocol():
-    protocol = ctx_protocol.get()
-    if protocol:
-        return protocol
-    relationship = ctx_relationship.get()
-    if relationship:
-        return relationship.protocol
-    raise RuntimeError("no any current protocol")
-
-
-def get_current_relationship():
-    relationship = ctx_relationship.get()
-    if relationship:
-        return relationship
-    raise RuntimeError("no any current relationship")
-
-
-def require_relationship(func):
-    @functools.wraps(func)
-    async def wrapper(*args, **kwargs):
-        if ctx_relationship.get():
-            return await func(*args, **kwargs)
-        raise RuntimeError("no any current relationship")
-
-    return wrapper
+from __future__ import annotations
+
+import functools
+from typing import TYPE_CHECKING, Any
+
+from graia.broadcast.utilles import Ctx
+
+if TYPE_CHECKING:
+    from graia.broadcast.entities.event import Dispatchable
+
+    from avilla.core.application import Avilla
+    from avilla.core.protocol import BaseProtocol
+    from avilla.core.relationship import Relationship
+
+
+ctx_avilla: Ctx[Avilla] = Ctx("avilla")
+ctx_protocol: Ctx[BaseProtocol] = Ctx("protocol")
+ctx_relationship: Ctx[Relationship] = Ctx("relationship")
+
+
+def get_current_avilla() -> Avilla:
+    avilla = ctx_avilla.get()
+    if avilla:
+        return avilla
+    protocol = ctx_protocol.get()
+    if protocol:
+        return protocol.avilla
+    relationship = ctx_relationship.get()
+    if relationship:
+        return relationship.protocol.avilla
+    raise RuntimeError("no any current avilla")
+
+
+def get_current_protocol():
+    protocol = ctx_protocol.get()
+    if protocol:
+        return protocol
+    relationship = ctx_relationship.get()
+    if relationship:
+        return relationship.protocol
+    raise RuntimeError("no any current protocol")
+
+
+def get_current_relationship():
+    relationship = ctx_relationship.get()
+    if relationship:
+        return relationship
+    raise RuntimeError("no any current relationship")
+
+
+def require_relationship(func):
+    @functools.wraps(func)
+    async def wrapper(*args, **kwargs):
+        if ctx_relationship.get():
+            return await func(*args, **kwargs)
+        raise RuntimeError("no any current relationship")
+
+    return wrapper
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/elements.py` & `avilla-core-1.0.0rc4/avilla/core/elements.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,92 @@
-from __future__ import annotations
-
-from pathlib import Path
-from typing import Any
-
-from graia.amnesia.message import Element
-from graia.amnesia.message.element import Text as Text
-
-from avilla.core.resource import Resource
-from avilla.core.resource.local import LocalFileResource
-from avilla.core.utilles.selector import Selector
-
-
-class Notice(Element):
-    """该消息元素用于承载消息中用于提醒/呼唤特定用户的部分."""
-
-    target: Selector
-
-    def __init__(self, target: Selector) -> None:
-        """实例化一个 Notice 消息元素, 用于承载消息中用于提醒/呼唤特定用户的部分.
-
-        Args:
-            target (str): 需要提醒/呼唤的特定用户的 ID.
-        """
-
-        self.target = target
-
-    def __str__(self) -> str:
-        return f"[$Notice:target={self.target}]"
-
-
-class NoticeAll(Element):
-    "该消息元素用于群组中的管理员提醒群组中的所有成员"
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __str__(self) -> str:
-        return "[$NoticeAll]"
-
-
-class Image(Element):
-    resource: Resource[bytes]
-
-    def __init__(self, resource: Resource[bytes] | Path | str):
-        if isinstance(resource, Path):
-            resource = LocalFileResource(resource)
-        elif isinstance(resource, str):
-            resource = LocalFileResource(Path(resource))
-        self.resource = resource
-
-    def __str__(self) -> str:
-        return "[$Image]"
-
-
-class Audio(Element):
-    resource: Resource[bytes]
-
-    def __init__(self, resource: Resource[bytes] | Path | str):
-        if isinstance(resource, Path):
-            resource = LocalFileResource(resource)
-        elif isinstance(resource, str):
-            resource = LocalFileResource(Path(resource))
-        self.resource = resource
-
-    def __str__(self) -> str:
-        return "[$Audio]"
-
-
-class Video(Element):
-    resource: Resource[bytes]
-
-    def __init__(self, resource: Resource[bytes] | Path | str):
-        if isinstance(resource, Path):
-            resource = LocalFileResource(resource)
-        elif isinstance(resource, str):
-            resource = LocalFileResource(Path(resource))
-        self.resource = resource
-
-    def __str__(self) -> str:
-        return "[$Video]"
-
-
-class Unknown(Element):
-    type: str
-    raw_data: Any
-
-    def __init__(self, type: str, raw_data: Any) -> None:
-        self.type = type
-        self.raw_data = raw_data
-
-    def __str__(self) -> str:
-        return f"[$Unknown:type={self.type}]"
+from __future__ import annotations
+
+from pathlib import Path
+from typing import Any
+
+from graia.amnesia.message import Element
+from graia.amnesia.message.element import Text as Text
+
+from avilla.core.resource import LocalFileResource, Resource
+from avilla.core.utilles.selector import Selector
+
+
+class Notice(Element):
+    """该消息元素用于承载消息中用于提醒/呼唤特定用户的部分."""
+
+    target: Selector
+
+    def __init__(self, target: Selector) -> None:
+        """实例化一个 Notice 消息元素, 用于承载消息中用于提醒/呼唤特定用户的部分.
+
+        Args:
+            target (str): 需要提醒/呼唤的特定用户的 ID.
+        """
+
+        self.target = target
+
+    def __str__(self) -> str:
+        return f"[$Notice:target={self.target}]"
+
+
+class NoticeAll(Element):
+    "该消息元素用于群组中的管理员提醒群组中的所有成员"
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __str__(self) -> str:
+        return "[$NoticeAll]"
+
+
+class Picture(Element):
+    resource: Resource[bytes]
+
+    def __init__(self, resource: Resource[bytes] | Path | str):
+        if isinstance(resource, Path):
+            resource = LocalFileResource(resource)
+        elif isinstance(resource, str):
+            resource = LocalFileResource(Path(resource))
+        self.resource = resource
+
+    def __str__(self) -> str:
+        return "[$Picture]"
+
+
+class Audio(Element):
+    resource: Resource[bytes]
+
+    def __init__(self, resource: Resource[bytes] | Path | str):
+        if isinstance(resource, Path):
+            resource = LocalFileResource(resource)
+        elif isinstance(resource, str):
+            resource = LocalFileResource(Path(resource))
+        self.resource = resource
+
+    def __str__(self) -> str:
+        return "[$Audio]"
+
+
+class Video(Element):
+    resource: Resource[bytes]
+
+    def __init__(self, resource: Resource[bytes] | Path | str):
+        if isinstance(resource, Path):
+            resource = LocalFileResource(resource)
+        elif isinstance(resource, str):
+            resource = LocalFileResource(Path(resource))
+        self.resource = resource
+
+    def __str__(self) -> str:
+        return "[$Video]"
+
+
+class Unknown(Element):
+    type: str
+    raw_data: Any
+
+    def __init__(self, type: str, raw_data: Any) -> None:
+        self.type = type
+        self.raw_data = raw_data
+
+    def __str__(self) -> str:
+        return f"[$Unknown:type={self.type}]"
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/event/__init__.py` & `avilla-core-1.0.0rc4/avilla/core/event/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,104 @@
-from __future__ import annotations
-
-from abc import ABCMeta, abstractmethod
-from datetime import datetime
-from typing import TYPE_CHECKING, Any
-
-from graia.broadcast.entities.event import Dispatchable
-
-if TYPE_CHECKING:
-    from avilla.core.account import AbstractAccount
-    from avilla.core.metadata.model import MetadataModifies
-    from avilla.core.utilles.selector import Selector
-
-
-class AvillaEvent(Dispatchable, metaclass=ABCMeta):
-    account: AbstractAccount
-    time: datetime
-
-    extra: dict[Any, Any]
-
-    def __init__(
-        self, account: AbstractAccount, *, extra: dict[Any, Any] | None = None, time: datetime | None = None
-    ) -> None:
-        self.account = account
-        self.extra = extra or {}
-        self.time = time or datetime.now()
-
-    @property
-    @abstractmethod
-    def ctx(self) -> Selector:
-        ...
-
-    def get_via(self) -> Selector | None:
-        ...
-
-
-class MetadataModified(AvillaEvent):
-    ctx: Selector
-    modifies: MetadataModifies
-    operator: Selector | None = None
-
-    def __init__(
-        self,
-        ctx: Selector,
-        modifies: MetadataModifies,
-        account: AbstractAccount,
-        operator: Selector | None = None,
-        time: datetime | None = None,
-        extra: dict[Any, Any] | None = None,
-    ):
-        self.ctx = ctx
-        self.modifies = modifies
-        self.operator = operator
-        super().__init__(account, time=time, extra=extra)
-
-
-class RelationshipCreated(AvillaEvent):
-    ctx: Selector
-    via: Selector | None
-    # 用 via 同时表示两个方向的关系.(自发行为和被动行为)
-    # 自发行为就是 None, 被动行为反之
-
-    def __init__(
-        self,
-        ctx: Selector,
-        account: AbstractAccount,
-        time: datetime | None = None,
-        via: Selector | None = None,
-    ):
-        self.ctx = ctx
-        self.via = via
-        super().__init__(account, time=time)
-
-    def get_via(self) -> Selector | None:
-        return self.via
-
-
-class RelationshipDestroyed(AvillaEvent):
-    ctx: Selector
-    via: Selector | None
-
-    def __init__(
-        self,
-        ctx: Selector,
-        account: AbstractAccount,
-        time: datetime | None = None,
-        via: Selector | None = None,
-    ):
-        self.ctx = ctx
-        self.via = via
-        super().__init__(account, time=time)
-
-    def get_via(self) -> Selector | None:
-        return self.via
+from __future__ import annotations
+
+from abc import ABCMeta, abstractmethod
+from dataclasses import dataclass
+from datetime import datetime
+from typing import TYPE_CHECKING, Any
+
+from graia.broadcast.entities.event import Dispatchable
+
+if TYPE_CHECKING:
+    from avilla.core.account import AbstractAccount
+    from avilla.core.utilles.selector import Selector
+
+    from ..cell import Cell, CellOf
+
+
+class AvillaEvent(Dispatchable, metaclass=ABCMeta):
+    account: AbstractAccount
+    time: datetime
+
+    extra: dict[Any, Any]
+
+    def __init__(
+        self, account: AbstractAccount, *, extra: dict[Any, Any] | None = None, time: datetime | None = None
+    ) -> None:
+        self.account = account
+        self.extra = extra or {}
+        self.time = time or datetime.now()
+
+    @property
+    @abstractmethod
+    def ctx(self) -> Selector:
+        ...
+
+    def get_via(self) -> Selector | None:
+        ...
+
+
+@dataclass
+class MetadataModify:
+    describe: type[Cell] | CellOf
+    field: str
+    current: Any
+    past: Any | None = None
+
+
+class MetadataModified(AvillaEvent):
+    ctx: Selector
+    modifies: list[MetadataModify]
+    operator: Selector | None = None
+
+    def __init__(
+        self,
+        ctx: Selector,
+        modifies: list[MetadataModify],
+        account: AbstractAccount,
+        operator: Selector | None = None,
+        time: datetime | None = None,
+        extra: dict[Any, Any] | None = None,
+    ):
+        self.ctx = ctx
+        self.modifies = modifies
+        self.operator = operator
+        super().__init__(account, time=time, extra=extra)
+
+
+class RelationshipCreated(AvillaEvent):
+    ctx: Selector
+    via: Selector | None
+    # 用 via 同时表示两个方向的关系.(自发行为和被动行为)
+    # 自发行为就是 None, 被动行为反之
+
+    def __init__(
+        self,
+        ctx: Selector,
+        account: AbstractAccount,
+        time: datetime | None = None,
+        via: Selector | None = None,
+    ):
+        self.ctx = ctx
+        self.via = via
+        super().__init__(account, time=time)
+
+    def get_via(self) -> Selector | None:
+        return self.via
+
+
+class RelationshipDestroyed(AvillaEvent):
+    ctx: Selector
+    via: Selector | None
+
+    def __init__(
+        self,
+        ctx: Selector,
+        account: AbstractAccount,
+        time: datetime | None = None,
+        via: Selector | None = None,
+    ):
+        self.ctx = ctx
+        self.via = via
+        super().__init__(account, time=time)
+
+    def get_via(self) -> Selector | None:
+        return self.via
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/event/lifecycle.py` & `avilla-core-1.0.0rc4/avilla/core/event/lifecycle.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import TYPE_CHECKING
-
-from graia.broadcast.entities.dispatcher import BaseDispatcher
-from graia.broadcast.entities.event import Dispatchable
-from graia.broadcast.interfaces.dispatcher import DispatcherInterface
-
-if TYPE_CHECKING:
-    from ..account import AbstractAccount
-    from ..application import Avilla
-
-
-class AvillaLifecycleEvent(Dispatchable):
-    """指示有关应用 (Avilla) 的事件."""
-
-    avilla: Avilla
-
-    def __init__(self, avilla: Avilla):
-        self.avilla = avilla
-
-    class Dispatcher(BaseDispatcher):
-        @classmethod
-        async def catch(cls, interface: "DispatcherInterface[AvillaLifecycleEvent]"):
-            from ..application import Avilla
-
-            if interface.annotation is Avilla:
-                return interface.event.avilla
-
-
-class ApplicationClosing(AvillaLifecycleEvent):
-    """指示 Avilla 正在关闭."""
-
-
-class ApplicationClosed(AvillaLifecycleEvent):
-    """指示 Avilla 已经关闭."""
-
-
-class ApplicationPreparing(AvillaLifecycleEvent):
-    """指示 Avilla 正在准备."""
-
-
-class ApplicationReady(AvillaLifecycleEvent):
-    """指示 Avilla 已准备完毕."""
-
-
-@dataclass
-class AccountStatusChanged(AvillaLifecycleEvent):
-    """指示当前账号 (Account) 状态发生改变的事件"""
-
-    account: "AbstractAccount"
-
-    class Dispatcher(BaseDispatcher):
-        @classmethod
-        async def catch(cls, interface: "DispatcherInterface[AccountStatusChanged]"):
-            from ..account import AbstractAccount
-
-            if issubclass(interface.annotation, AbstractAccount):
-                return interface.event.account
-
-
-class AccountAvailable(AccountStatusChanged):
-    """指示当前账号处于可用状态."""
-
-
-class AccountUnavailable(AccountStatusChanged):
-    """指示当前账号处于不可用状态."""
+from __future__ import annotations
+
+from dataclasses import dataclass
+from typing import TYPE_CHECKING
+
+from graia.broadcast.entities.dispatcher import BaseDispatcher
+from graia.broadcast.entities.event import Dispatchable
+from graia.broadcast.interfaces.dispatcher import DispatcherInterface
+
+if TYPE_CHECKING:
+    from ..account import AbstractAccount
+    from ..application import Avilla
+
+
+class AvillaLifecycleEvent(Dispatchable):
+    """指示有关应用 (Avilla) 的事件."""
+
+    avilla: Avilla
+
+    def __init__(self, avilla: Avilla):
+        self.avilla = avilla
+
+    class Dispatcher(BaseDispatcher):
+        @classmethod
+        async def catch(cls, interface: "DispatcherInterface[AvillaLifecycleEvent]"):
+            from ..application import Avilla
+
+            if interface.annotation is Avilla:
+                return interface.event.avilla
+
+
+class ApplicationClosing(AvillaLifecycleEvent):
+    """指示 Avilla 正在关闭."""
+
+
+class ApplicationClosed(AvillaLifecycleEvent):
+    """指示 Avilla 已经关闭."""
+
+
+class ApplicationPreparing(AvillaLifecycleEvent):
+    """指示 Avilla 正在准备."""
+
+
+class ApplicationReady(AvillaLifecycleEvent):
+    """指示 Avilla 已准备完毕."""
+
+
+@dataclass
+class AccountStatusChanged(AvillaLifecycleEvent):
+    """指示当前账号 (Account) 状态发生改变的事件"""
+
+    account: "AbstractAccount"
+
+    class Dispatcher(BaseDispatcher):
+        @classmethod
+        async def catch(cls, interface: "DispatcherInterface[AccountStatusChanged]"):
+            from ..account import AbstractAccount
+
+            if issubclass(interface.annotation, AbstractAccount):
+                return interface.event.account
+
+
+class AccountAvailable(AccountStatusChanged):
+    """指示当前账号处于可用状态."""
+
+
+class AccountUnavailable(AccountStatusChanged):
+    """指示当前账号处于不可用状态."""
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/message.py` & `avilla-core-1.0.0rc4/avilla/core/message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, cast
-
-from avilla.core.platform import Land
-from avilla.core.utilles.selector import Selector
-
-if TYPE_CHECKING:
-    from datetime import datetime
-
-    from graia.amnesia.message import MessageChain as MessageChain
-
-
-@dataclass
-class Message:
-    id: str
-    mainline: Selector
-    sender: Selector
-    content: MessageChain
-    time: datetime
-    reply: Selector | None = None
-
-    @property
-    def land(self):
-        return Land(cast(str, self.mainline.pattern.get("land")))
-
-    def to_selector(self) -> Selector:
-        return self.mainline.copy().message(self.id)
+from __future__ import annotations
+
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, cast
+
+from graia.amnesia.message import MessageChain
+
+from avilla.core.cell import Cell
+from avilla.core.platform import Land
+from avilla.core.utilles.selector import Selector
+
+if TYPE_CHECKING:
+    from datetime import datetime
+
+
+@dataclass
+class Message(Cell):
+    id: str
+    mainline: Selector
+    sender: Selector
+    content: MessageChain
+    time: datetime
+    reply: Selector | None = None
+
+    @property
+    def land(self):
+        return Land(cast(str, self.mainline.pattern.get("land")))
+
+    def to_selector(self) -> Selector:
+        return self.mainline.copy().message(self.id)
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/platform.py` & `avilla-core-1.0.0rc4/avilla/core/platform.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import TypedDict, TypeVar
-
-
-@dataclass
-class PlatformDescription:
-    ...
-
-
-PD = TypeVar("PD", bound=PlatformDescription)
-
-
-@dataclass
-class Platform:
-    description: dict[type[PlatformDescription], PlatformDescription]
-
-    def __init__(self, land: Land, abstract: Abstract, *description: PlatformDescription) -> None:
-        self.description = {type(i): i for i in description}
-        self.description[Land] = land
-        self.description[Abstract] = abstract
-
-    def __getitem__(self, item: type[PD]) -> PD:
-        return self.description[item]  # type: ignore
-
-
-class Maintainer(TypedDict):
-    name: str
-
-
-@dataclass
-class Land(PlatformDescription):
-    name: str
-    maintainers: list[Maintainer] = field(default_factory=list)
-    humanized_name: str | None = None
-
-
-@dataclass
-class Abstract(PlatformDescription):
-    protocol: str
-    maintainers: list[Maintainer] = field(default_factory=list)
-    humanized_name: str | None = None
-
-
-@dataclass
-class Branch(PlatformDescription):
-    value: str
-
-
-@dataclass
-class Version(PlatformDescription):
-    components: dict[str, str]
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import TypedDict, TypeVar
+
+
+@dataclass
+class PlatformDescription:
+    ...
+
+
+PD = TypeVar("PD", bound=PlatformDescription)
+
+
+@dataclass
+class Platform:
+    description: dict[type[PlatformDescription], PlatformDescription]
+
+    def __init__(self, land: Land, abstract: Abstract, *description: PlatformDescription) -> None:
+        self.description = {type(i): i for i in description}
+        self.description[Land] = land
+        self.description[Abstract] = abstract
+
+    def __getitem__(self, item: type[PD]) -> PD:
+        return self.description[item]  # type: ignore
+
+
+class Maintainer(TypedDict):
+    name: str
+
+
+@dataclass
+class Land(PlatformDescription):
+    name: str
+    maintainers: list[Maintainer] = field(default_factory=list)
+    humanized_name: str | None = None
+
+
+@dataclass
+class Abstract(PlatformDescription):
+    protocol: str
+    maintainers: list[Maintainer] = field(default_factory=list)
+    humanized_name: str | None = None
+
+
+@dataclass
+class Branch(PlatformDescription):
+    value: str
+
+
+@dataclass
+class Version(PlatformDescription):
+    components: dict[str, str]
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/querier.py` & `avilla-core-1.0.0rc4/avilla/core/querier.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from __future__ import annotations
-
-import inspect
-from typing import (
-    TYPE_CHECKING,
-    AsyncGenerator,
-    AsyncIterator,
-    Callable,
-    ClassVar,
-    Generic,
-    TypeVar,
-)
-
-from typing_extensions import Self
-
-from avilla.core.utilles.selector import Selector
-
-if TYPE_CHECKING:
-    from avilla.core.protocol import BaseProtocol
-    from avilla.core.relationship import Relationship
-
-
-def query(target: str):
-    def wrapper(func):
-        func.__query_key__ = target
-        return func
-
-    return wrapper
-
-
-class AbstractQueryHandler:
-    prefix: str | None
-    queriers: ClassVar[
-        dict[
-            str,
-            Callable[[Self, Relationship, Selector, Callable[[Selector], bool]], AsyncGenerator[Selector, None]],
-        ]
-    ] = {}
-
-    def __init_subclass__(cls, prefix: str | None = None):
-        super().__init_subclass__()
-        cls.queriers = {}
-        cls.prefix = prefix
-        for mro in reversed(inspect.getmro(cls)):
-            if issubclass(mro, AbstractQueryHandler):
-                cls.queriers.update(mro.queriers)
-        members = inspect.getmembers(cls, predicate=inspect.isfunction)
-        for _, value in members:
-            if hasattr(value, "__query_key__"):
-                cls.queriers[value.__query_key__] = value
-
-
-TProtocol = TypeVar("TProtocol", bound="BaseProtocol")
-
-
-class ProtocolAbstractQueryHandler(AbstractQueryHandler, Generic[TProtocol]):
-    protocol: TProtocol
-
-    def __init__(self, protocol: TProtocol) -> None:
-        self.protocol = protocol
-
-    def __init_subclass__(cls, prefix: str | None = None):
-        super().__init_subclass__(prefix)
+from __future__ import annotations
+
+import inspect
+from typing import (
+    TYPE_CHECKING,
+    AsyncGenerator,
+    AsyncIterator,
+    Callable,
+    ClassVar,
+    Generic,
+    TypeVar,
+)
+
+from typing_extensions import Self
+
+from avilla.core.utilles.selector import Selector
+
+if TYPE_CHECKING:
+    from avilla.core.protocol import BaseProtocol
+    from avilla.core.relationship import Relationship
+
+
+def query(target: str):
+    def wrapper(func):
+        func.__query_key__ = target
+        return func
+
+    return wrapper
+
+
+class AbstractQueryHandler:
+    prefix: str | None
+    queriers: ClassVar[
+        dict[
+            str,
+            Callable[[Self, Relationship, Selector, Callable[[Selector], bool]], AsyncGenerator[Selector, None]],
+        ]
+    ] = {}
+
+    def __init_subclass__(cls, prefix: str | None = None):
+        super().__init_subclass__()
+        cls.queriers = {}
+        cls.prefix = prefix
+        for mro in reversed(inspect.getmro(cls)):
+            if issubclass(mro, AbstractQueryHandler):
+                cls.queriers.update(mro.queriers)
+        members = inspect.getmembers(cls, predicate=inspect.isfunction)
+        for _, value in members:
+            if hasattr(value, "__query_key__"):
+                cls.queriers[value.__query_key__] = value
+
+
+TProtocol = TypeVar("TProtocol", bound="BaseProtocol")
+
+
+class ProtocolAbstractQueryHandler(AbstractQueryHandler, Generic[TProtocol]):
+    protocol: TProtocol
+
+    def __init__(self, protocol: TProtocol) -> None:
+        self.protocol = protocol
+
+    def __init_subclass__(cls, prefix: str | None = None):
+        super().__init_subclass__(prefix)
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/typing.py` & `avilla-core-1.0.0rc4/avilla/core/typing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Coroutine,
-    Generic,
-    Protocol,
-    TypeVar,
-    runtime_checkable,
-)
-
-if TYPE_CHECKING:
-    from avilla.core.action.extension import ActionExtension
-    from avilla.core.protocol import BaseProtocol
-    from avilla.core.relationship import RelationshipExecutor
-
-TProtocol = TypeVar("TProtocol", bound="BaseProtocol")
-
-ActionExtensionImpl = Callable[
-    ["RelationshipExecutor", "ActionExtension", dict[str, Any] | None], Coroutine[None, None, Any]
-]
-
-
-_T = TypeVar("_T", contravariant=True)
-
-
-@runtime_checkable
-class Ensureable(Protocol, Generic[_T]):
-    def ensure(self, interact: _T) -> Any:
-        ...
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Coroutine,
+    Generic,
+    Protocol,
+    TypeVar,
+    runtime_checkable,
+)
+
+if TYPE_CHECKING:
+    from avilla.core.protocol import BaseProtocol
+
+"""
+TProtocol = TypeVar("TProtocol", bound="BaseProtocol")
+
+
+ActionExtensionImpl = Callable[
+    ["RelationshipExecutor", "ActionExtension", dict[str, Any] | None], Coroutine[None, None, Any]
+]
+"""
+
+_T = TypeVar("_T", contravariant=True)
+
+
+@runtime_checkable
+class Ensureable(Protocol, Generic[_T]):
+    def ensure(self, interact: _T) -> Any:
+        ...
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/utilles/event_parser.py` & `avilla-core-1.0.0rc4/avilla/core/utilles/event_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from __future__ import annotations
-
-import inspect
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Callable, Coroutine, Generic, TypeVar
-
-from graia.amnesia.message.element import Element
-from graia.broadcast.utilles import run_always_await
-from loguru import logger
-from typing_extensions import Self
-
-from avilla.core.account import AbstractAccount
-from avilla.core.event import AvillaEvent
-
-if TYPE_CHECKING:
-    from avilla.core.account import AbstractAccount
-    from avilla.core.protocol import BaseProtocol
-
-
-def event(event_type: str):
-    def wrapper(func):
-        func.__event_parser__ = event_type
-        return func
-
-    return wrapper
-
-
-_P = TypeVar("_P", bound="BaseProtocol")
-
-
-class AbstractEventParser(ABC, Generic[_P]):
-    event_parser: dict[str, Callable[[Self, _P, AbstractAccount, dict], Element | Coroutine[None, None, Element]]] = {}
-
-    def __init_subclass__(cls) -> None:
-        super().__init_subclass__()
-        cls.event_parser = {}
-        for mro in reversed(inspect.getmro(cls)):
-            if issubclass(mro, AbstractEventParser):
-                cls.event_parser.update(mro.event_parser)
-        members = inspect.getmembers(cls)
-        for _, value in members:
-            if callable(value) and getattr(value, "__event_parser__", False):
-                cls.event_parser[value.__event_parser__] = value
-
-    @abstractmethod
-    def get_event_type(self, raw: dict) -> str:
-        ...
-
-    async def parse_event(
-        self, protocol: _P, account: AbstractAccount, raw: dict, *, error: bool = False
-    ) -> AvillaEvent | None:
-        event_type = self.get_event_type(raw)
-        deserializer = self.event_parser.get(event_type)
-        if deserializer is None:
-            if error:
-                raise NotImplementedError(f"Event type {event_type} is not supported.")
-            logger.warning(f"Event type {event_type} is not supported by {self.__class__.__name__}", raw)
-            return
-        return await run_always_await(deserializer, self, protocol, account, raw)  # type: ignore
+from __future__ import annotations
+
+import inspect
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Callable, Coroutine, Generic, TypeVar
+
+from graia.amnesia.message.element import Element
+from graia.broadcast.utilles import run_always_await
+from loguru import logger
+from typing_extensions import Self
+
+from avilla.core.account import AbstractAccount
+from avilla.core.event import AvillaEvent
+
+if TYPE_CHECKING:
+    from avilla.core.account import AbstractAccount
+    from avilla.core.protocol import BaseProtocol
+
+
+def event(event_type: str):
+    def wrapper(func):
+        func.__event_parser__ = event_type
+        return func
+
+    return wrapper
+
+
+_P = TypeVar("_P", bound="BaseProtocol")
+
+
+class AbstractEventParser(ABC, Generic[_P]):
+    event_parser: dict[str, Callable[[Self, _P, AbstractAccount, dict], Coroutine[None, None, AvillaEvent | None]]] = {}
+
+    def __init_subclass__(cls) -> None:
+        super().__init_subclass__()
+        cls.event_parser = {}
+        for mro in reversed(inspect.getmro(cls)):
+            if issubclass(mro, AbstractEventParser):
+                cls.event_parser.update(mro.event_parser)
+        members = inspect.getmembers(cls)
+        for _, value in members:
+            if callable(value) and getattr(value, "__event_parser__", False):
+                cls.event_parser[value.__event_parser__] = value
+
+    @abstractmethod
+    def get_event_type(self, raw: dict) -> str:
+        ...
+
+    async def parse_event(
+        self, protocol: _P, account: AbstractAccount, raw: dict, *, error: bool = False
+    ) -> AvillaEvent | None:
+        event_type = self.get_event_type(raw)
+        deserializer = self.event_parser.get(event_type)
+        if deserializer is None:
+            if error:
+                raise NotImplementedError(f"Event type {event_type} is not supported.")
+            logger.warning(f"Event type {event_type} is not supported by {self.__class__.__name__}", raw)
+            return
+        return await deserializer(self, protocol, account, raw)
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/utilles/message_serializer.py` & `avilla-core-1.0.0rc4/avilla/core/utilles/message_deserializer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,64 @@
-from __future__ import annotations
-
-import inspect
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, Coroutine, Generic, TypeVar
-
-from graia.amnesia.message import MessageChain
-from graia.amnesia.message.element import Element
-from graia.broadcast.utilles import run_always_await
-from typing_extensions import Self
-
-if TYPE_CHECKING:
-    from avilla.core.protocol import BaseProtocol
-
-
-def element(element_type: type[Element]):
-    def wrapper(func: Callable):
-        func.__element_serializer__ = element_type
-        return func
-
-    return wrapper
-
-
-_P = TypeVar("_P", bound="BaseProtocol")
-
-
-class MessageSerializer(Generic[_P]):
-    element_serializer: dict[type[Element], Callable[[Self, _P, Any], dict | Coroutine[None, None, dict]]] = {}
-
-    def __init_subclass__(cls) -> None:
-        super().__init_subclass__()
-        cls.element_serializer = {}
-        for mro in reversed(inspect.getmro(cls)):
-            if issubclass(mro, MessageSerializer):
-                cls.element_serializer.update(mro.element_serializer)
-        members = inspect.getmembers(cls)
-        for _, value in members:
-            if callable(value) and getattr(value, "__element_serializer__", False):
-                cls.element_serializer[value.__element_serializer__] = value
-
-    async def serialize_element(self, protocol: _P, element: Element) -> dict:
-        if type(element) not in self.element_serializer:
-            raise NotImplementedError(f"Element type {type(element)} is not supported.")
-        return await run_always_await(self.element_serializer[type(element)], self, protocol, element)  # type: ignore
-
-    async def serialize_chain(self, protocol: _P, message: MessageChain):
-        return [await self.serialize_element(protocol, element) for element in message.content]
+from __future__ import annotations
+
+import inspect
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, Generic, Iterable, TypeVar
+
+from graia.amnesia.message.element import Element
+from typing_extensions import Self
+
+from avilla.core.elements import Unknown
+from avilla.core.utilles import run_always_await
+
+if TYPE_CHECKING:
+    from avilla.core.protocol import BaseProtocol
+
+
+def deserializer(element_type: str):
+    def wrapper(func):
+        func.__element_deserializer__ = element_type
+        return func
+
+    return wrapper
+
+
+_P = TypeVar("_P", bound="BaseProtocol")
+
+
+class MessageDeserializer(ABC, Generic[_P]):
+    element_deserializer: dict[
+        str, Callable[[Self, _P, dict], Coroutine[None, None, Element]] | Callable[[Self, _P, dict], Element]
+    ] = {}
+    ignored_types: set[str] = set()
+
+    def __init_subclass__(cls) -> None:
+        super().__init_subclass__()
+        cls.element_deserializer = {}
+        for mro in reversed(inspect.getmro(cls)):
+            if issubclass(mro, MessageDeserializer):
+                cls.element_deserializer.update(mro.element_deserializer)
+        members = inspect.getmembers(cls)
+        for _, value in members:
+            if callable(value) and getattr(value, "__element_deserializer__", False):
+                cls.element_deserializer[value.__element_deserializer__] = value
+
+    def split_message(self, data: list) -> Iterable[dict]:
+        yield from data
+
+    @abstractmethod
+    def get_element_type(self, raw: dict) -> str:
+        ...
+
+    async def parse_element(self, protocol: _P, raw: dict) -> Element:
+        element_type = self.get_element_type(raw)
+        deserializer = self.element_deserializer.get(element_type)
+        if deserializer is None:
+            return Unknown(type=element_type, raw_data=raw)
+        return await run_always_await(deserializer, self, protocol, raw)  # type: ignore
+
+    async def parse_sentence(self, protocol: _P, data: list) -> list[Any]:
+        return [
+            await self.parse_element(protocol, raw)
+            for raw in self.split_message(data)
+            if self.get_element_type(raw) not in self.ignored_types
+        ]
```

### Comparing `avilla-core-1.0.0rc3/avilla/core/utilles/selector.py` & `avilla-core-1.0.0rc4/avilla/core/utilles/selector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,299 @@
-from __future__ import annotations
-
-from collections import ChainMap
-from itertools import filterfalse
-from typing import TYPE_CHECKING, Any, Callable, Literal, Protocol, runtime_checkable
-
-from typing_extensions import Self
-
-from avilla.core.platform import Land
-
-if TYPE_CHECKING:
-    ...
-
-MatchRule = Literal["any", "exact", "exist", "fragment", "startswith"]
-Pattern = str | Callable[[str], bool]
-
-
-class Selector:
-    mode: MatchRule = "exact"
-    pattern: dict[str, str]
-    path_excludes: frozenset[str]
-    referent: Any = None
-
-    def __init__(self, *, mode: MatchRule = "exact", path_excludes: frozenset[str] = frozenset()) -> None:
-        self.mode = mode
-        self.path_excludes = path_excludes
-        self.pattern = {}
-
-    def __getattr__(self, name: str) -> Callable[[str], Self]:
-        def wrapper(content: str) -> Self:
-            self.pattern[name] = content
-            return self
-
-        return wrapper
-
-    def __hash__(self) -> int:
-        return hash("Selector") + hash(tuple(self.pattern.items()))
-
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o, Selector) and o.pattern == self.pattern
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.pattern
-
-    def __getitem__(self, key: str) -> str:
-        return self.pattern[key]
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(mode={self.mode}).{'.'.join(f'{k}({v})' for k, v in self.pattern.items())}"
-
-    @property
-    def empty(self) -> bool:
-        return not self.pattern
-
-    @property
-    def path(self) -> str:
-        return ".".join(filterfalse(self.path_excludes.__contains__, self.pattern))
-
-    @property
-    def path_without_land(self) -> str:
-        return ".".join(filterfalse((self.path_excludes | {"land"}).__contains__, self.pattern))
-
-    @classmethod
-    def exist(cls) -> Self:
-        return cls(mode="exist")
-
-    @classmethod
-    def any(cls) -> Self:
-        return cls(mode="any")
-
-    @classmethod
-    def fragment(cls, *path_excludes: str) -> Self:
-        return cls(mode="fragment", path_excludes=frozenset(path_excludes))
-
-    @classmethod
-    def from_dict(cls, pattern: dict) -> Self:
-        instance = cls()
-        instance.pattern = pattern
-        return instance
-
-    @property
-    def latest_key(self) -> str:
-        return list(self.pattern.keys())[-1]
-
-    def land(self, land: Land | str):
-        if isinstance(land, Land):
-            land = land.name
-        self.pattern["land"] = land
-        return self
-
-    def match(self, other: Selector) -> bool:
-        if not isinstance(other, Selector):
-            return False
-        try:
-            match = {
-                "any": self._match_any,
-                "exact": self._match_exact,
-                "exist": self._match_exist,
-                "fragment": self._match_fragment,
-                "startswith": self._match_startswith,
-            }[self.mode]
-        except KeyError:
-            raise ValueError(f"Unknown match rule: {self.mode}") from None
-
-        return match(other)
-
-    def _match_any(self, other: Selector) -> bool:
-        return True
-
-    def _match_exact(self, other: Selector) -> bool:
-        return type(other) is Selector and self.path == self.path and self.pattern == other.pattern
-
-    def _match_exist(self, other: Selector) -> bool:
-        return set(self.pattern.items()).issubset(other.pattern.items())
-
-    def _match_fragment(self, other: Selector) -> bool:
-        fragment = list(self.pattern.items())
-        full = list(other.pattern.items())
-
-        try:
-            start = full.index(fragment[0])
-        except IndexError:
-            return True
-        except ValueError:
-            return False
-
-        return full[start : start + len(fragment)] == fragment
-
-    def _match_startswith(self, other: Selector) -> bool:
-        fragment = list(self.pattern.items())
-        full = list(other.pattern.items())
-
-        return all(fragment[i] == full[i] for i in range(len(fragment)))
-
-    def mix(self, path: str, **pattern: str) -> Self:
-        pattern = self.pattern | pattern
-        instance = self.__class__(mode=self.mode, path_excludes=self.path_excludes)
-
-        try:
-            instance.pattern = {each: pattern[each] for each in path.split(".")}
-        except KeyError:
-            raise ValueError(f"given information cannot mix with {path}") from None
-
-        return instance
-
-    def mixin(self, path: str, *selectors: Self) -> Self:
-        return self.mix(path, **ChainMap(*(x.pattern for x in selectors)))
-
-    def appendix(self, key: str, value: str) -> Self:
-        self.pattern[key] = value
-        return self
-
-    def copy(self) -> Self:
-        instance = self.__class__(mode=self.mode, path_excludes=self.path_excludes)
-        instance.pattern = self.pattern.copy()
-        return instance
-
-    def as_dyn(self) -> DynamicSelector:
-        instance = DynamicSelector(mode=self.mode, path_excludes=self.path_excludes)
-        for k, v in self.pattern.items():
-            getattr(instance, k)(v)
-        return instance
-
-    def set_referent(self, referent: Any) -> Self:
-        self.referent = referent
-        return self
-
-
-class DynamicSelector(Selector):
-    pattern: dict[str, Pattern]
-
-    def __getattr__(self, name: str, /):
-        def wrapper(content: Pattern | Literal["*"]):
-            if content == "*":
-                content = lambda _: True
-
-            self.pattern[name] = content
-            return self
-
-        return wrapper
-
-    def __hash__(self) -> int:
-        raise TypeError("Dynamic Selector is unhashable.")
-
-    __getitem__: Callable[[str], Pattern]
-
-    @classmethod
-    def way(cls, path: str) -> Selector:
-        instance = cls()
-        instance.pattern = {i: lambda _: True for i in path.split(".")}
-        return instance
-
-    def _match_exact(self, other: Selector) -> bool:
-        if isinstance(other, DynamicSelector):
-            raise TypeError("Can't match dynamic selector with another dynamic selector")
-        for k in other.pattern:
-            if k not in self.pattern:
-                return False
-            own_pattern = self.pattern[k]
-            if (
-                callable(own_pattern)
-                and not own_pattern(other.pattern[k])
-                or not callable(own_pattern)
-                and own_pattern != other.pattern[k]
-            ):
-                return False
-        return True
-
-    def _match_exist(self, other: Selector) -> bool:
-        for a, b in ((self.pattern[path], other.pattern[path]) for path in self.pattern):
-            if callable(a):
-                if callable(b):
-                    raise TypeError("Can't partially match dynamic selector with another dynamic selector")
-                elif not a(b):
-                    return False
-            elif a != b:
-                return False
-
-        return True
-
-    def _match_fragment(self, other: Selector) -> bool:
-        fragment = list(self.pattern)
-        full = list(other.pattern)
-
-        try:
-            start = full.index(fragment[0])
-        except IndexError:
-            return True
-        except ValueError:
-            return False
-
-        full = full[start : start + len(fragment)]
-        if fragment != full:
-            return False
-
-        for a, b in ((self.pattern[path], other.pattern[path]) for path in fragment):
-            if callable(a):
-                if callable(b):
-                    raise TypeError("Can't partially match dynamic selector with another dynamic selector")
-                elif not a(b):
-                    return False
-            elif a != b:
-                return False
-
-        return True
-
-    def _match_startswith(self, other: Selector) -> bool:
-        if not other.path.startswith(self.path):
-            return False
-
-        for a, b in ((self.pattern[path], other.pattern[path]) for path in self.pattern):
-            if callable(a):
-                if callable(b):
-                    raise TypeError("Can't partially match dynamic selector with another dynamic selector")
-                elif not a(b):
-                    return False
-            elif a != b:
-                return False
-
-        return True
-
-
-@runtime_checkable
-class Selectable(Protocol):
-    def to_selector(self) -> Selector:
-        ...
+from __future__ import annotations
+
+from collections import ChainMap
+from itertools import filterfalse
+from typing import TYPE_CHECKING, Any, Callable, Literal, Protocol, runtime_checkable
+
+from typing_extensions import Self
+
+from avilla.core.platform import Land
+
+if TYPE_CHECKING:
+    ...
+
+MatchRule = Literal["any", "exact", "exist", "fragment", "startswith"]
+Pattern = str | Callable[[str], bool]
+
+
+class Selector:
+    mode: MatchRule = "exact"
+    pattern: dict[str, str]
+    path_excludes: frozenset[str]
+    referent: Any = None
+
+    def __init__(self, *, mode: MatchRule = "exact", path_excludes: frozenset[str] = frozenset()) -> None:
+        self.mode = mode
+        self.path_excludes = path_excludes
+        self.pattern = {}
+
+    def __getattr__(self, name: str) -> Callable[[str], Self]:
+        def wrapper(content: str) -> Self:
+            self.pattern[name] = content
+            return self
+
+        return wrapper
+
+    def __hash__(self) -> int:
+        return hash("Selector") + hash(tuple(self.pattern.items()))
+
+    def __eq__(self, o: object) -> bool:
+        return isinstance(o, Selector) and o.pattern == self.pattern
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.pattern
+
+    def __getitem__(self, key: str) -> str:
+        return self.pattern[key]
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(mode={self.mode}).{'.'.join(f'{k}({v})' for k, v in self.pattern.items())}"
+
+    @property
+    def empty(self) -> bool:
+        return not self.pattern
+
+    @property
+    def path(self) -> str:
+        return ".".join(filterfalse(self.path_excludes.__contains__, self.pattern))
+
+    @property
+    def path_without_land(self) -> str:
+        return ".".join(filterfalse((self.path_excludes | {"land"}).__contains__, self.pattern))
+
+    @classmethod
+    def exist(cls) -> Self:
+        return cls(mode="exist")
+
+    @classmethod
+    def any(cls) -> Self:
+        return cls(mode="any")
+
+    @classmethod
+    def fragment(cls, *path_excludes: str) -> Self:
+        return cls(mode="fragment", path_excludes=frozenset(path_excludes))
+
+    @classmethod
+    def from_dict(cls, pattern: dict) -> Self:
+        instance = cls()
+        instance.pattern = pattern
+        return instance
+
+    @property
+    def latest_key(self) -> str:
+        return list(self.pattern.keys())[-1]
+
+    def land(self, land: Land | str):
+        if isinstance(land, Land):
+            land = land.name
+        self.pattern["land"] = land
+        return self
+
+    def match(self, other: Selectable) -> bool:
+        if not isinstance(other, Selector):
+            if not isinstance(other, Selectable):
+                return False
+            other = other.to_selector()
+        try:
+            match = {
+                "any": self._match_any,
+                "exact": self._match_exact,
+                "exist": self._match_exist,
+                "fragment": self._match_fragment,
+                "startswith": self._match_startswith,
+            }[self.mode]
+        except KeyError:
+            raise ValueError(f"Unknown match rule: {self.mode}") from None
+
+        return match(other)
+
+    def _match_any(self, other: Selector) -> bool:
+        return True
+
+    def _match_exact(self, other: Selector) -> bool:
+        return type(other) is Selector and self.path == other.path and self.pattern == other.pattern
+
+    def _match_exist(self, other: Selector) -> bool:
+        return set(self.pattern.items()).issubset(other.pattern.items())
+
+    def _match_fragment(self, other: Selector) -> bool:
+        fragment = list(self.pattern.items())
+        full = list(other.pattern.items())
+
+        try:
+            start = full.index(fragment[0])
+        except IndexError:
+            return True
+        except ValueError:
+            return False
+
+        return full[start : start + len(fragment)] == fragment
+
+    def _match_startswith(self, other: Selector) -> bool:
+        fragment = list(self.pattern.items())
+        full = list(other.pattern.items())
+
+        return all(fragment[i] == full[i] for i in range(len(fragment)))
+
+    def mix(self, path: str, **pattern: str) -> Self:
+        pattern = self.pattern | pattern
+        instance = self.__class__(mode=self.mode, path_excludes=self.path_excludes)
+
+        try:
+            instance.pattern = {each: pattern[each] for each in path.split(".")}
+        except KeyError:
+            raise ValueError(f"given information cannot mix with {path}") from None
+
+        return instance
+
+    def mixin(self, path: str, *selectors: Self) -> Self:
+        return self.mix(path, **ChainMap(*(x.pattern for x in selectors)))
+
+    def appendix(self, key: str, value: str) -> Self:
+        self.pattern[key] = value
+        return self
+
+    def copy(self) -> Self:
+        instance = self.__class__(mode=self.mode, path_excludes=self.path_excludes)
+        instance.pattern = self.pattern.copy()
+        return instance
+
+    def as_dyn(self) -> DynamicSelector:
+        instance = DynamicSelector(mode=self.mode, path_excludes=self.path_excludes)
+        for k, v in self.pattern.items():
+            getattr(instance, k)(v)
+        return instance
+
+    def to_selector(self):
+        return self
+
+    def follows(self, pattern: str) -> bool:
+        patterns: dict[str, str] = {}
+        bracket_depth: int = 0
+        path_buf: list[str] = []
+        pattern_buf: list[str] = []
+        for ch in pattern:
+            if ch == "." and bracket_depth == 0:
+                patterns["".join(path_buf)] = "".join(pattern_buf) or "*"
+                path_buf.clear()
+                pattern_buf.clear()
+            if ch == "(":
+                if bracket_depth:
+                    pattern_buf.append(ch)
+                bracket_depth += 1
+            elif ch == ")":
+                if not bracket_depth:
+                    raise ValueError
+                bracket_depth -= 1
+                if bracket_depth:
+                    pattern_buf.append(ch)
+            else:
+                (pattern_buf if bracket_depth else path_buf).append(ch)
+        if path_buf:
+            patterns["".join(path_buf)] = "".join(pattern_buf) or "*"
+        return (self.path if "land" in patterns else self.path_without_land) == ".".join(patterns) and all(
+            k in self.pattern and v in ["*", self.pattern[k]] for k, v in patterns.items()
+        )
+
+    def set_referent(self, referent: Any) -> Self:
+        self.referent = referent
+        return self
+
+
+class DynamicSelector(Selector):
+    pattern: dict[str, Pattern]
+
+    def __getattr__(self, name: str, /):
+        def wrapper(content: Pattern | Literal["*"]):
+            if content == "*":
+                content = lambda _: True
+
+            self.pattern[name] = content
+            return self
+
+        return wrapper
+
+    def __hash__(self) -> int:
+        raise TypeError("Dynamic Selector is unhashable.")
+
+    __getitem__: Callable[[str], Pattern]
+
+    @classmethod
+    def way(cls, path: str) -> Selector:
+        instance = cls()
+        instance.pattern = {i: lambda _: True for i in path.split(".")}
+        return instance
+
+    def _match_exact(self, other: Selector) -> bool:
+        if isinstance(other, DynamicSelector):
+            raise TypeError("Can't match dynamic selector with another dynamic selector")
+        for k in other.pattern:
+            if k not in self.pattern:
+                return False
+            own_pattern = self.pattern[k]
+            if (
+                callable(own_pattern)
+                and not own_pattern(other.pattern[k])
+                or not callable(own_pattern)
+                and own_pattern != other.pattern[k]
+            ):
+                return False
+        return True
+
+    def _match_exist(self, other: Selector) -> bool:
+        for a, b in ((self.pattern[path], other.pattern[path]) for path in self.pattern):
+            if callable(a):
+                if callable(b):
+                    raise TypeError("Can't partially match dynamic selector with another dynamic selector")
+                elif not a(b):
+                    return False
+            elif a != b:
+                return False
+
+        return True
+
+    def _match_fragment(self, other: Selector) -> bool:
+        fragment = list(self.pattern)
+        full = list(other.pattern)
+
+        try:
+            start = full.index(fragment[0])
+        except IndexError:
+            return True
+        except ValueError:
+            return False
+
+        full = full[start : start + len(fragment)]
+        if fragment != full:
+            return False
+
+        for a, b in ((self.pattern[path], other.pattern[path]) for path in fragment):
+            if callable(a):
+                if callable(b):
+                    raise TypeError("Can't partially match dynamic selector with another dynamic selector")
+                elif not a(b):
+                    return False
+            elif a != b:
+                return False
+
+        return True
+
+    def _match_startswith(self, other: Selector) -> bool:
+        if not other.path.startswith(self.path):
+            return False
+
+        for a, b in ((self.pattern[path], other.pattern[path]) for path in self.pattern):
+            if callable(a):
+                if callable(b):
+                    raise TypeError("Can't partially match dynamic selector with another dynamic selector")
+                elif not a(b):
+                    return False
+            elif a != b:
+                return False
+
+        return True
+
+
+@runtime_checkable
+class Selectable(Protocol):
+    def to_selector(self) -> Selector:
+        ...
```

### Comparing `avilla-core-1.0.0rc3/pyproject.toml` & `avilla-core-1.0.0rc4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avilla-core"
-version = "1.0.0rc3"
+version = "1.0.0rc4"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "graia-broadcast>=0.17.5",
     "graia-amnesia>=0.5.2",
     "loguru>=0.6.0",
@@ -25,31 +25,32 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=22.3.0",
     "flake8>=4.0.1",
     "isort>=5.10.1",
     "typing-extensions>=4.2.0",
     "graia-scheduler>=0.0.8",
-    "pdm-mina>=0.2.0",
     "mina-build>=0.2.6",
     "pre-commit>=2.20.0",
+    "devtools>=0.9.0",
+    "richuru>=0.1.1",
 ]
 
 [tool.mina]
 enabled = false
 
 [tool.mina.packages.core]
 includes = [
     "avilla/core",
     "avilla/core/py.typed",
 ]
 
 [tool.mina.packages.core.project]
 name = "avilla-core"
-version = "1.0.0rc3"
+version = "1.0.0rc4"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "graia-broadcast",
     "graia-amnesia",
     "loguru",
@@ -63,39 +64,37 @@
 [tool.mina.packages.core.project.license]
 text = "MIT"
 
 [tool.mina.packages.core.project.urls]
 homepage = "https://github.com/GraiaProject/Avilla"
 repository = "https://github.com/GraiaProject/Avilla"
 
-[tool.mina.packages.irc]
+[tool.mina.packages.elizabeth]
 includes = [
-    "avilla/irc",
+    "avilla/elizabeth",
 ]
 raw-dependencies = [
-    "avilla-core>=1.0.0rc3",
+    "avilla-core>=1.0.0rc4",
 ]
 
-[tool.mina.packages.irc.project]
-name = "avilla-irc"
-version = "1.0.0rc3"
+[tool.mina.packages.elizabeth.project]
+name = "avilla-elizabeth"
+version = "1.0.0rc4"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
-dependencies = [
-    "irc",
-]
+dependencies = []
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
-[tool.mina.packages.irc.project.license]
+[tool.mina.packages.elizabeth.project.license]
 text = "MIT"
 
-[tool.mina.packages.irc.project.urls]
+[tool.mina.packages.elizabeth.project.urls]
 homepage = "https://github.com/GraiaProject/Avilla"
 repository = "https://github.com/GraiaProject/Avilla"
 
 [tool.black]
 include = "\\.pyi?$"
 line-length = 120
 target-version = [
```

### Comparing `avilla-core-1.0.0rc3/PKG-INFO` & `avilla-core-1.0.0rc4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,112 @@
-Metadata-Version: 2.1
-Name: avilla-core
-Version: 1.0.0rc3
-License: MIT
-Author-email: GreyElaina <GreyElaina@outlook.com>
-Requires-Python: >=3.9
-Project-URL: homepage, https://github.com/GraiaProject/Avilla
-Project-URL: repository, https://github.com/GraiaProject/Avilla
-Description-Content-Type: text/markdown
-
-<div align="center">
-
-# Avilla
-
-_The next-gen framework for IM development._
-
-> 即刻动身, 踏上寻找第二个故乡的旅程.
-
-</div>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="code_style" />
-  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" />
-
-</p>
-
-Avilla 是 `Graia Project` 的 "下一代" 框架实现,
-通过对 [ `OneBot` ](https://github.com/botuniverse/onebot), [ `Telegram Bot API` ](https://core.telegram.org/bots) 及其他的基于不同即时通讯软件实现的各式对接接口,
-以及其他具有相应概念的 "异步消息流" 实例进行总结, 抽象其中最为基本的各式模型, 构造了一个理论上可以实现零成本切换对接平台的框架.
-
-**该框架目前处于快速迭代状态, API 可能会发生 _剧烈_ 变化, 可能还不适合进行生产性的开发与运维**
-
-> 项目名称取自日本轻小说 《魔女之旅》 的角色 "艾维莉亚(Avilla)".
-
-## Roadmap
-
-* `Avilla Protocol` : 对各式常见的行为进行抽象, 并通过可扩展的模型, 实现尽可能的功能可迁移性.
-  - 使用 [Launart](https://github.com/GraiaProject/Launart) 调度启动任务与应用实例的生命周期;
-  - 创新性的 Relationship 模型, 携带有进行任意操作所需的基本信息, 规范化行为模式与实现的编写;
-  - 使用 `Selector`, 实现了信息与对象本身的解耦, 减少平台实现的负担;
-  - 规范化的 `Resource` 抽象优化了对不同资源与资源类型的操作, 尤其是其内容的获取与其元信息的操作;
-  - 规范各式请求为 `Request`;
-  - 将各式元信息放缩为各个最小功能单元及其之间的组合, 不失表现性和可扩展性;
-  - 使用各式如 `Broadcast Control` 的注入入口, 极大简化了接口的使用;
-  - 复用来自 `Amnesia` 的通用接口;
-* And more...
-
-```py
-from creart import create
-from graia.amnesia.builtins.aiohttp import AiohttpService
-from graia.broadcast import Broadcast
-
-from avilla.core import Avilla, MessageReceived, Relationship, Selector
-from avilla.elizabeth.connection.config import WebsocketClientConfig
-from avilla.elizabeth.protocol import ElizabethProtocol
-
-broadcast = create(Broadcast)
-avilla = Avilla(broadcast, [
-    ElizabethProtocol(
-        WebsocketClientConfig("bot-account", "mah-verify-code")
-    )
-], [AiohttpService()])
-
-@broadcast.receiver(MessageReceived)
-async def on_message_received(event: MessageReceived, rs: Relationship):
-    if Selector.fragment().as_dyn().group("*").member("master-account").match(rs.ctx):
-        await rs.send_message("Hello, Avilla!")
-
-avilla.launch_manager.launch_blocking(loop=broadcast.loop)
-```
-
-## 部件发布情况
-
-|代号|协议|开发进度|PyPI|维护者|
-| :-: | :-: | :-: | :-: | :-: |
-|      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |
-| [Elizabeth](avilla/elizabeth) | `mirai-api-http` |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official |
-|    [-](avilla/onebot/v11)     |   `OneBot v11`   |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official |
-|    [-](avilla/onebot/v12)     |   `OneBot v12`   | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) | Official |
-|     [-](avilla/telegram)      |    `Telegram`    | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     |
-| [Nightcord](avilla/nightcord) |  `Discord Bots`  | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  | Official |
-
-## 我们的愿景
-
-创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
-助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
-
-## 相关项目
-
-<div align="center">
-
-星座的光芒是由一个个星点共同组成的, 任何优秀的作品都绝不会是一个人的功绩.  
-而若是没有这些项目, Avilla 的实现就无从谈起.  
-排名不分顺序, 可能有许遗漏, 这里仅列出部分较为重要的项目.
-
-</div>
-
-  + [ `Nonebot Team` ](https://github.com/nonebot):
-    - [ `Nonebot v2` ](https://github.com/nonebot/nonebot2): 同样是社区中赫赫有名的优秀框架.
-  + [ `Arclet Project` ](https://github.com/ArcletProject): 在借鉴的基础上, 还进行了难能可贵的优秀创新, 仍在不断成长的框架实现.
-  + [ `Mamoe Technologies` ](https://github.com/mamoe):
-    - [ `mirai` ](https://github.com/mamoe/mirai)
-    - [ `mirai-api-http` ](https://github.com/project-mirai/mirai-api-http)
-  + [ `OneBot Spec` ](https://github.com/botuniverse/onebot): Avilla for OneBot 所依据的实现规范, 同时也是 Avilla Protocol 设计时的参考之一.
-  + [ `go-cqhttp` ](https://github.com/Mrs4s/go-cqhttp): 可能是现在运用最为广泛的 OneBot v11 & v12 实现.
-
-无论如何, Avilla 都是 Graia Project 下的一个子项目, 以下项目均在不同层面上支持了 Avilla 的开发:
-  + [ `Broadcast Control` ](https://github.com/GraiaProject/BroadcastControl): 事件系统实现, 最为锋利的魔剑(Magic Sword).
-  + [ `Ariadne` ](https://github.com/GraiaProject/Ariadne): 继承了前作的衣钵, 在 Avilla 尚未成熟之际撑起大梁的后续作品, 同样进行了可贵的创新.
-
-<div align="center">
-
-衷心感谢这些以及其他未被提及的项目.
-
-</div>
-
-
-## 开源协议
-
-若非特殊说明, Avilla 及其子包默认使用 MIT 作为开源协议, 但如果你若引用到了使用 GPL/AGPL/LGPL 等具有传染性开源协议的项目, 无论是对 Avilla 实现或是使用了相应 Avilla 实现的项目仍需要遵循相关规则.
-
+<div align="center">
+
+# Avilla
+
+_The next-gen framework for IM development._
+
+> 即刻动身, 踏上寻找第二个故乡的旅程.
+
+</div>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="code_style" />
+  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" />
+
+</p>
+
+Avilla 是 `Graia Project` 的 "下一代" 框架实现,
+通过对 [ `OneBot` ](https://github.com/botuniverse/onebot), [ `Telegram Bot API` ](https://core.telegram.org/bots) 及其他的基于不同即时通讯软件实现的各式对接接口,
+以及其他具有相应概念的 "异步消息流" 实例进行总结, 抽象其中最为基本的各式模型, 构造了一个理论上可以实现零成本切换对接平台的框架.
+
+**该框架目前处于快速迭代状态, API 可能会发生 _剧烈_ 变化, 可能还不适合进行生产性的开发与运维**
+
+> 项目名称取自日本轻小说 《魔女之旅》 的角色 "艾维莉亚(Avilla)".
+
+|Docs|[![docs](https://img.shields.io/badge/docs%20on-readthedocs-black)](https://graia.readthedocs.io/)|[![docs](https://img.shields.io/badge/docs%20on-netlify-informational)](https://graia.netlify.app/)|[![docs](https://img.shields.io/badge/docs%20on-cloudflare-orange)](https://graia.pages.dev/)|
+|:-:|:-:|:-:|:-:|
+
+## Notable Features
+
+ - **原生跨平台**: 开创性的 Relationship 操作模型, 配合最小功能单元, 行为扩展等诸多独特设计, 无论是简单的消息收发还是平台设计的独特交互, Avilla 都能处理地得心应手.
+ - **原生多账号**: Avilla 在设计之初, 就考虑了同时管理多个账号, 甚至是多个平台上的多个账号这些问题, 并加以研究与解决. 而现在, 账号管理本应如此简单便捷而收放自如.
+ - **一次编写, 多平台可用**: 得益于 Avilla 的强大抽象, 开发者只需面向 Avilla 就能完成核心业务的开发, 显著的减少了维护成本.
+ - **平台特性友好**: Avilla 以 Activity, Reaction, Extension 等诸项设计, 使得开发者在运用平台特性的方式更加规范而不失表达性. 担心平台间特性的不通用? 你可以同时为多个平台编写不同的特性用例, Avilla 会自动应用可用的适配, 不改动核心逻辑的同时保证基本特性的可用!
+  > 担心可用性? 我们同样提供了一些核心的非平台依赖实现, 例如 `TextCommand`, 这些组件仅要求平台实现最基本的交互实现, 剩下的一切交给 Avilla 处理!
+ - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
+ - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
+
+## Quick Start
+
+```py
+from creart import create
+from graia.amnesia.builtins.aiohttp import AiohttpService
+from graia.broadcast import Broadcast
+
+from avilla.core import Avilla, MessageReceived, Relationship, Selector
+from avilla.elizabeth.connection.config import WebsocketClientConfig
+from avilla.elizabeth.protocol import ElizabethProtocol
+
+broadcast = create(Broadcast)
+avilla = Avilla(broadcast, [
+    ElizabethProtocol(
+        WebsocketClientConfig("bot-account", "mah-verify-code")
+    )
+], [AiohttpService()])
+
+@broadcast.receiver(MessageReceived)
+async def on_message_received(event: MessageReceived, rs: Relationship):
+    if Selector.fragment().as_dyn().group("*").member("master-account").match(rs.ctx):
+        await rs.send_message("Hello, Avilla!")
+
+avilla.launch_manager.launch_blocking(loop=broadcast.loop)
+```
+
+## 部件发布情况
+
+|代号|协议|开发进度|PyPI|维护者|开源协议|
+| :-: | :-: | :-: | :-: | :-: | :-: |
+|      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |MIT|
+| [Elizabeth](avilla/elizabeth) | `mirai-api-http` |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official |AGPLv3|
+|    [-](avilla/onebot/v11)     |   `OneBot v11`   |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official | - |
+|    [-](avilla/onebot/v12)     |   `OneBot v12`   | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) | Official | - |
+|     [-](avilla/telegram)      |    `Telegram`    | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     | - |
+| [Nightcord](avilla/nightcord) |  `Discord Bots`  | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  | Official | - |
+
+## 我们的愿景
+
+创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
+助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
+
+## 相关项目
+
+<div align="center">
+
+星座的光芒是由一个个星点共同组成的, 任何优秀的作品都绝不会是一个人的功绩.  
+而若是没有这些项目, Avilla 的实现就无从谈起.  
+排名不分顺序, 可能有许遗漏, 这里仅列出部分较为重要的项目.
+
+</div>
+
+  + [ `Nonebot Team` ](https://github.com/nonebot):
+    - [ `Nonebot v2` ](https://github.com/nonebot/nonebot2): 同样是社区中赫赫有名的优秀框架.
+  + [ `Arclet Project` ](https://github.com/ArcletProject): 在借鉴的基础上, 还进行了难能可贵的优秀创新, 仍在不断成长的框架实现.
+  + [ `Mamoe Technologies` ](https://github.com/mamoe):
+    - [ `mirai` ](https://github.com/mamoe/mirai)
+    - [ `mirai-api-http` ](https://github.com/project-mirai/mirai-api-http)
+  + [ `OneBot Spec` ](https://github.com/botuniverse/onebot): Avilla for OneBot 所依据的实现规范, 同时也是 Avilla Protocol 设计时的参考之一.
+  + [ `go-cqhttp` ](https://github.com/Mrs4s/go-cqhttp): 可能是现在运用最为广泛的 OneBot v11 & v12 实现.
+
+无论如何, Avilla 都是 Graia Project 下的一个子项目, 以下项目均在不同层面上支持了 Avilla 的开发:
+  + [ `Broadcast Control` ](https://github.com/GraiaProject/BroadcastControl): 事件系统实现, 最为锋利的魔剑(Magic Sword).
+  + [ `Ariadne` ](https://github.com/GraiaProject/Ariadne): 继承了前作的衣钵, 在 Avilla 尚未成熟之际撑起大梁的后续作品, 同样进行了可贵的创新.
+
+<div align="center">
+
+衷心感谢这些以及其他未被提及的项目.
+
+</div>
+
+
+## 开源协议
+
+若非特殊说明, Avilla 及其子包默认使用 MIT 作为开源协议, 但如果你若引用到了使用 GPL/AGPL/LGPL 等具有传染性开源协议的项目, 无论是对 Avilla 实现或是使用了相应 Avilla 实现的项目仍需要遵循相关规则.
```

