# Comparing `tmp/heizer-999999.dev1681441540.tar.gz` & `tmp/heizer-999999.dev1690413391.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heizer-999999.dev1681441540.tar", last modified: Fri Apr 14 03:05:48 2023, max compression
+gzip compressed data, was "heizer-999999.dev1690413391.tar", last modified: Wed Jul 26 23:16:39 2023, max compression
```

## Comparing `heizer-999999.dev1681441540.tar` & `heizer-999999.dev1690413391.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.053672 heizer-999999.dev1681441540/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.053672 heizer-999999.dev1681441540/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/.github/workflows/deploy-latest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.053672 heizer-999999.dev1681441540/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/img1.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.057672 heizer-999999.dev1681441540/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.057672 heizer-999999.dev1681441540/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.057672 heizer-999999.dev1681441540/docs/source/_static/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/_static/websocket/create-topic.png
--rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/_static/websocket/message-in-browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/_static/websocket/publish-kafka-msg.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.057672 heizer-999999.dev1681441540/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/heizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.057672 heizer-999999.dev1681441540/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/tutorial/consumer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/tutorial/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/docs/source/tutorial/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/heizer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 03:05:40.000000 heizer-999999.dev1681441540/heizer/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/heizer/_source/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/_source/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/_source/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/_source/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/_source/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/_source/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/heizer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/heizer/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/heizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-14 03:05:48.000000 heizer-999999.dev1681441540/heizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-14 03:05:48.000000 heizer-999999.dev1681441540/heizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:05:48.000000 heizer-999999.dev1681441540/heizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 03:05:48.000000 heizer-999999.dev1681441540/heizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 03:05:48.000000 heizer-999999.dev1681441540/heizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/samples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/samples/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/samples/websockets/client.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/samples/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:48.061672 heizer-999999.dev1681441540/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-14 03:05:36.000000 heizer-999999.dev1681441540/tests/test_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.478335 heizer-999999.dev1690413391/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.478335 heizer-999999.dev1690413391/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/.github/workflows/deploy-latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/img1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/docs/source/_static/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/_static/websocket/create-topic.png
+-rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/_static/websocket/message-in-browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/_static/websocket/publish-kafka-msg.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/heizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/tutorial/consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/tutorial/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/docs/source/tutorial/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.482335 heizer-999999.dev1690413391/heizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 23:16:31.000000 heizer-999999.dev1690413391/heizer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/heizer/_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/_source/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/_source/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/_source/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/_source/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/_source/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/heizer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/heizer/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/heizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-26 23:16:39.000000 heizer-999999.dev1690413391/heizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-26 23:16:39.000000 heizer-999999.dev1690413391/heizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:16:39.000000 heizer-999999.dev1690413391/heizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-26 23:16:39.000000 heizer-999999.dev1690413391/heizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 23:16:39.000000 heizer-999999.dev1690413391/heizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/samples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/samples/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/samples/websockets/client.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/samples/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:39.486335 heizer-999999.dev1690413391/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-26 23:16:27.000000 heizer-999999.dev1690413391/tests/test_consumer.py
```

### Comparing `heizer-999999.dev1681441540/.github/workflows/deploy-latest.yml` & `heizer-999999.dev1690413391/.github/workflows/deploy-latest.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/.github/workflows/main.yml` & `heizer-999999.dev1690413391/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/.github/workflows/release.yml` & `heizer-999999.dev1690413391/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/.gitignore` & `heizer-999999.dev1690413391/.gitignore`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/.pre-commit-config.yaml` & `heizer-999999.dev1690413391/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/LICENSE` & `heizer-999999.dev1690413391/LICENSE`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/PKG-INFO` & `heizer-999999.dev1690413391/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681441540
+Version: 999999.dev1690413391
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `heizer-999999.dev1681441540/README.md` & `heizer-999999.dev1690413391/README.md`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docker-compose.yaml` & `heizer-999999.dev1690413391/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/Makefile` & `heizer-999999.dev1690413391/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/img1.png` & `heizer-999999.dev1690413391/docs/img1.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/make.bat` & `heizer-999999.dev1690413391/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/_static/websocket/create-topic.png` & `heizer-999999.dev1690413391/docs/source/_static/websocket/create-topic.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/_static/websocket/message-in-browser.png` & `heizer-999999.dev1690413391/docs/source/_static/websocket/message-in-browser.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/_static/websocket/publish-kafka-msg.png` & `heizer-999999.dev1690413391/docs/source/_static/websocket/publish-kafka-msg.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/_templates/versions.html` & `heizer-999999.dev1690413391/docs/source/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/conf.py` & `heizer-999999.dev1690413391/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/tutorial/consumer.rst` & `heizer-999999.dev1690413391/docs/source/tutorial/consumer.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/tutorial/prepare.rst` & `heizer-999999.dev1690413391/docs/source/tutorial/prepare.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/docs/source/tutorial/websockets.rst` & `heizer-999999.dev1690413391/docs/source/tutorial/websockets.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/heizer/_source/__init__.py` & `heizer-999999.dev1690413391/heizer/_source/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import sys
 
