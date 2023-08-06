# Comparing `tmp/runtimepy-1.7.2.tar.gz` & `tmp/runtimepy-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.7.2.tar", last modified: Fri Jun 30 07:48:13 2023, max compression
+gzip compressed data, was "runtimepy-1.7.3.tar", last modified: Sun Aug  6 07:16:19 2023, max compression
```

## Comparing `runtimepy-1.7.2.tar` & `runtimepy-1.7.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.238222 runtimepy-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 07:46:27.000000 runtimepy-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-30 07:48:13.238222 runtimepy-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 07:46:27.000000 runtimepy-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-30 07:46:27.000000 runtimepy-1.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.222220 runtimepy-1.7.2/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.222220 runtimepy-1.7.2/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.222220 runtimepy-1.7.2/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.222220 runtimepy-1.7.2/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.226220 runtimepy-1.7.2/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.226220 runtimepy-1.7.2/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.214219 runtimepy-1.7.2/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.226220 runtimepy-1.7.2/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.226220 runtimepy-1.7.2/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.226220 runtimepy-1.7.2/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/housekeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.230221 runtimepy-1.7.2/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.234221 runtimepy-1.7.2/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.238222 runtimepy-1.7.2/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/task/basic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/task/basic/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.238222 runtimepy-1.7.2/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.238222 runtimepy-1.7.2/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.238222 runtimepy-1.7.2/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 07:46:27.000000 runtimepy-1.7.2/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.222220 runtimepy-1.7.2/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-30 07:48:13.000000 runtimepy-1.7.2/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-30 07:48:13.000000 runtimepy-1.7.2/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:48:13.000000 runtimepy-1.7.2/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 07:48:13.000000 runtimepy-1.7.2/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 07:48:13.000000 runtimepy-1.7.2/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 07:48:13.000000 runtimepy-1.7.2/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 07:48:13.238222 runtimepy-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-30 07:46:27.000000 runtimepy-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:48:13.238222 runtimepy-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 07:46:27.000000 runtimepy-1.7.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 07:46:27.000000 runtimepy-1.7.2/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 07:46:27.000000 runtimepy-1.7.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.662706 runtimepy-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:13:25.000000 runtimepy-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-06 07:16:19.662706 runtimepy-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-06 07:13:25.000000 runtimepy-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-06 07:13:25.000000 runtimepy-1.7.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.642706 runtimepy-1.7.3/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.642706 runtimepy-1.7.3/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.646705 runtimepy-1.7.3/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.646705 runtimepy-1.7.3/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.646705 runtimepy-1.7.3/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.646705 runtimepy-1.7.3/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.638706 runtimepy-1.7.3/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.650705 runtimepy-1.7.3/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.650705 runtimepy-1.7.3/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.650705 runtimepy-1.7.3/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.650705 runtimepy-1.7.3/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.650705 runtimepy-1.7.3/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/housekeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.654706 runtimepy-1.7.3/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.658706 runtimepy-1.7.3/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/task/basic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/task/basic/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.662706 runtimepy-1.7.3/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.662706 runtimepy-1.7.3/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.662706 runtimepy-1.7.3/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-06 07:13:25.000000 runtimepy-1.7.3/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.642706 runtimepy-1.7.3/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-06 07:16:19.000000 runtimepy-1.7.3/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-06 07:16:19.000000 runtimepy-1.7.3/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:16:19.000000 runtimepy-1.7.3/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 07:16:19.000000 runtimepy-1.7.3/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-06 07:16:19.000000 runtimepy-1.7.3/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 07:16:19.000000 runtimepy-1.7.3/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:16:19.662706 runtimepy-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-06 07:13:25.000000 runtimepy-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:19.662706 runtimepy-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-06 07:13:25.000000 runtimepy-1.7.3/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-06 07:13:25.000000 runtimepy-1.7.3/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 07:13:25.000000 runtimepy-1.7.3/tests/test_resources.py
```

### Comparing `runtimepy-1.7.2/LICENSE` & `runtimepy-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/PKG-INFO` & `runtimepy-1.7.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.7.2
+Version: 1.7.3
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,30 +21,36 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=dcf2c1807c7b51c3ecf85165da8ba116
+    hash=817cf762c796141c0bcef9a9834f06ac
     =====================================
 -->
 
-# runtimepy ([1.7.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.3](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
 *A framework for implementing Python services.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/runtimepy.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/runtimepy)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/runtimepy.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
```

### Comparing `runtimepy-1.7.2/README.md` & `runtimepy-1.7.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=dcf2c1807c7b51c3ecf85165da8ba116
+    hash=817cf762c796141c0bcef9a9834f06ac
     =====================================
 -->
 
-# runtimepy ([1.7.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.3](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
 *A framework for implementing Python services.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/runtimepy.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/runtimepy)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/runtimepy.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
