# Comparing `tmp/wonda-0.6.0a1.tar.gz` & `tmp/wonda-0.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonda-0.6.0a1.tar", max compression
+gzip compressed data, was "wonda-0.6.0a2.tar", max compression
```

## Comparing `wonda-0.6.0a1.tar` & `wonda-0.6.0a2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1131 2023-01-08 13:20:34.909130 wonda-0.6.0a1/LICENSE
--rw-r--r--   0        0        0     2177 2023-08-01 13:12:06.355095 wonda-0.6.0a1/README.md
--rw-r--r--   0        0        0      542 2023-08-01 14:00:48.639524 wonda-0.6.0a1/pyproject.toml
--rw-r--r--   0        0        0      356 2023-08-01 13:12:06.359212 wonda-0.6.0a1/wonda/__init__.py
--rw-r--r--   0        0        0      220 2023-08-01 14:26:17.698469 wonda-0.6.0a1/wonda/api/__init__.py
--rw-r--r--   0        0        0     1941 2023-08-01 14:34:12.037508 wonda-0.6.0a1/wonda/api/abc.py
--rw-r--r--   0        0        0     1282 2023-08-01 14:36:44.589394 wonda-0.6.0a1/wonda/api/api.py
--rw-r--r--   0        0        0       68 2023-08-01 14:15:25.890716 wonda-0.6.0a1/wonda/api/response.py
--rw-r--r--   0        0        0       58 2023-07-09 17:08:19.452596 wonda-0.6.0a1/wonda/api/utils/__init__.py
--rw-r--r--   0        0        0      631 2023-08-01 13:12:06.360196 wonda-0.6.0a1/wonda/api/utils/file_util.py
--rw-r--r--   0        0        0     1076 2023-08-01 14:04:17.058304 wonda-0.6.0a1/wonda/api/utils/token_util.py
--rw-r--r--   0        0        0      253 2023-08-01 13:32:22.879290 wonda-0.6.0a1/wonda/api/validators/__init__.py
--rw-r--r--   0        0        0      327 2023-08-01 14:34:07.149011 wonda-0.6.0a1/wonda/api/validators/abc.py
--rw-r--r--   0        0        0      831 2023-08-01 14:39:32.506796 wonda-0.6.0a1/wonda/api/validators/request.py
--rw-r--r--   0        0        0      713 2023-08-01 14:20:27.832088 wonda-0.6.0a1/wonda/api/validators/response.py
--rw-r--r--   0        0        0      559 2023-08-01 13:12:06.361697 wonda-0.6.0a1/wonda/bot/__init__.py
--rw-r--r--   0        0        0      324 2023-08-01 13:16:13.482655 wonda-0.6.0a1/wonda/bot/abc.py
--rw-r--r--   0        0        0       68 2023-08-01 13:12:06.362105 wonda-0.6.0a1/wonda/bot/blueprint/__init__.py
--rw-r--r--   0        0        0      616 2023-08-01 13:19:08.503857 wonda-0.6.0a1/wonda/bot/blueprint/abc.py
--rw-r--r--   0        0        0      817 2023-08-01 13:16:13.828698 wonda-0.6.0a1/wonda/bot/blueprint/default.py
--rw-r--r--   0        0        0     2219 2023-08-01 13:16:13.736400 wonda-0.6.0a1/wonda/bot/bot.py
--rw-r--r--   0        0        0      212 2023-08-01 13:16:13.736421 wonda-0.6.0a1/wonda/bot/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-08-01 13:16:13.828532 wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/__init__.py
--rw-r--r--   0        0        0      510 2023-08-01 13:16:13.839652 wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/abc.py
--rw-r--r--   0        0        0     1115 2023-08-01 13:16:13.828518 wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/default.py
--rw-r--r--   0        0        0       58 2023-08-01 13:12:06.387599 wonda-0.6.0a1/wonda/bot/dispatch/handler/__init__.py
--rw-r--r--   0        0        0      391 2023-08-01 13:12:06.387736 wonda-0.6.0a1/wonda/bot/dispatch/handler/abc.py
--rw-r--r--   0        0        0     1219 2023-08-01 13:12:06.387872 wonda-0.6.0a1/wonda/bot/dispatch/handler/func.py
--rw-r--r--   0        0        0       78 2023-08-01 13:12:06.362854 wonda-0.6.0a1/wonda/bot/dispatch/middlewares/__init__.py
--rw-r--r--   0        0        0      406 2023-08-01 13:12:06.388025 wonda-0.6.0a1/wonda/bot/dispatch/middlewares/abc.py
--rw-r--r--   0        0        0       62 2023-08-01 13:12:06.363015 wonda-0.6.0a1/wonda/bot/dispatch/router/__init__.py
--rw-r--r--   0        0        0      637 2023-08-01 14:10:44.271381 wonda-0.6.0a1/wonda/bot/dispatch/router/abc.py
--rw-r--r--   0        0        0     1072 2023-08-01 13:12:06.388166 wonda-0.6.0a1/wonda/bot/dispatch/router/default.py
--rw-r--r--   0        0        0      110 2023-08-01 13:12:06.363412 wonda-0.6.0a1/wonda/bot/dispatch/view/__init__.py
--rw-r--r--   0        0        0     3533 2023-08-01 13:39:56.214935 wonda-0.6.0a1/wonda/bot/dispatch/view/abc.py
--rw-r--r--   0        0        0     2103 2023-08-01 13:18:52.420643 wonda-0.6.0a1/wonda/bot/dispatch/view/impl.py
--rw-r--r--   0        0        0       56 2023-04-21 11:36:28.382086 wonda-0.6.0a1/wonda/bot/polling/__init__.py
--rw-r--r--   0        0        0      464 2023-08-01 13:12:06.364052 wonda-0.6.0a1/wonda/bot/polling/abc.py
--rw-r--r--   0        0        0     1211 2023-08-01 13:12:06.364287 wonda-0.6.0a1/wonda/bot/polling/bot.py
--rw-r--r--   0        0        0      129 2023-08-01 13:12:06.364526 wonda-0.6.0a1/wonda/bot/rules/__init__.py
--rw-r--r--   0        0        0     1816 2023-08-01 14:48:49.174835 wonda-0.6.0a1/wonda/bot/rules/abc.py
--rw-r--r--   0        0        0     4437 2023-08-01 13:50:29.499615 wonda-0.6.0a1/wonda/bot/rules/base.py
--rw-r--r--   0        0        0     5537 2023-08-01 13:12:06.365118 wonda-0.6.0a1/wonda/bot/rules/message.py
--rw-r--r--   0        0        0      125 2023-08-01 13:12:06.365285 wonda-0.6.0a1/wonda/bot/states/__init__.py
--rw-r--r--   0        0        0       78 2023-08-01 13:12:06.365455 wonda-0.6.0a1/wonda/bot/states/dispenser/__init__.py
--rw-r--r--   0        0        0      822 2023-08-01 13:12:06.365624 wonda-0.6.0a1/wonda/bot/states/dispenser/abc.py
--rw-r--r--   0        0        0      832 2023-08-01 13:12:06.365811 wonda-0.6.0a1/wonda/bot/states/dispenser/default.py
--rw-r--r--   0        0        0      574 2023-08-01 13:12:06.365978 wonda-0.6.0a1/wonda/bot/states/types.py
--rw-r--r--   0        0        0      636 2023-08-01 13:12:06.366161 wonda-0.6.0a1/wonda/bot/updates/__init__.py
--rw-r--r--   0        0        0      135 2023-08-01 13:12:06.366317 wonda-0.6.0a1/wonda/bot/updates/base.py
--rw-r--r--   0        0        0     5287 2023-08-01 13:12:50.665638 wonda-0.6.0a1/wonda/bot/updates/types.py
--rw-r--r--   0        0        0        0 2022-12-09 12:31:48.203870 wonda-0.6.0a1/wonda/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:12:06.388351 wonda-0.6.0a1/wonda/contrib/middleware/__init__.py
--rw-r--r--   0        0        0        0 2022-12-09 12:31:48.204053 wonda-0.6.0a1/wonda/contrib/rules/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 19:17:57.296559 wonda-0.6.0a1/wonda/contrib/storage/__init__.py
--rw-r--r--   0        0        0     1475 2023-08-01 13:12:06.388804 wonda-0.6.0a1/wonda/contrib/storage/redis.py
--rw-r--r--   0        0        0      298 2023-08-01 13:12:06.366842 wonda-0.6.0a1/wonda/errors/__init__.py
--rw-r--r--   0        0        0      269 2023-08-01 13:12:06.367058 wonda-0.6.0a1/wonda/errors/base_exceptions.py
--rw-r--r--   0        0        0     1635 2023-08-01 14:03:19.646417 wonda-0.6.0a1/wonda/errors/code_exception.py
--rw-r--r--   0        0        0       73 2023-04-21 11:36:28.384533 wonda-0.6.0a1/wonda/errors/error_handler/__init__.py
--rw-r--r--   0        0        0      704 2023-08-01 13:12:06.367251 wonda-0.6.0a1/wonda/errors/error_handler/abc.py
--rw-r--r--   0        0        0     2031 2023-08-01 13:12:06.367470 wonda-0.6.0a1/wonda/errors/error_handler/error_handler.py
--rw-r--r--   0        0        0      533 2023-08-01 14:27:57.256711 wonda-0.6.0a1/wonda/modules.py
--rw-r--r--   0        0        0       76 2023-08-01 13:12:06.389026 wonda-0.6.0a1/wonda/net/__init__.py
--rw-r--r--   0        0        0      799 2023-08-01 13:12:06.389181 wonda-0.6.0a1/wonda/net/abc.py
--rw-r--r--   0        0        0     1960 2023-08-01 14:28:02.359184 wonda-0.6.0a1/wonda/net/default.py
--rw-r--r--   0        0        0      123 2023-08-01 13:12:06.368301 wonda-0.6.0a1/wonda/tools/__init__.py
--rw-r--r--   0        0        0      551 2023-08-01 13:12:06.368500 wonda-0.6.0a1/wonda/tools/delayed_task.py
--rw-r--r--   0        0        0      284 2023-08-01 13:12:06.368688 wonda-0.6.0a1/wonda/tools/keyboard/__init__.py
--rw-r--r--   0        0        0      704 2023-08-01 13:12:06.368872 wonda-0.6.0a1/wonda/tools/keyboard/abc.py
--rw-r--r--   0        0        0     2889 2023-08-01 14:46:49.980391 wonda-0.6.0a1/wonda/tools/keyboard/builder.py
--rw-r--r--   0        0        0     5281 2023-08-01 13:12:06.389685 wonda-0.6.0a1/wonda/tools/keyboard/elements.py
--rw-r--r--   0        0        0     2603 2023-08-01 14:08:40.080104 wonda-0.6.0a1/wonda/tools/loop_wrapper.py
--rw-r--r--   0        0        0      174 2023-08-01 13:12:06.369277 wonda-0.6.0a1/wonda/tools/storage/__init__.py
--rw-r--r--   0        0        0      648 2023-08-01 13:12:06.369452 wonda-0.6.0a1/wonda/tools/storage/abc.py
--rw-r--r--   0        0        0     1861 2023-08-01 13:12:06.369619 wonda-0.6.0a1/wonda/tools/storage/memory.py
--rw-r--r--   0        0        0      132 2023-08-01 13:12:06.369784 wonda-0.6.0a1/wonda/tools/storage/types.py
--rw-r--r--   0        0        0       73 2023-02-27 18:52:52.469528 wonda-0.6.0a1/wonda/tools/text/__init__.py
--rw-r--r--   0        0        0       29 2023-02-27 18:52:54.495531 wonda-0.6.0a1/wonda/tools/text/formatting/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-27 18:52:47.941301 wonda-0.6.0a1/wonda/tools/text/formatting/html.py
--rw-r--r--   0        0        0     2761 2023-02-27 18:52:50.221309 wonda-0.6.0a1/wonda/tools/text/formatting/markdown.py
--rw-r--r--   0        0        0       93 2022-12-09 12:31:48.210068 wonda-0.6.0a1/wonda/tools/text/parse_mode.py
--rw-r--r--   0        0        0       55 2023-02-01 05:24:13.893095 wonda-0.6.0a1/wonda/types/__init__.py
--rw-r--r--   0        0        0     4438 2023-08-01 13:13:03.042503 wonda-0.6.0a1/wonda/types/enums.py
--rw-r--r--   0        0        0      451 2023-08-01 13:12:06.389838 wonda-0.6.0a1/wonda/types/helper.py
--rw-r--r--   0        0        0    78297 2023-08-01 14:19:52.164954 wonda-0.6.0a1/wonda/types/methods.py
--rw-r--r--   0        0        0    59280 2023-08-01 13:13:37.342354 wonda-0.6.0a1/wonda/types/objects.py
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 wonda-0.6.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-01-08 13:20:34.909130 wonda-0.6.0a2/LICENSE
+-rw-r--r--   0        0        0     2177 2023-08-01 13:12:06.355095 wonda-0.6.0a2/README.md
+-rw-r--r--   0        0        0      542 2023-08-05 22:39:20.696026 wonda-0.6.0a2/pyproject.toml
+-rw-r--r--   0        0        0      356 2023-08-01 13:12:06.359212 wonda-0.6.0a2/wonda/__init__.py
+-rw-r--r--   0        0        0      220 2023-08-01 14:26:17.698469 wonda-0.6.0a2/wonda/api/__init__.py
+-rw-r--r--   0        0        0     1927 2023-08-03 09:50:01.190006 wonda-0.6.0a2/wonda/api/abc.py
+-rw-r--r--   0        0        0     1275 2023-08-05 19:40:21.588287 wonda-0.6.0a2/wonda/api/api.py
+-rw-r--r--   0        0        0       68 2023-08-01 14:15:25.890716 wonda-0.6.0a2/wonda/api/response.py
+-rw-r--r--   0        0        0       58 2023-07-09 17:08:19.452596 wonda-0.6.0a2/wonda/api/utils/__init__.py
+-rw-r--r--   0        0        0      610 2023-08-02 09:44:34.167419 wonda-0.6.0a2/wonda/api/utils/file_util.py
+-rw-r--r--   0        0        0     1076 2023-08-05 22:37:19.630447 wonda-0.6.0a2/wonda/api/utils/token_util.py
+-rw-r--r--   0        0        0      253 2023-08-01 13:32:22.879290 wonda-0.6.0a2/wonda/api/validators/__init__.py
+-rw-r--r--   0        0        0      299 2023-08-03 09:49:56.572577 wonda-0.6.0a2/wonda/api/validators/abc.py
+-rw-r--r--   0        0        0      671 2023-08-05 22:40:15.626483 wonda-0.6.0a2/wonda/api/validators/request.py
+-rw-r--r--   0        0        0      713 2023-08-02 09:55:43.097743 wonda-0.6.0a2/wonda/api/validators/response.py
+-rw-r--r--   0        0        0      564 2023-08-05 22:14:36.212013 wonda-0.6.0a2/wonda/bot/__init__.py
+-rw-r--r--   0        0        0      323 2023-08-05 20:24:36.981966 wonda-0.6.0a2/wonda/bot/abc.py
+-rw-r--r--   0        0        0       68 2023-08-05 22:14:36.255732 wonda-0.6.0a2/wonda/bot/blueprint/__init__.py
+-rw-r--r--   0        0        0      622 2023-08-05 22:37:58.295875 wonda-0.6.0a2/wonda/bot/blueprint/abc.py
+-rw-r--r--   0        0        0      817 2023-08-05 22:14:36.255937 wonda-0.6.0a2/wonda/bot/blueprint/default.py
+-rw-r--r--   0        0        0     2196 2023-08-05 22:39:01.445239 wonda-0.6.0a2/wonda/bot/bot.py
+-rw-r--r--   0        0        0      212 2023-08-01 13:16:13.736421 wonda-0.6.0a2/wonda/bot/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-01 13:16:13.828532 wonda-0.6.0a2/wonda/bot/dispatch/dispatcher/__init__.py
+-rw-r--r--   0        0        0      333 2023-08-03 10:01:04.474641 wonda-0.6.0a2/wonda/bot/dispatch/dispatcher/abc.py
+-rw-r--r--   0        0        0     1115 2023-08-05 22:38:33.689046 wonda-0.6.0a2/wonda/bot/dispatch/dispatcher/default.py
+-rw-r--r--   0        0        0       58 2023-08-01 13:12:06.387599 wonda-0.6.0a2/wonda/bot/dispatch/handler/__init__.py
+-rw-r--r--   0        0        0      391 2023-08-01 13:12:06.387736 wonda-0.6.0a2/wonda/bot/dispatch/handler/abc.py
+-rw-r--r--   0        0        0     1219 2023-08-05 22:38:35.651178 wonda-0.6.0a2/wonda/bot/dispatch/handler/func.py
+-rw-r--r--   0        0        0       78 2023-08-01 13:12:06.362854 wonda-0.6.0a2/wonda/bot/dispatch/middlewares/__init__.py
+-rw-r--r--   0        0        0      406 2023-08-01 13:12:06.388025 wonda-0.6.0a2/wonda/bot/dispatch/middlewares/abc.py
+-rw-r--r--   0        0        0       62 2023-08-01 13:12:06.363015 wonda-0.6.0a2/wonda/bot/dispatch/router/__init__.py
+-rw-r--r--   0        0        0      637 2023-08-01 14:10:44.271381 wonda-0.6.0a2/wonda/bot/dispatch/router/abc.py
+-rw-r--r--   0        0        0     1072 2023-08-01 13:12:06.388166 wonda-0.6.0a2/wonda/bot/dispatch/router/default.py
+-rw-r--r--   0        0        0      110 2023-08-01 13:12:06.363412 wonda-0.6.0a2/wonda/bot/dispatch/view/__init__.py
+-rw-r--r--   0        0        0     3533 2023-08-05 22:13:59.602475 wonda-0.6.0a2/wonda/bot/dispatch/view/abc.py
+-rw-r--r--   0        0        0     2103 2023-08-01 13:18:52.420643 wonda-0.6.0a2/wonda/bot/dispatch/view/impl.py
+-rw-r--r--   0        0        0       62 2023-08-05 20:27:52.464488 wonda-0.6.0a2/wonda/bot/polling/__init__.py
+-rw-r--r--   0        0        0      457 2023-08-05 20:24:36.958931 wonda-0.6.0a2/wonda/bot/polling/abc.py
+-rw-r--r--   0        0        0     1509 2023-08-05 20:27:53.959327 wonda-0.6.0a2/wonda/bot/polling/default.py
+-rw-r--r--   0        0        0      129 2023-08-01 13:12:06.364526 wonda-0.6.0a2/wonda/bot/rules/__init__.py
+-rw-r--r--   0        0        0     1816 2023-08-01 14:48:49.174835 wonda-0.6.0a2/wonda/bot/rules/abc.py
+-rw-r--r--   0        0        0     4437 2023-08-01 13:50:29.499615 wonda-0.6.0a2/wonda/bot/rules/base.py
+-rw-r--r--   0        0        0     5535 2023-08-03 14:29:37.741552 wonda-0.6.0a2/wonda/bot/rules/message.py
+-rw-r--r--   0        0        0      125 2023-08-01 13:12:06.365285 wonda-0.6.0a2/wonda/bot/states/__init__.py
+-rw-r--r--   0        0        0       78 2023-08-01 13:12:06.365455 wonda-0.6.0a2/wonda/bot/states/dispenser/__init__.py
+-rw-r--r--   0        0        0      822 2023-08-01 13:12:06.365624 wonda-0.6.0a2/wonda/bot/states/dispenser/abc.py
+-rw-r--r--   0        0        0      832 2023-08-01 13:12:06.365811 wonda-0.6.0a2/wonda/bot/states/dispenser/default.py
+-rw-r--r--   0        0        0      574 2023-08-01 13:12:06.365978 wonda-0.6.0a2/wonda/bot/states/types.py
+-rw-r--r--   0        0        0      636 2023-08-01 13:12:06.366161 wonda-0.6.0a2/wonda/bot/updates/__init__.py
+-rw-r--r--   0        0        0      149 2023-08-05 22:39:51.531540 wonda-0.6.0a2/wonda/bot/updates/base.py
+-rw-r--r--   0        0        0     5287 2023-08-01 13:12:50.665638 wonda-0.6.0a2/wonda/bot/updates/types.py
+-rw-r--r--   0        0        0        0 2022-12-09 12:31:48.203870 wonda-0.6.0a2/wonda/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:12:06.388351 wonda-0.6.0a2/wonda/contrib/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-09 12:31:48.204053 wonda-0.6.0a2/wonda/contrib/rules/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:17:57.296559 wonda-0.6.0a2/wonda/contrib/storage/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-01 13:12:06.388804 wonda-0.6.0a2/wonda/contrib/storage/redis.py
+-rw-r--r--   0        0        0      298 2023-08-01 13:12:06.366842 wonda-0.6.0a2/wonda/errors/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-01 13:12:06.367058 wonda-0.6.0a2/wonda/errors/base_exceptions.py
+-rw-r--r--   0        0        0     1635 2023-08-01 14:03:19.646417 wonda-0.6.0a2/wonda/errors/code_exception.py
+-rw-r--r--   0        0        0       73 2023-04-21 11:36:28.384533 wonda-0.6.0a2/wonda/errors/error_handler/__init__.py
+-rw-r--r--   0        0        0      704 2023-08-01 13:12:06.367251 wonda-0.6.0a2/wonda/errors/error_handler/abc.py
+-rw-r--r--   0        0        0     2031 2023-08-01 13:12:06.367470 wonda-0.6.0a2/wonda/errors/error_handler/error_handler.py
+-rw-r--r--   0        0        0      533 2023-08-01 14:27:57.256711 wonda-0.6.0a2/wonda/modules.py
+-rw-r--r--   0        0        0       76 2023-08-01 13:12:06.389026 wonda-0.6.0a2/wonda/net/__init__.py
+-rw-r--r--   0        0        0      877 2023-08-05 19:40:03.710995 wonda-0.6.0a2/wonda/net/abc.py
+-rw-r--r--   0        0        0     2283 2023-08-03 08:59:33.003113 wonda-0.6.0a2/wonda/net/default.py
+-rw-r--r--   0        0        0      123 2023-08-01 13:12:06.368301 wonda-0.6.0a2/wonda/tools/__init__.py
+-rw-r--r--   0        0        0      551 2023-08-01 13:12:06.368500 wonda-0.6.0a2/wonda/tools/delayed_task.py
+-rw-r--r--   0        0        0      284 2023-08-01 13:12:06.368688 wonda-0.6.0a2/wonda/tools/keyboard/__init__.py
+-rw-r--r--   0        0        0      730 2023-08-05 22:17:58.484731 wonda-0.6.0a2/wonda/tools/keyboard/abc.py
+-rw-r--r--   0        0        0     2864 2023-08-05 19:39:08.370714 wonda-0.6.0a2/wonda/tools/keyboard/builder.py
+-rw-r--r--   0        0        0     5281 2023-08-01 13:12:06.389685 wonda-0.6.0a2/wonda/tools/keyboard/elements.py
+-rw-r--r--   0        0        0     2603 2023-08-01 14:08:40.080104 wonda-0.6.0a2/wonda/tools/loop_wrapper.py
+-rw-r--r--   0        0        0      174 2023-08-01 13:12:06.369277 wonda-0.6.0a2/wonda/tools/storage/__init__.py
+-rw-r--r--   0        0        0      648 2023-08-01 13:12:06.369452 wonda-0.6.0a2/wonda/tools/storage/abc.py
+-rw-r--r--   0        0        0     1861 2023-08-01 13:12:06.369619 wonda-0.6.0a2/wonda/tools/storage/memory.py
+-rw-r--r--   0        0        0      132 2023-08-01 13:12:06.369784 wonda-0.6.0a2/wonda/tools/storage/types.py
+-rw-r--r--   0        0        0       73 2023-02-27 18:52:52.469528 wonda-0.6.0a2/wonda/tools/text/__init__.py
+-rw-r--r--   0        0        0       29 2023-02-27 18:52:54.495531 wonda-0.6.0a2/wonda/tools/text/formatting/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-27 18:52:47.941301 wonda-0.6.0a2/wonda/tools/text/formatting/html.py
+-rw-r--r--   0        0        0     2761 2023-02-27 18:52:50.221309 wonda-0.6.0a2/wonda/tools/text/formatting/markdown.py
+-rw-r--r--   0        0        0       93 2022-12-09 12:31:48.210068 wonda-0.6.0a2/wonda/tools/text/parse_mode.py
+-rw-r--r--   0        0        0       55 2023-02-01 05:24:13.893095 wonda-0.6.0a2/wonda/types/__init__.py
+-rw-r--r--   0        0        0     4438 2023-08-01 13:13:03.042503 wonda-0.6.0a2/wonda/types/enums.py
+-rw-r--r--   0        0        0      588 2023-08-05 19:34:57.249565 wonda-0.6.0a2/wonda/types/helper.py
+-rw-r--r--   0        0        0    78297 2023-08-05 19:55:33.676987 wonda-0.6.0a2/wonda/types/methods.py
+-rw-r--r--   0        0        0    59280 2023-08-05 19:56:33.820272 wonda-0.6.0a2/wonda/types/objects.py
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 wonda-0.6.0a2/PKG-INFO
```

### Comparing `wonda-0.6.0a1/LICENSE` & `wonda-0.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/README.md` & `wonda-0.6.0a2/README.md`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/pyproject.toml` & `wonda-0.6.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wonda"
-version = "0.6.0a1"
+version = "0.6.0a2"
 description = "Asynchronous feature-rich framework for building Telegram bots"
 authors = []
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/wondergram-org/wonda/"
 
 [tool.poetry.dependencies]
```