-FORMAT = "%(asctime)s %(levelname)-8s %(message)s"
+FORMAT = "heizer %(asctime)s %(levelname)-8s %(message)s"
 
 
 def get_logger(name: str) -> logging.Logger:
     formatter = logging.Formatter(fmt=FORMAT, datefmt="%Y-%m-%d %H:%M:%S")
     handler = logging.FileHandler("/tmp/heizer_log.txt", mode="w")
     handler.setFormatter(formatter)
     screen_handler = logging.StreamHandler(stream=sys.stdout)
```

### Comparing `heizer-999999.dev1681441540/heizer/_source/admin.py` & `heizer-999999.dev1690413391/heizer/_source/admin.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/heizer/_source/consumer.py` & `heizer-999999.dev1690413391/heizer/_source/consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import functools
 import logging
+import signal
 from uuid import uuid4
 
 from confluent_kafka import Consumer
 from pydantic import BaseModel
 
 from heizer._source import get_logger
 from heizer._source.admin import create_new_topic, get_admin_client
@@ -30,14 +31,24 @@
 F = TypeVar("F", bound=Callable[..., Any])
 P = ParamSpec("P")
 T = TypeVar("T")
 
 logger = get_logger(__name__)
 
 
+def signal_handler(signal: Any, frame: Any) -> None:
+    global interrupted
+    interrupted = True
+
+
+signal.signal(signal.SIGINT, signal_handler)
+
+interrupted = False
+
+
 class consumer(object):
     """A decorator to create a consumer"""
 
     __id__: str
     name: Optional[str]
 
     topics: List[HeizerTopic]
@@ -45,126 +56,132 @@
     call_once: bool = False
     stopper: Optional[Stopper] = None
     deserializer: Optional[Type[BaseModel]] = None
 
     is_async: bool = False
     poll_timeout: int = 1
 
-    init_topics: bool = True
+    init_topics: bool = False
 
     def __init__(
         self,
         *,
         topics: List[HeizerTopic],
         config: HeizerConfig = HeizerConfig(),
         call_once: bool = False,
         stopper: Optional[Stopper] = None,
         deserializer: Optional[Type[BaseModel]] = None,
         is_async: bool = False,
         name: Optional[str] = None,
         poll_timeout: Optional[int] = None,
-        init_topics: bool = True,
+        init_topics: bool = False,
     ):
         self.topics = topics
         self.config = config
         self.call_once = call_once
         self.stopper = stopper
         self.deserializer = deserializer
         self.__id__ = str(uuid4())
         self.name = name or self.__id__
         self.is_async = is_async
-        self.poll_timeout = poll_timeout or 1
+        self.poll_timeout = poll_timeout if poll_timeout is not None else 1
         self.init_topics = init_topics
 
-    async def __run__(
+    def __repr__(self) -> str:
+        return self.name or self.__id__
+
+    async def __run__(  # type: ignore
         self,
         func: Callable[Concatenate[HeizerMessage, P], Union[T, Awaitable[T]]],
-        c: Consumer,
         is_async: bool,
         *args: P.args,
         **kwargs: P.kwargs,
-    ) -> Union[Optional[T]]:  # ignore type
+    ) -> Union[Optional[T]]:
         """Run the consumer"""
 
+        logger.debug(f"[{self}] Creating consumer ")
+        c = Consumer(self.config.value)
+
+        logger.debug(f"[{self}] Subscribing to topics {[topic.name for topic in self.topics]}")
+        c.subscribe([topic.name for topic in self.topics])
+
         if self.init_topics:
-            logger.debug("Initializing topics")
+            logger.debug(f"[{self}] Initializing topics")
             admin_client = get_admin_client(self.config)
             create_new_topic(admin_client, self.topics)
 
         while True:
+            if interrupted:
+                logger.debug(f"[{self}] Interrupted by keyboard")
+                break
+
             msg = c.poll(self.poll_timeout)
 
             if msg is None:
                 continue
 
             if msg.error():
-                logger.error(f"Consumer error: {msg.error()}")
+                logger.error(f"[{self}] Consumer error: {msg.error()}")
                 continue
 