```

### Comparing `runtimepy-1.7.2/pyproject.toml` & `runtimepy-1.7.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.7.2"
+version = "1.7.3"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
@@ -33,14 +33,16 @@
   "pylint",
   "flake8",
   "black",
   "ruff",
   "mypy",
   "isort",
   "yamllint",
+  "yambs",
+  "vmklib",
   "pytest-asyncio",
   "setuptools-wrapper",
   "types-setuptools"
 ]
 
 [project.scripts]
 runtimepy = "runtimepy.entry:main"
```

### Comparing `runtimepy-1.7.2/runtimepy/app.py` & `runtimepy-1.7.3/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/__init__.py` & `runtimepy-1.7.3/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/environment/__init__.py` & `runtimepy-1.7.3/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/environment/array.py` & `runtimepy-1.7.3/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/environment/base.py` & `runtimepy-1.7.3/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/environment/create.py` & `runtimepy-1.7.3/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/environment/file.py` & `runtimepy-1.7.3/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/environment/names.py` & `runtimepy-1.7.3/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/channel/registry.py` & `runtimepy-1.7.3/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/codec/protocol/base.py` & `runtimepy-1.7.3/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/codec/protocol/json.py` & `runtimepy-1.7.3/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/commands/all.py` & `runtimepy-1.7.3/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/commands/arbiter.py` & `runtimepy-1.7.3/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/commands/tui.py` & `runtimepy-1.7.3/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.7.3/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.7.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/entry.py` & `runtimepy-1.7.3/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/enum/__init__.py` & `runtimepy-1.7.3/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/enum/registry.py` & `runtimepy-1.7.3/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/enum/type.py` & `runtimepy-1.7.3/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/mapping.py` & `runtimepy-1.7.3/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/mixins/enum.py` & `runtimepy-1.7.3/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/mixins/regex.py` & `runtimepy-1.7.3/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/__init__.py` & `runtimepy-1.7.3/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/__init__.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/base.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/config.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/config.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/factory/task.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/imports.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/info.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/task.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/udp.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.7.3/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/connection.py` & `runtimepy-1.7.3/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/factories/__init__.py` & `runtimepy-1.7.3/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/manager.py` & `runtimepy-1.7.3/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/metrics.py` & `runtimepy-1.7.3/runtimepy/net/metrics.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/mixin.py` & `runtimepy-1.7.3/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/tcp/connection.py` & `runtimepy-1.7.3/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.7.3/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.7.3/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/udp/connection.py` & `runtimepy-1.7.3/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/util.py` & `runtimepy-1.7.3/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/net/websocket/connection.py` & `runtimepy-1.7.3/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/__init__.py` & `runtimepy-1.7.3/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/array.py` & `runtimepy-1.7.3/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/base.py` & `runtimepy-1.7.3/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/bool.py` & `runtimepy-1.7.3/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/byte_order.py` & `runtimepy-1.7.3/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/field/__init__.py` & `runtimepy-1.7.3/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/field/fields.py` & `runtimepy-1.7.3/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.7.3/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.7.3/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/float.py` & `runtimepy-1.7.3/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/int.py` & `runtimepy-1.7.3/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/string.py` & `runtimepy-1.7.3/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/type/__init__.py` & `runtimepy-1.7.3/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/type/base.py` & `runtimepy-1.7.3/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/type/float.py` & `runtimepy-1.7.3/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/primitives/type/int.py` & `runtimepy-1.7.3/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/registry/__init__.py` & `runtimepy-1.7.3/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/registry/bool.py` & `runtimepy-1.7.3/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/registry/item.py` & `runtimepy-1.7.3/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/registry/name.py` & `runtimepy-1.7.3/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/schemas.py` & `runtimepy-1.7.3/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/task/asynchronous.py` & `runtimepy-1.7.3/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/task/basic/manager.py` & `runtimepy-1.7.3/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/task/basic/metrics.py` & `runtimepy-1.7.3/runtimepy/task/basic/metrics.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/task/basic/periodic.py` & `runtimepy-1.7.3/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/tui/channels/__init__.py` & `runtimepy-1.7.3/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy/tui/task.py` & `runtimepy-1.7.3/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.7.3/runtimepy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.7.2
+Version: 1.7.3
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,30 +21,36 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=dcf2c1807c7b51c3ecf85165da8ba116
+    hash=817cf762c796141c0bcef9a9834f06ac
     =====================================
 -->
 
-# runtimepy ([1.7.2](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.3](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
 *A framework for implementing Python services.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/runtimepy.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/runtimepy)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/runtimepy.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
```

### Comparing `runtimepy-1.7.2/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.7.3/runtimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/setup.py` & `runtimepy-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/tests/test_entry.py` & `runtimepy-1.7.3/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.2/tests/test_mapping.py` & `runtimepy-1.7.3/tests/test_mapping.py`

 * *Files identical despite different names*