### Comparing `wonda-0.6.0a1/wonda/api/abc.py` & `wonda-0.6.0a2/wonda/api/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def file_url(self) -> str:
         """
         Link to the file storage
         """
         return self.API_URL + f"file/bot{self.token}/"
 
     @abstractmethod
-    async def request(self, method: str, params: dict = {}) -> bytes | None:
+    async def request(self, method: str, params: dict = {}) -> bytes:
         """
         Opens a request session and makes a single API call
         """
         pass
 
     async def request_many(
         self, requests: typing.Iterable[APIRequest]  # type: ignore
@@ -52,14 +52,14 @@
         Performs validation of the request data.
         If necessary, modifies and transforms it.
         """
         for v in self.request_validators:
             params = await v.validate(params)
         return params
 
-    async def validate_response(self, response: bytes) -> bytes | None:
+    async def validate_response(self, response: bytes) -> bytes:
         """
         Verifies and adapts the response.
         """
         for v in self.response_validators:
             response = await v.validate(response)
         return response
```

### Comparing `wonda-0.6.0a1/wonda/api/api.py` & `wonda-0.6.0a2/wonda/api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.token = token
         self.http_client = http_client or DefaultNetworkClient()
         self.request_validators: list[ABCRequestValidator] = DEFAULT_REQUEST_VALIDATORS
         self.response_validators: list[
             ABCResponseValidator
         ] = DEFAULT_RESPONSE_VALIDATORS
 
-    async def request(self, method: str, params: dict = {}) -> bytes | None:
+    async def request(self, method: str, params: dict = {}) -> bytes:
         await logger.debug("Calling", method=method, params=params)
 
         data = await self.validate_request(params or {})
         response = await self.http_client.request_bytes(
             self.api_url + method, data=data
         )
```

### Comparing `wonda-0.6.0a1/wonda/api/utils/file_util.py` & `wonda-0.6.0a2/wonda/api/utils/file_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 class File:
     def __init__(self, content: bytes, name: str | None = None) -> None:
         self.content, self.name = content, name
 
     @classmethod
-    def from_bytes(cls, source: bytes, name: str | None = None) -> InputFile:
-        return InputFile(name or f"{hash(source)}.bin", source)
+    def from_bytes(cls, source: bytes, name: str) -> InputFile:
+        return InputFile(name or f"unnamed.bin", source)
 
     @classmethod
     def from_path(cls, source: str | Path, name: str | None = None) -> InputFile:
         source = Path(source) if isinstance(source, str) else source
 
         with source.open("rb") as f:
             return InputFile(name or source.name, f.read())
```

### Comparing `wonda-0.6.0a1/wonda/api/utils/token_util.py` & `wonda-0.6.0a2/wonda/api/utils/token_util.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/api/validators/request.py` & `wonda-0.6.0a2/wonda/api/validators/request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,22 @@
-from typing import Any
-
-from aiohttp import FormData
-
-from wonda.api.utils.file_util import InputFile
 from wonda.api.validators.abc import ABCRequestValidator
-from wonda.types.helper import Model, json
-
+from wonda.api.utils.file_util import InputFile
+from wonda.types.helper import Model
 
-def translate(v: Any) -> Any:
-    if isinstance(v, Model):
-        return json.encode(v).decode()
-    elif isinstance(v, dict):
+def translate(v):
+    if isinstance(v, dict):
         return {n: translate(p) for n, p in v.items() if v is not None}
     elif isinstance(v, list):
         return [translate(i) for i in v]
-    elif isinstance(v, InputFile):
-        return (v.name, v.content)
-    elif v is None:
-        pass
+    elif isinstance(v, Model):
+        return v.json()
+    elif isinstance(v, int):
+        return str(v)
     return v
 
 
 class TranslateTypesValidator(ABCRequestValidator):
-    async def validate(self, request: dict) -> FormData:
-        return FormData({k: translate(v) for k, v in request.items() if v is not None})
+    async def validate(self, data: dict) -> dict:
+        return {k: translate(v) for k, v in data.items() if v is not None}
 
 
 __all__ = ("TranslateTypesValidator",)
```

### Comparing `wonda-0.6.0a1/wonda/api/validators/response.py` & `wonda-0.6.0a2/wonda/api/validators/response.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/__init__.py` & `wonda-0.6.0a2/wonda/bot/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from wonda.api.utils import File, Token
 
 from .abc import ABCFramework
 from .blueprint import ABCBlueprint, DefaultBlueprint
 from .bot import Bot
 from .dispatch import ABCHandler, ABCMiddleware, ABCRouter, ABCView, DefaultRouter
-from .polling import ABCPolling, BotPolling
+from .polling import ABCPoller, DefaultPoller
 from .rules import *
 from .states import (
     ABCStateDispenser,
     BaseStateGroup,
     DefaultStateDispenser,
     StateRepr,
     get_state_repr,
 )
 from .updates import *
 
 Blueprint = DefaultBlueprint
-Polling = BotPolling
+Polling = DefaultPoller
 Router = DefaultRouter
 StateDispenser = DefaultStateDispenser
```

### Comparing `wonda-0.6.0a1/wonda/bot/blueprint/abc.py` & `wonda-0.6.0a2/wonda/bot/blueprint/abc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from wonda.bot.abc import ABCFramework
 
 if TYPE_CHECKING:
     from wonda.api import ABCAPI
     from wonda.bot.dispatch.dispatcher import ABCDispatcher
     from wonda.bot.states import ABCStateDispenser
@@ -11,12 +11,12 @@
 
 class ABCBlueprint(ABCFramework):
     api: "ABCAPI"
     dispatcher: "ABCDispatcher"
     state_dispenser: "ABCStateDispenser"
 
     @abstractmethod
-    def load_into(self, framework: Any) -> "ABCBlueprint":
+    def load_into(self, framework: "ABCFramework") -> "ABCBlueprint":
         pass
 
     def run_forever(self) -> None:
         raise NotImplementedError("Running polling from blueprints is not implemented")
```

### Comparing `wonda-0.6.0a1/wonda/bot/blueprint/default.py` & `wonda-0.6.0a2/wonda/bot/blueprint/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/default.py` & `wonda-0.6.0a2/wonda/bot/dispatch/dispatcher/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/dispatch/handler/func.py` & `wonda-0.6.0a2/wonda/bot/dispatch/handler/func.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/dispatch/router/abc.py` & `wonda-0.6.0a2/wonda/bot/dispatch/router/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/dispatch/router/default.py` & `wonda-0.6.0a2/wonda/bot/dispatch/router/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/dispatch/view/abc.py` & `wonda-0.6.0a2/wonda/bot/dispatch/view/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/dispatch/view/impl.py` & `wonda-0.6.0a2/wonda/bot/dispatch/view/impl.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/polling/bot.py` & `wonda-0.6.0a2/wonda/bot/polling/default.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 from typing import AsyncIterator
 
-from wonda.api import ABCAPI
-from wonda.bot.polling.abc import ABCPolling
+from wonda.api.abc import ABCAPI
+from wonda.bot.polling.abc import ABCPoller
 from wonda.errors import ABCErrorHandler, ErrorHandler, TelegramAPIError
 from wonda.modules import logger
+from wonda.types.helper import json
 from wonda.types.objects import Update
 
 
-class BotPolling(ABCPolling):
+class DefaultPoller(ABCPoller):
     def __init__(
-        self,
-        api: ABCAPI | None = None,
-        error_handler: ABCErrorHandler | None = None,
-    ):
+        self, api: ABCAPI, error_handler: ABCErrorHandler | None = None
+    ) -> None:
         self.api = api
         self.error_handler = error_handler or ErrorHandler()
 
-        self.stop = False
-        self.offset = 0
+        self.offset: int = 0
+        self.allowed_updates: list[str] = []
 
-    async def get_updates(self) -> list["Update"]:
-        updates = []
+        self.stop = False
 
+    async def get_updates(self) -> list[Update]:
         try:
-            updates = await self.api.get_updates(offset=self.offset)
+            updates = await self.api.request(
+                "getUpdates",
+                {"offset": self.offset, "allowed_updates": self.allowed_updates},
+            )
         except TelegramAPIError[401, 404] as e:
             await logger.critical(e)
             self.stop = True
 
-        return updates
+        return json.decode(updates, type=list[Update])
+
+    async def listen(self) -> AsyncIterator[Update]:
+        await logger.debug(
+            "Polling", offset=self.offset, allowed_updates=self.allowed_updates
+        )
 
-    async def listen(self) -> AsyncIterator["Update"]:
         while not self.stop:
             try:
                 updates = await self.get_updates()
                 for update in updates:
                     self.offset = update.update_id + 1
                     yield update
             except BaseException as e:
-                await self.error_handler.handle(e)
+                await self.error_handler.handle(e)
```

### Comparing `wonda-0.6.0a1/wonda/bot/rules/abc.py` & `wonda-0.6.0a2/wonda/bot/rules/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/rules/base.py` & `wonda-0.6.0a2/wonda/bot/rules/base.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/rules/message.py` & `wonda-0.6.0a2/wonda/bot/rules/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Command(ABCRule[Message]):
     """
     A rule that handles bot commands. It takes in a list of
     valid command texts and checks if the message
     contains one of those commands.
     """
 
-    me: "User | None" = None
+    me: User | None = None
 
     def __init__(self, texts: str | list[str], prefixes: str | list[str] = "/") -> None:
         self.texts = texts if isinstance(texts, list) else [texts]
         self.prefixes = prefixes if isinstance(prefixes, list) else [prefixes]
 
     async def check(self, m: Message, ctx: dict) -> bool:
         if text := m.text or m.caption:
```

### Comparing `wonda-0.6.0a1/wonda/bot/states/dispenser/abc.py` & `wonda-0.6.0a2/wonda/bot/states/dispenser/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/states/dispenser/default.py` & `wonda-0.6.0a2/wonda/bot/states/dispenser/default.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/states/types.py` & `wonda-0.6.0a2/wonda/bot/states/types.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/updates/__init__.py` & `wonda-0.6.0a2/wonda/bot/updates/__init__.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/bot/updates/types.py` & `wonda-0.6.0a2/wonda/bot/updates/types.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/contrib/storage/redis.py` & `wonda-0.6.0a2/wonda/contrib/storage/redis.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/errors/code_exception.py` & `wonda-0.6.0a2/wonda/errors/code_exception.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/errors/error_handler/abc.py` & `wonda-0.6.0a2/wonda/errors/error_handler/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/errors/error_handler/error_handler.py` & `wonda-0.6.0a2/wonda/errors/error_handler/error_handler.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/modules.py` & `wonda-0.6.0a2/wonda/modules.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/net/abc.py` & `wonda-0.6.0a2/wonda/net/abc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from abc import ABC, abstractmethod
 from typing import Any
 
+_ = Any
+
 
 class ABCNetworkClient(ABC):
     @abstractmethod
+    def construct_form(self, data: dict) -> _:
+        pass
+
+    @abstractmethod
     async def request_text(
-        self, url: str, method: str = "get", data: dict | None = None, **kwargs
+        self, url: str, method: str = "get", data: dict | None = None, **kw
     ) -> str:
         pass
 
     @abstractmethod
     async def request_json(
-        self, url: str, method: str = "get", data: dict | None = None, **kwargs
+        self, url: str, method: str = "get", data: dict | None = None, **kw
     ) -> dict:
         pass
 
     @abstractmethod
     async def request_bytes(
-        self, url: str, method: str = "get", data: dict | None = None, **kwargs
+        self, url: str, method: str = "get", data: dict | None = None, **kw
     ) -> bytes:
         pass
 
     @abstractmethod
     async def close(self) -> None:
         pass
```

### Comparing `wonda-0.6.0a1/wonda/net/default.py` & `wonda-0.6.0a2/wonda/net/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 import ssl
 
 import certifi
-from aiohttp import ClientResponse, ClientSession, ClientTimeout, FormData, TCPConnector
+from aiohttp import ClientSession, ClientTimeout, FormData, TCPConnector
 
 from wonda.modules import JSONModule, json
 from wonda.net.abc import ABCNetworkClient
 
-Data = dict | FormData
-
 
 class DefaultNetworkClient(ABCNetworkClient):
     def __init__(
         self,
         session: ClientSession | None = None,
         json_processing_module: JSONModule | None = None,
         timeout: ClientTimeout | None = None,
     ) -> None:
         self.json_processing_module = json_processing_module or json
         self.session = session or ClientSession(
-            timeout=ClientTimeout(0),
+            timeout=timeout or ClientTimeout(0),
             connector=TCPConnector(
                 ssl=ssl.create_default_context(cafile=certifi.where())
             ),
             json_serialize=self.json_processing_module.dumps,
         )
 
     async def request_bytes(
-        self, url: str, method: str = "get", data: Data | None = None, **kw
+        self, url: str, method: str = "get", data: dict | None = None, **kw
     ) -> bytes:
         async with self.session.request(
             url=url, method=method, data=data, **kw
         ) as response:
             return await response.content.read()
 
     async def request_json(
-        self, url: str, method: str = "get", data: Data | None = None, **kw
+        self, url: str, method: str = "get", data: dict | None = None, **kw
     ) -> dict:
         response = await self.request_bytes(url, method, data, **kw)
         return self.json_processing_module.loads(response)
 
     async def request_text(
-        self, url: str, method: str = "get", data: Data | None = None, **kw
+        self, url: str, method: str = "get", data: dict | None = None, **kw
     ) -> str:
         response = await self.request_bytes(url, method, data, **kw)
         return response.decode()
 
     async def close(self) -> None:
         if self.session and not self.session.closed:
             await self.session.close()
 
+    def construct_form(cls, data: dict) -> FormData:
+        form = FormData(quote_fields=False)
+        for k, v in data.items():
+            params = {}
+            if isinstance(v, tuple):
+                params["filename"], v = v[0], v[1]
+            else:
+                v = str(v)
+            form.add_field(k, v, **params)
+        return form
+
     def __del__(self):
         if self.session and not self.session.closed:
             if self.session._connector is not None and self.session._connector_owner:
                 self.session._connector.close()
             self.session._connector = None
```

### Comparing `wonda-0.6.0a1/wonda/tools/delayed_task.py` & `wonda-0.6.0a2/wonda/tools/delayed_task.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/tools/keyboard/abc.py` & `wonda-0.6.0a2/wonda/tools/keyboard/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from abc import ABC, abstractmethod
-from typing import Any, Self
+from typing import Any
 
 
 class ABCKeyboardBuilder(ABC):
     """
     A keyboard builder interface.
     """
 
     @abstractmethod
-    def add(self, button: "ABCButton") -> Self:
+    def add(self, button: "ABCButton") -> "ABCKeyboardBuilder":
         """
         Adds a button to the keyboard.
         """
         pass
 
     @abstractmethod
-    def row(self) -> Self:
+    def row(self) -> "ABCKeyboardBuilder":
         """
         Adds a row to the keyboard. Panics if the last row was empty.
         """
         pass
 
     @abstractmethod
     def build(self) -> Any:
```

### Comparing `wonda-0.6.0a1/wonda/tools/keyboard/builder.py` & `wonda-0.6.0a2/wonda/tools/keyboard/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from typing import Any, Generic, TypeVar
+from typing import Any
 
 from wonda.tools.keyboard.abc import ABCButton, ABCKeyboardBuilder
 from wonda.types.objects import (
     InlineKeyboardButton,
     InlineKeyboardMarkup,
     KeyboardButton,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 _ = Any
-T = TypeVar("T")
 
 
-class BaseKeyboardBuilder(ABCKeyboardBuilder, Generic[T]):
+class BaseKeyboardBuilder(ABCKeyboardBuilder):
     """
     A basic keyboard builder which implements independent logic for
     `.add()` and `.row()` methods
     """
 
+    button_type: _
+
     def __init__(self) -> None:
         self.rows: list[list[ABCButton]] = [[]]
 
     @property
-    def keyboard(self) -> list[list[Any]]:
+    def keyboard(self) -> list[list[_]]:
         """
         Keyboard markup to be sent.
         """
-        type = self.__orig_bases__[0].__args__[0]  # type: ignore
-        return [[type(**button.dict()) for button in row] for row in self.rows]
+        return [
+            [self.button_type(**button.dict()) for button in row] for row in self.rows
+        ]
 
     @property
     def last_row(self) -> list[ABCButton]:
         """
         Convenience property to get the last button row.
         """
         return self.rows[-1]
@@ -51,29 +53,33 @@
         self.rows.append([])
         return self
 
     def build(self) -> ReplyKeyboardMarkup | InlineKeyboardMarkup:
         raise NotImplementedError("`.build()` method implemenation is builder specific")
 
 
-class InlineKeyboardBuilder(BaseKeyboardBuilder[InlineKeyboardButton]):
+class InlineKeyboardBuilder(BaseKeyboardBuilder):
     """
     A builder for an inline keyboard. No options are available
     for this type of keyboard.
     """
 
+    button_type = InlineKeyboardButton
+
     def build(self) -> InlineKeyboardMarkup:
         return InlineKeyboardMarkup(self.keyboard)
 
 
-class ReplyKeyboardBuilder(BaseKeyboardBuilder[KeyboardButton]):
+class ReplyKeyboardBuilder(BaseKeyboardBuilder):
     """
     A builder for a keyboard with custom reply options.
     """
 
+    button_type = KeyboardButton
+
     def __init__(
         self,
         is_persistent: bool = False,
         resize_keyboard: bool = False,
         one_time_keyboard: bool = False,
         selective: bool = False,
     ) -> None:
```

### Comparing `wonda-0.6.0a1/wonda/tools/keyboard/elements.py` & `wonda-0.6.0a2/wonda/tools/keyboard/elements.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/tools/loop_wrapper.py` & `wonda-0.6.0a2/wonda/tools/loop_wrapper.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/tools/storage/abc.py` & `wonda-0.6.0a2/wonda/tools/storage/abc.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/tools/storage/memory.py` & `wonda-0.6.0a2/wonda/tools/storage/memory.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/tools/text/formatting/html.py` & `wonda-0.6.0a2/wonda/tools/text/formatting/html.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/tools/text/formatting/markdown.py` & `wonda-0.6.0a2/wonda/tools/text/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/types/enums.py` & `wonda-0.6.0a2/wonda/types/enums.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/types/methods.py` & `wonda-0.6.0a2/wonda/types/methods.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/wonda/types/objects.py` & `wonda-0.6.0a2/wonda/types/objects.py`

 * *Files identical despite different names*

### Comparing `wonda-0.6.0a1/PKG-INFO` & `wonda-0.6.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wonda
-Version: 0.6.0a1
+Version: 0.6.0a2
 Summary: Asynchronous feature-rich framework for building Telegram bots
 Home-page: https://github.com/wondergram-org/wonda/
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