-            logger.debug("Received message")
+            logger.debug(f"[{self}] Received message")
             hmessage = HeizerMessage(msg)
 
             if self.deserializer is not None:
-                logger.debug("Parsing message")
+                logger.debug(f"[{self}] Parsing message")
                 try:
                     hmessage.formatted_value = self.deserializer.parse_raw(hmessage.value)
                 except Exception as e:
-                    logger.exception("Failed to deserialize message", exc_info=e)
+                    logger.exception(f"[{self}] Failed to deserialize message", exc_info=e)
 
             result = None
 
-            logger.debug("Executing function")
+            logger.debug(f"[{self}] Executing function {func.__name__}")
             try:
                 if is_async:
                     result = await func(hmessage, *args, **kwargs)  # type: ignore
                 else:
                     result = func(hmessage, *args, **kwargs)
             except Exception as e:
                 logger.exception(
-                    f"Failed to execute function {func.__name__}",
+                    f"[{self}] Failed to execute function {func.__name__}",
                     exc_info=e,
                 )
             finally:
                 # TODO: add failed message to a retry queue
-                logger.debug("Committing message")
+                logger.debug(f"[{self}] Committing message")
                 c.commit()
 
             if self.stopper is not None:
-                logger.debug("Executing stopper function")
+                logger.debug(f"[{self}] Executing stopper function")
                 try:
                     should_stop = self.stopper(hmessage)
                 except Exception as e:
                     logger.warning(
-                        f"Failed to execute stopper function {self.stopper.__name__}.",
+                        f"[{self}] Failed to execute stopper function {self.stopper.__name__}.",
                         exc_info=e,
                     )
                     should_stop = False
 
                 if should_stop:
                     return result
 
             if self.call_once is True:
-                logger.debug("Call Once is on, returning result")
+                logger.debug(f"[{self}] Call Once is on, returning result")
                 return result
 
     def __call__(
         self, func: Callable[Concatenate[HeizerMessage, P], T]
     ) -> Callable[P, Union[Coroutine[Any, Any, Optional[T]], T, None]]:
-        logger.debug("Creating consumer")
-        c = Consumer(self.config.value)
-
-        logger.debug("Subscribing to topics")
-        c.subscribe([topic.name for topic in self.topics])
-
         @functools.wraps(func)
         async def async_decorator(*args: P.args, **kwargs: P.kwargs) -> Optional[T]:
             """Async decorator"""
-            logging.debug("Running async decorator")
-            return await self.__run__(func, c, self.is_async, *args, **kwargs)
+            logging.debug(f"[{self}] Running async decorator")
+            return await self.__run__(func, self.is_async, *args, **kwargs)
 
         @functools.wraps(func)
         def decorator(*args: P.args, **kwargs: P.kwargs) -> Optional[T]:
             """Sync decorator"""
-            logging.debug("Running sync decorator")
-            return asyncio.get_event_loop().run_until_complete(self.__run__(func, c, self.is_async, *args, **kwargs))
+            logging.debug(f"[{self}] Running sync decorator")
+            return asyncio.run(self.__run__(func, self.is_async, *args, **kwargs))
 
         return async_decorator if self.is_async else decorator
```

### Comparing `heizer-999999.dev1681441540/heizer/_source/message.py` & `heizer-999999.dev1690413391/heizer/_source/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 from confluent_kafka import Message
 
 from heizer.types import Any, Dict, List, Optional, Tuple, Union
 
 
 class HeizerMessage:
+    """
+    :class: HeizerMessage
+
+    A utility class for parsing Kafka messages using the confluent_kafka library.
+
+    Properties:
+        - `message`: A `confluent_kafka.Message` object representing the Kafka message.
+        - `topic`: Optional[str] - The topic of the Kafka message.
+        - `partition`: int - The partition of the Kafka message.
+        - `headers`: Optional[Dict[str, str]] - The headers of the Kafka message.
+        - `key`: Optional[str] - The key of the Kafka message.
+        - `value`: Optional[str] - The value of the Kafka message.
+        - `formatted_value`: Optional[Any] - A formatted version of the value.
+    """
+
     # initialized properties
     message: Message
     topic: Optional[str]
     partition: int
     headers: Optional[Dict[str, str]]
     key: Optional[str]
     value: Optional[str]
```

### Comparing `heizer-999999.dev1681441540/heizer/_source/producer.py` & `heizer-999999.dev1690413391/heizer/_source/producer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 import json
 from uuid import uuid4
 
 from confluent_kafka import Message, Producer
 
 from heizer._source import get_logger
-from heizer._source.admin import create_new_topic, get_admin_client
 from heizer._source.topic import HeizerTopic
 from heizer.config import HeizerConfig
 from heizer.types import Any, Callable, Dict, List, Optional, TypeVar, Union, cast
 
 logger = get_logger(__name__)
 
 R = TypeVar("R")
@@ -51,16 +50,14 @@
 
     default_key: Optional[str] = None
     default_headers: Optional[Dict[str, str]] = None
 
     key_alias: str = "key"
     headers_alias: str = "headers"
 
-    init_topics: bool = True
-
     # private properties
     _producer_instance: Optional[Producer] = None
 
     def __init__(
         self,
         topics: List[HeizerTopic],
         config: HeizerConfig = HeizerConfig(),
@@ -83,30 +80,24 @@
         if key_alias:
             self.key_alias = key_alias
         if headers_alias:
             self.headers_alias = headers_alias
 
         self.__id__ = str(uuid4())
         self.name = name or self.__id__
-        self.init_topics = init_topics
 
     @property
     def _producer(self) -> Producer:
         if not self._producer_instance:
             self._producer_instance = Producer(self.config.value)
         return self._producer_instance
 
     def __call__(self, func: F) -> F:
         @functools.wraps(func)
         def decorator(*args: Any, **kwargs: Any) -> Any:
-            if self.init_topics:
-                logger.debug("Initializing topics")
-                admin_client = get_admin_client(self.config)
-                create_new_topic(admin_client, self.topics)
-
             try:
                 result = func(*args, **kwargs)
             except Exception as e:
                 raise e
 
             try:
                 key = result.pop(self.key_alias, self.default_key)
```

### Comparing `heizer-999999.dev1681441540/heizer/_source/topic.py` & `heizer-999999.dev1690413391/heizer/_source/topic.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/heizer/config.py` & `heizer-999999.dev1690413391/heizer/config.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/heizer/types.py` & `heizer-999999.dev1690413391/heizer/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Awaitable, Callable, Coroutine, Dict, List, Optional, Tuple, Type, TypeVar, Union, cast
 
 if sys.version_info.minor <= 10:
     from typing_extensions import Concatenate, ParamSpec
 else:
     from typing import Concatenate, ParamSpec
 
-KafkaConfig = Dict[str, str]
+KafkaConfig = Dict[str, Any]
 Stopper = Callable[..., bool]
 
 
 __all__ = [
     "Any",
     "Awaitable",
     "Callable",
```

### Comparing `heizer-999999.dev1681441540/heizer.egg-info/PKG-INFO` & `heizer-999999.dev1690413391/heizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1681441540
+Version: 999999.dev1690413391
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `heizer-999999.dev1681441540/heizer.egg-info/SOURCES.txt` & `heizer-999999.dev1690413391/heizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/pyproject.toml` & `heizer-999999.dev1690413391/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries"
 ]
 
 dependencies = [
-    "confluent_kafka>=2.0.2,<2.1.0",
+    "confluent_kafka",
     "pydantic",
     "typing; python_version<'3.10'",
     "typing_extensions; python_version<'3.10'",
 ]
 
 [project.optional-dependencies]
 all = ["websockets"]
```

### Comparing `heizer-999999.dev1681441540/samples/websockets/client.html` & `heizer-999999.dev1690413391/samples/websockets/client.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/samples/websockets/server.py` & `heizer-999999.dev1690413391/samples/websockets/server.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1681441540/tests/test_consumer.py` & `heizer-999999.dev1690413391/tests/test_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 from typing import Any, Dict, cast
 
 import pytest
 from pydantic import BaseModel
 
-from heizer import HeizerConfig, HeizerMessage, HeizerTopic, consumer, producer
+from heizer import HeizerConfig, HeizerMessage, HeizerTopic, consumer, create_new_topic, get_admin_client, producer
 
 Producer_Config = HeizerConfig(
     {
         "bootstrap.servers": os.environ.get("KAFKA_SERVER", "localhost:9092"),
     }
 )
 
@@ -29,16 +29,20 @@
             "auto.offset.reset": "earliest",
         }
     )
 
 
 @pytest.mark.parametrize("group_id", ["test_consumer_stopper"])
 def test_consumer_stopper(group_id, consumer_config) -> None:
+    toppics = [HeizerTopic(name="heizer.test.result", partitions=[0, 1, 2], replication_factor=2)]
+    admin = get_admin_client(consumer_config)
+    create_new_topic(admin, toppics)
+
     @producer(
-        topics=[HeizerTopic(name="heizer.test.result", partitions=[0, 1, 2], replication_factor=2)],
+        topics=toppics,
         config=Producer_Config,
         key_alias="myKey",
         headers_alias="myHeaders",
     )
     def produce_data(status: str, result_value: str) -> Dict[str, Any]:
         return {
             "key1": 1,
```

