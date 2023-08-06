# Comparing `tmp/red_team_language-0.1.1.tar.gz` & `tmp/red_team_language-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_team_language-0.1.1.tar", last modified: Tue Sep 27 01:21:30 2022, max compression
+gzip compressed data, was "red_team_language-0.2.0.tar", last modified: Sun Aug  6 15:12:48 2023, max compression
```

## Comparing `red_team_language-0.1.1.tar` & `red_team_language-0.2.0.tar`

### file list

```diff
@@ -1,69 +1,788 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.677214 red_team_language-0.1.1/
--rw-rw-r--   0 user      (1000) user      (1000)    35149 2022-07-27 00:04:51.000000 red_team_language-0.1.1/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       61 2022-09-27 01:09:48.000000 red_team_language-0.1.1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2910 2022-09-27 01:21:30.678214 red_team_language-0.1.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1329 2022-09-02 02:39:04.000000 red_team_language-0.1.1/README.md
--rw-r--r--   0 user      (1000) user      (1000)       77 2022-07-26 23:56:06.000000 red_team_language-0.1.1/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.669215 red_team_language-0.1.1/red_team_language.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2910 2022-09-27 01:21:30.000000 red_team_language-0.1.1/red_team_language.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1683 2022-09-27 01:21:30.000000 red_team_language-0.1.1/red_team_language.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-27 01:21:30.000000 red_team_language-0.1.1/red_team_language.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       37 2022-09-27 01:21:30.000000 red_team_language-0.1.1/red_team_language.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       13 2022-09-27 01:21:30.000000 red_team_language-0.1.1/red_team_language.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2022-09-27 01:21:30.000000 red_team_language-0.1.1/red_team_language.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-27 01:14:06.000000 red_team_language-0.1.1/red_team_language.egg-info/zip-safe
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.670215 red_team_language-0.1.1/rtl/
--rw-rw-r--   0 user      (1000) user      (1000)      778 2022-09-27 01:10:32.000000 red_team_language-0.1.1/rtl/Dockerfile
--rw-r--r--   0 user      (1000) user      (1000)       22 2022-09-27 01:21:19.000000 red_team_language-0.1.1/rtl/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.670215 red_team_language-0.1.1/rtl/examples/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-09-27 01:04:50.000000 red_team_language-0.1.1/rtl/examples/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.672215 red_team_language-0.1.1/rtl/examples/shell/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-09-27 01:04:57.000000 red_team_language-0.1.1/rtl/examples/shell/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      585 2022-08-30 00:59:43.000000 red_team_language-0.1.1/rtl/examples/shell/executable_binary.rtl
--rw-r--r--   0 user      (1000) user      (1000)      130 2022-08-30 01:28:24.000000 red_team_language-0.1.1/rtl/examples/shell/executable_binary_inline.rtl
--rw-r--r--   0 user      (1000) user      (1000)      102 2022-08-30 00:55:01.000000 red_team_language-0.1.1/rtl/examples/shell/executable_script.rtl
--rw-r--r--   0 user      (1000) user      (1000)       98 2022-08-30 01:32:02.000000 red_team_language-0.1.1/rtl/examples/shell/executable_script_inline.rtl
--rw-r--r--   0 user      (1000) user      (1000)      189 2022-08-30 01:30:42.000000 red_team_language-0.1.1/rtl/examples/shell/executable_script_inline_obfuscated.rtl
--rw-rw-r--   0 user      (1000) user      (1000)      239 2022-09-20 00:21:08.000000 red_team_language-0.1.1/rtl/examples/shell/executable_script_obfuscated.rtl
--rw-r--r--   0 user      (1000) user      (1000)      197 2022-08-30 00:57:48.000000 red_team_language-0.1.1/rtl/examples/shell/executable_script_path.rtl
--rw-rw-r--   0 user      (1000) user      (1000)       39 2022-08-05 00:33:18.000000 red_team_language-0.1.1/rtl/examples/shell/failure_unknown_script.rtl
--rw-rw-r--   0 user      (1000) user      (1000)      360 2022-09-20 00:22:22.000000 red_team_language-0.1.1/rtl/examples/shell/openssl_reverse_shell.rtl
--rw-r--r--   0 user      (1000) user      (1000)      137 2022-08-30 01:36:34.000000 red_team_language-0.1.1/rtl/examples/shell/shell_double_executable.rtl
--rw-r--r--   0 user      (1000) user      (1000)       76 2022-08-30 01:36:42.000000 red_team_language-0.1.1/rtl/examples/shell/shell_executable.rtl
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.672215 red_team_language-0.1.1/rtl/lib/
--rw-r--r--   0 user      (1000) user      (1000)      271 2022-09-02 01:08:10.000000 red_team_language-0.1.1/rtl/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.672215 red_team_language-0.1.1/rtl/lib/protocol/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-07-31 18:01:53.000000 red_team_language-0.1.1/rtl/lib/protocol/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.674214 red_team_language-0.1.1/rtl/lib/protocol/shell/
--rw-r--r--   0 user      (1000) user      (1000)      624 2022-09-02 01:06:06.000000 red_team_language-0.1.1/rtl/lib/protocol/shell/Makefile
--rw-r--r--   0 user      (1000) user      (1000)      546 2022-09-02 01:07:00.000000 red_team_language-0.1.1/rtl/lib/protocol/shell/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)   900350 2022-08-30 02:05:51.000000 red_team_language-0.1.1/rtl/lib/protocol/shell/main.c
--rw-rw-r--   0 user      (1000) user      (1000)     2578 2022-08-30 02:05:52.000000 red_team_language-0.1.1/rtl/lib/protocol/shell/shell.c
--rw-rw-r--   0 user      (1000) user      (1000)      359 2022-08-30 02:05:52.000000 red_team_language-0.1.1/rtl/lib/protocol/shell/shell.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.674214 red_team_language-0.1.1/rtl/lib/transform/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-07-31 17:30:20.000000 red_team_language-0.1.1/rtl/lib/transform/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.675214 red_team_language-0.1.1/rtl/lib/transform/xor/
--rw-r--r--   0 user      (1000) user      (1000)      598 2022-09-02 01:19:37.000000 red_team_language-0.1.1/rtl/lib/transform/xor/Makefile
--rw-r--r--   0 user      (1000) user      (1000)      463 2022-09-02 01:42:37.000000 red_team_language-0.1.1/rtl/lib/transform/xor/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1297 2022-08-06 20:18:52.000000 red_team_language-0.1.1/rtl/lib/transform/xor/main.c
--rw-r--r--   0 user      (1000) user      (1000)     1256 2022-08-06 20:23:03.000000 red_team_language-0.1.1/rtl/lib/transform/xor/xor.c
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.676214 red_team_language-0.1.1/rtl/parser/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-07-27 00:41:09.000000 red_team_language-0.1.1/rtl/parser/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      375 2022-09-02 01:20:35.000000 red_team_language-0.1.1/rtl/parser/_with.py
--rw-rw-r--   0 user      (1000) user      (1000)     1016 2022-08-14 01:14:35.000000 red_team_language-0.1.1/rtl/parser/credential.py
--rw-rw-r--   0 user      (1000) user      (1000)     3776 2022-09-02 02:25:32.000000 red_team_language-0.1.1/rtl/parser/driver.py
--rw-r--r--   0 user      (1000) user      (1000)     8541 2022-08-30 00:57:56.000000 red_team_language-0.1.1/rtl/parser/executable.py
--rw-rw-r--   0 user      (1000) user      (1000)     1317 2022-08-21 19:36:28.000000 red_team_language-0.1.1/rtl/parser/helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)      682 2022-08-14 01:14:35.000000 red_team_language-0.1.1/rtl/parser/host.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.677214 red_team_language-0.1.1/rtl/parser/protocol/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-07-24 18:49:51.000000 red_team_language-0.1.1/rtl/parser/protocol/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5001 2022-09-02 01:20:14.000000 red_team_language-0.1.1/rtl/parser/protocol/shell.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-07-24 18:49:47.000000 red_team_language-0.1.1/rtl/parser/protocol/ssh.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-07-24 18:49:43.000000 red_team_language-0.1.1/rtl/parser/protocol/tcp.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-27 01:21:30.677214 red_team_language-0.1.1/rtl/parser/transform/
--rw-r--r--   0 user      (1000) user      (1000)       33 2022-07-31 18:24:23.000000 red_team_language-0.1.1/rtl/parser/transform/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1394 2022-08-14 01:14:35.000000 red_team_language-0.1.1/rtl/parser/transform/transform.py
--rw-rw-r--   0 user      (1000) user      (1000)     5790 2022-09-02 01:20:26.000000 red_team_language-0.1.1/rtl/parser/transform/xor.py
--rw-r--r--   0 user      (1000) user      (1000)     2946 2022-09-02 02:25:18.000000 red_team_language-0.1.1/rtl/rtl.py
--rw-r--r--   0 user      (1000) user      (1000)     2000 2022-09-27 01:21:30.678214 red_team_language-0.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      180 2022-08-26 01:48:10.000000 red_team_language-0.1.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    35149 2022-07-27 00:04:51.000000 red_team_language-0.2.0/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2022-09-27 01:09:48.000000 red_team_language-0.2.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2910 2023-08-06 15:12:48.324770 red_team_language-0.2.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1329 2022-09-02 02:39:04.000000 red_team_language-0.2.0/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       77 2022-07-26 23:56:06.000000 red_team_language-0.2.0/pyproject.toml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/red_team_language.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2910 2023-08-06 15:12:48.000000 red_team_language-0.2.0/red_team_language.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    37573 2023-08-06 15:12:48.000000 red_team_language-0.2.0/red_team_language.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-06 15:12:48.000000 red_team_language-0.2.0/red_team_language.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       37 2023-08-06 15:12:48.000000 red_team_language-0.2.0/red_team_language.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       13 2023-08-06 15:12:48.000000 red_team_language-0.2.0/red_team_language.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2023-08-06 15:12:48.000000 red_team_language-0.2.0/red_team_language.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-27 01:14:06.000000 red_team_language-0.2.0/red_team_language.egg-info/zip-safe
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/
+-rw-rw-r--   0 user      (1000) user      (1000)      778 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/Dockerfile
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-08-06 15:12:21.000000 red_team_language-0.2.0/rtl/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/examples/shell/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      617 2023-07-21 19:54:56.000000 red_team_language-0.2.0/rtl/examples/shell/ctf_2023.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      585 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/executable_binary.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      130 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/executable_binary_inline.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/executable_script.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/executable_script_inline.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      189 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/executable_script_inline_obfuscated.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      239 2023-08-03 00:48:30.000000 red_team_language-0.2.0/rtl/examples/shell/executable_script_obfuscated.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      197 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/executable_script_path.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      124 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/examples/shell/executable_script_ssh.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/failure_unknown_script.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      360 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/openssl_reverse_shell.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)      137 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/shell_double_executable.rtl
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/examples/shell/shell_executable.rtl
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/examples/ssh/
+-rw-rw-r--   0 user      (1000) user      (1000)      240 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/examples/ssh/executable_script_ssh.rtl
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)      271 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/lib/protocol/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/common/
+-rw-rw-r--   0 user      (1000) user      (1000)      728 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/common/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      494 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/common/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      418 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/common/main.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1568 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/common/rtl_common.c
+-rw-rw-r--   0 user      (1000) user      (1000)      243 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/common/rtl_common.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/shell/
+-rw-rw-r--   0 user      (1000) user      (1000)      820 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/shell/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      546 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/lib/protocol/shell/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)   900350 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/lib/protocol/shell/main.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/shell/shell.c
+-rw-rw-r--   0 user      (1000) user      (1000)      359 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/lib/protocol/shell/shell.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/
+-rw-rw-r--   0 user      (1000) user      (1000)     1677 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      463 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/3.22.1/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/3.22.1/CompilerIdC/
+-rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)       58 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_ARPA_INET_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_INTTYPES_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_NETINET_IN_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       58 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_IOCTL_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       58 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_PARAM_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_SELECT_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_SOCKET_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_TIME_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       56 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_UIO_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       55 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_SYS_UN_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)       55 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/CMakeFiles/CheckIncludeFiles/HAVE_UNISTD_H.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7503 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/docs/
+-rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/docs/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/src/
+-rw-rw-r--   0 user      (1000) user      (1000)    30948 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/src/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     2548 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/build/src/libssh2_config.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/
+-rw-rw-r--   0 user      (1000) user      (1000)    10317 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/direct_tcpip.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4964 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/scp.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7785 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/scp_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5900 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/scp_write.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7624 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/scp_write_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8848 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10134 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_RW_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6804 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_append.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4907 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_mkdir.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4916 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_mkdir_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8050 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6249 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_write.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7892 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_write_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8276 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftp_write_sliding.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8841 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftpdir.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6735 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/sftpdir_nonblock.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10934 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/ssh2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6993 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/ssh2_agent.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7853 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/ssh2_agent_forwarding.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10585 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/ssh2_echo.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8297 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/ssh2_exec.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8741 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/subsystem_netconf.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10162 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/tcpip-forward.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12852 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/example/x11.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/include/
+-rw-rw-r--   0 user      (1000) user      (1000)    58602 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/include/libssh2.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4909 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/include/libssh2_publickey.h
+-rw-rw-r--   0 user      (1000) user      (1000)    16768 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/include/libssh2_sftp.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/
+-rw-rw-r--   0 user      (1000) user      (1000)     7037 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/ccsid.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/include/
+-rw-rw-r--   0 user      (1000) user      (1000)     1824 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/include/alloca.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2086 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/include/assert.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2570 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/include/stdio.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.292770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/include/sys/
+-rw-rw-r--   0 user      (1000) user      (1000)     2409 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/include/sys/socket.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2396 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/libssh2_ccsid.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6551 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/libssh2_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8340 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/macros.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5402 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/os400/os400sys.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.296770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/
+-rw-rw-r--   0 user      (1000) user      (1000)    31747 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/agent.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14690 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/agent_win.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6729 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/bcrypt_pbkdf.c
+-rw-rw-r--   0 user      (1000) user      (1000)    31289 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/blowfish.c
+-rw-rw-r--   0 user      (1000) user      (1000)   106325 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/channel.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4759 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/channel.h
+-rw-rw-r--   0 user      (1000) user      (1000)    10891 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/comp.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/comp.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12611 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/crypt.c
+-rw-rw-r--   0 user      (1000) user      (1000)      349 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/crypto.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15759 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/crypto.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/global.c
+-rw-rw-r--   0 user      (1000) user      (1000)    39333 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/hostkey.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3492 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/keepalive.c
+-rw-rw-r--   0 user      (1000) user      (1000)   161966 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/kex.c
+-rw-rw-r--   0 user      (1000) user      (1000)    42762 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/knownhost.c
+-rw-rw-r--   0 user      (1000) user      (1000)    19471 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/libgcrypt.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9745 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/libgcrypt.h
+-rw-rw-r--   0 user      (1000) user      (1000)    42642 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/libssh2_priv.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2562 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/libssh2_setup.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13132 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/mac.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2577 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/mac.h
+-rw-rw-r--   0 user      (1000) user      (1000)    41075 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/mbedtls.c
+-rw-rw-r--   0 user      (1000) user      (1000)    23352 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/mbedtls.h
+-rw-rw-r--   0 user      (1000) user      (1000)    25084 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/misc.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5686 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/misc.h
+-rw-rw-r--   0 user      (1000) user      (1000)   120738 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/openssl.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15554 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/openssl.h
+-rw-rw-r--   0 user      (1000) user      (1000)    74000 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/os400qc3.c
+-rw-rw-r--   0 user      (1000) user      (1000)    19938 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/os400qc3.h
+-rw-rw-r--   0 user      (1000) user      (1000)    61243 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/packet.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3506 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/packet.h
+-rw-rw-r--   0 user      (1000) user      (1000)    26766 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/pem.c
+-rw-rw-r--   0 user      (1000) user      (1000)    47281 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/publickey.c
+-rw-rw-r--   0 user      (1000) user      (1000)    43657 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/scp.c
+-rw-rw-r--   0 user      (1000) user      (1000)    57759 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/session.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3645 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/session.h
+-rw-rw-r--   0 user      (1000) user      (1000)   133187 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/sftp.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7683 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/sftp.h
+-rw-rw-r--   0 user      (1000) user      (1000)    45274 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/transport.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3435 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/transport.h
+-rw-rw-r--   0 user      (1000) user      (1000)    96583 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/userauth.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2201 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/userauth.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6245 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/userauth_kbd_packet.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1832 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/userauth_kbd_packet.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1939 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/version.c
+-rw-rw-r--   0 user      (1000) user      (1000)    84835 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/wincng.c
+-rw-rw-r--   0 user      (1000) user      (1000)    24576 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/src/wincng.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.296770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)    13183 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/openssh_fixture.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1919 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/openssh_fixture.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.296770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/openssh_server/
+-rw-rw-r--   0 user      (1000) user      (1000)     3827 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/openssh_server/Dockerfile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.296770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/ossfuzz/
+-rw-rw-r--   0 user      (1000) user      (1000)       96 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/ossfuzz/testinput.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2601 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/runner.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1795 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/runner.h
+-rw-rw-r--   0 user      (1000) user      (1000)    14558 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/session_fixture.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2541 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/session_fixture.h
+-rw-rw-r--   0 user      (1000) user      (1000)      457 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_aa_warmup.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1576 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_agent_forward_ok.c
+-rw-rw-r--   0 user      (1000) user      (1000)      244 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_keyboard_fail.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8908 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_keyboard_info_request.c
+-rw-rw-r--   0 user      (1000) user      (1000)      242 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_keyboard_ok.c
+-rw-rw-r--   0 user      (1000) user      (1000)      244 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_password_fail_password.c
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_password_fail_username.c
+-rw-rw-r--   0 user      (1000) user      (1000)      242 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_password_ok.c
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_fail.c
+-rw-rw-r--   0 user      (1000) user      (1000)      346 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_dsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)      352 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_ecdsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)      435 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_ecdsa_signed.c
+-rw-rw-r--   0 user      (1000) user      (1000)      358 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_ed25519.c
+-rw-rw-r--   0 user      (1000) user      (1000)      383 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_ed25519_encrypted.c
+-rw-rw-r--   0 user      (1000) user      (1000)      361 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_ed25519_mem.c
+-rw-rw-r--   0 user      (1000) user      (1000)      351 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_rsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)      376 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_rsa_encrypted.c
+-rw-rw-r--   0 user      (1000) user      (1000)      431 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_rsa_openssh.c
+-rw-rw-r--   0 user      (1000) user      (1000)      434 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_auth_pubkey_ok_rsa_signed.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2464 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_hostkey.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6955 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_hostkey_hash.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3769 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_read.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2801 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_simple.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7033 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/tests/test_ssh2.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.296770 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/vms/
+-rw-rw-r--   0 user      (1000) user      (1000)     2328 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/vms/libssh2_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12822 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/libssh2/vms/man2help.c
+-rw-rw-r--   0 user      (1000) user      (1000)      712 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/main.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.296770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/
+-rw-rw-r--   0 user      (1000) user      (1000)     1096 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/Hacl_Curve25519.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8235 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/everest.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlib/
+-rw-rw-r--   0 user      (1000) user      (1000)     7003 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlib/FStar_UInt128.h
+-rw-rw-r--   0 user      (1000) user      (1000)    10800 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlib/FStar_UInt64_FStar_UInt32_FStar_UInt16_FStar_UInt8.h
+-rw-rw-r--   0 user      (1000) user      (1000)      985 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlib.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/
+-rw-rw-r--   0 user      (1000) user      (1000)     6747 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/c_endianness.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/
+-rw-rw-r--   0 user      (1000) user      (1000)      471 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/builtin.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/callconv.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1346 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/compat.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3056 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/debug.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3672 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/target.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2009 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/types.h
+-rw-rw-r--   0 user      (1000) user      (1000)      237 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/kremlin/internal/wasmsupport.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/vs2013/
+-rw-rw-r--   0 user      (1000) user      (1000)     1078 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/vs2013/Hacl_Curve25519.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/vs2013/inttypes.h
+-rw-rw-r--   0 user      (1000) user      (1000)      960 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/vs2013/stdbool.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6225 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/include/everest/x25519.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/
+-rw-rw-r--   0 user      (1000) user      (1000)    22405 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/Hacl_Curve25519.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1508 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/Hacl_Curve25519_joined.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3718 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/everest.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/kremlib/
+-rw-rw-r--   0 user      (1000) user      (1000)    14010 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/kremlib/FStar_UInt128_extracted.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5314 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/kremlib/FStar_UInt64_FStar_UInt32_FStar_UInt16_FStar_UInt8.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/legacy/
+-rw-rw-r--   0 user      (1000) user      (1000)    24161 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/legacy/Hacl_Curve25519.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5937 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/3rdparty/everest/library/x25519.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5560 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/3rdparty/
+-rw-rw-r--   0 user      (1000) user      (1000)     7735 2023-08-03 00:17:32.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/3rdparty/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/CMakeFiles/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/CMakeFiles/3.26.4/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/CMakeFiles/3.26.4/CompilerIdC/
+-rw-rw-r--   0 user      (1000) user      (1000)    26502 2023-08-03 00:17:31.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/CMakeFiles/3.26.4/CompilerIdC/CMakeCCompilerId.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9125 2023-08-03 00:17:32.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/include/
+-rw-rw-r--   0 user      (1000) user      (1000)     7730 2023-08-03 00:17:32.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/include/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/library/
+-rw-rw-r--   0 user      (1000) user      (1000)   127993 2023-08-03 00:17:32.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/library/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)    36873 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/library/error.c
+-rw-rw-r--   0 user      (1000) user      (1000)   108384 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/library/psa_crypto_driver_wrappers.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9091 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/library/ssl_debug_helpers_generated.c
+-rw-rw-r--   0 user      (1000) user      (1000)    28505 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/build/library/version_features.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/
+-rw-rw-r--   0 user      (1000) user      (1000)     3557 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/config-ccm-psk-dtls1_2.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3205 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/config-ccm-psk-tls1_2.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2528 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/config-no-entropy.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3751 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/config-suite-b.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2652 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/config-symmetric-only.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2605 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/configs/config-thread.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/docs/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/docs/architecture/
+-rw-rw-r--   0 user      (1000) user      (1000)      508 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/docs/architecture/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/docs/proposed/
+-rw-rw-r--   0 user      (1000) user      (1000)      456 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/docs/proposed/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.300770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/
+-rw-rw-r--   0 user      (1000) user      (1000)     3008 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_encdec.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1484 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_hashing.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3635 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_mainpage.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1446 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_rng.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1968 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_ssltls.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1686 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_tcpip.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1708 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/doxygen/input/doc_x509.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.304770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/
+-rw-rw-r--   0 user      (1000) user      (1000)    28058 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/aes.h
+-rw-rw-r--   0 user      (1000) user      (1000)    15644 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/aria.h
+-rw-rw-r--   0 user      (1000) user      (1000)    27658 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/asn1.h
+-rw-rw-r--   0 user      (1000) user      (1000)    15755 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/asn1write.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3156 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/base64.h
+-rw-rw-r--   0 user      (1000) user      (1000)    44891 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/bignum.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5004 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/build_info.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13826 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/camellia.h
+-rw-rw-r--   0 user      (1000) user      (1000)    25922 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ccm.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8292 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/chacha20.h
+-rw-rw-r--   0 user      (1000) user      (1000)    16140 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/chachapoly.h
+-rw-rw-r--   0 user      (1000) user      (1000)    45464 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/check_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)    53310 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/cipher.h
+-rw-rw-r--   0 user      (1000) user      (1000)     9903 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/cmac.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2278 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/compat-2.x.h
+-rw-rw-r--   0 user      (1000) user      (1000)    28434 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/config_psa.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1501 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/constant_time.h
+-rw-rw-r--   0 user      (1000) user      (1000)    25010 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ctr_drbg.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12122 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/debug.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13387 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/des.h
+-rw-rw-r--   0 user      (1000) user      (1000)    49986 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/dhm.h
+-rw-rw-r--   0 user      (1000) user      (1000)    19681 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ecdh.h
+-rw-rw-r--   0 user      (1000) user      (1000)    32221 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ecdsa.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13293 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ecjpake.h
+-rw-rw-r--   0 user      (1000) user      (1000)    60456 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ecp.h
+-rw-rw-r--   0 user      (1000) user      (1000)    10189 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/entropy.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7035 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/error.h
+-rw-rw-r--   0 user      (1000) user      (1000)    17661 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/gcm.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5753 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/hkdf.h
+-rw-rw-r--   0 user      (1000) user      (1000)    19068 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/hmac_drbg.h
+-rw-rw-r--   0 user      (1000) user      (1000)     9559 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/legacy_or_psa.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21268 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/lms.h
+-rw-rw-r--   0 user      (1000) user      (1000)   135093 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/mbedtls_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21343 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/md.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5902 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/md5.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5265 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/memory_buffer_alloc.h
+-rw-rw-r--   0 user      (1000) user      (1000)    11724 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/net_sockets.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7520 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/nist_kw.h
+-rw-rw-r--   0 user      (1000) user      (1000)    34905 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/oid.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6420 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/pem.h
+-rw-rw-r--   0 user      (1000) user      (1000)    43431 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/pk.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4733 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/pkcs12.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4823 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/pkcs5.h
+-rw-rw-r--   0 user      (1000) user      (1000)    10186 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/pkcs7.h
+-rw-rw-r--   0 user      (1000) user      (1000)    17161 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/platform.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1761 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/platform_time.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8429 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/platform_util.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6565 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/poly1305.h
+-rw-rw-r--   0 user      (1000) user      (1000)      978 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/private_access.h
+-rw-rw-r--   0 user      (1000) user      (1000)    14595 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/psa_util.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3984 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ripemd160.h
+-rw-rw-r--   0 user      (1000) user      (1000)    56410 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/rsa.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8044 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/sha1.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7385 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/sha256.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7845 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/sha512.h
+-rw-rw-r--   0 user      (1000) user      (1000)   255819 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ssl.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5871 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ssl_cache.h
+-rw-rw-r--   0 user      (1000) user      (1000)    25980 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ssl_ciphersuites.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3706 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ssl_cookie.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7218 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/ssl_ticket.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4381 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/threading.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3244 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/timing.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2813 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/version.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21978 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/x509.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6919 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/x509_crl.h
+-rw-rw-r--   0 user      (1000) user      (1000)    55740 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/x509_crt.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12197 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/mbedtls/x509_csr.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.304770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/
+-rw-rw-r--   0 user      (1000) user      (1000)   230408 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7770 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_builtin_composites.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3932 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_builtin_primitives.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6915 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_compat.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5690 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2102 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_driver_common.h
+-rw-rw-r--   0 user      (1000) user      (1000)     6479 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_driver_contexts_composites.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4620 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_driver_contexts_primitives.h
+-rw-rw-r--   0 user      (1000) user      (1000)    92158 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_extra.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3630 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_platform.h
+-rw-rw-r--   0 user      (1000) user      (1000)    68457 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_se_driver.h
+-rw-rw-r--   0 user      (1000) user      (1000)    52015 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_sizes.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21040 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_struct.h
+-rw-rw-r--   0 user      (1000) user      (1000)    18534 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_types.h
+-rw-rw-r--   0 user      (1000) user      (1000)   121718 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/include/psa/crypto_values.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.312770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/
+-rw-rw-r--   0 user      (1000) user      (1000)     9173 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)    73562 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/aes.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14122 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/aesce.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3670 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/aesce.h
+-rw-rw-r--   0 user      (1000) user      (1000)    31897 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/aesni.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5808 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/aesni.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21300 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/alignment.h
+-rw-rw-r--   0 user      (1000) user      (1000)    36529 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/aria.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12444 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/asn1parse.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13790 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/asn1write.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/base64.c
+-rw-rw-r--   0 user      (1000) user      (1000)    73754 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum.c
+-rw-rw-r--   0 user      (1000) user      (1000)    26511 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_core.c
+-rw-rw-r--   0 user      (1000) user      (1000)    34047 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_core.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12160 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_mod.c
+-rw-rw-r--   0 user      (1000) user      (1000)    20979 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_mod.h
+-rw-rw-r--   0 user      (1000) user      (1000)     9572 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_mod_raw.c
+-rw-rw-r--   0 user      (1000) user      (1000)    20642 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_mod_raw.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1572 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bignum_mod_raw_invasive.h
+-rw-rw-r--   0 user      (1000) user      (1000)    43214 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/bn_mul.h
+-rw-rw-r--   0 user      (1000) user      (1000)    35071 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/camellia.c
+-rw-rw-r--   0 user      (1000) user      (1000)    22646 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ccm.c
+-rw-rw-r--   0 user      (1000) user      (1000)    17447 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/chacha20.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15062 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/chachapoly.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3529 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/check_crypto_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)    51267 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/cipher.c
+-rw-rw-r--   0 user      (1000) user      (1000)    55132 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/cipher_wrap.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4792 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/cipher_wrap.h
+-rw-rw-r--   0 user      (1000) user      (1000)    33369 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/cmac.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5644 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/common.h
+-rw-rw-r--   0 user      (1000) user      (1000)    36296 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/constant_time.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14656 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/constant_time_internal.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/constant_time_invasive.h
+-rw-rw-r--   0 user      (1000) user      (1000)    28658 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ctr_drbg.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12103 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/debug.c
+-rw-rw-r--   0 user      (1000) user      (1000)    32697 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/des.c
+-rw-rw-r--   0 user      (1000) user      (1000)    20374 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/dhm.c
+-rw-rw-r--   0 user      (1000) user      (1000)    21971 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecdh.c
+-rw-rw-r--   0 user      (1000) user      (1000)    27774 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecdsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)    43428 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecjpake.c
+-rw-rw-r--   0 user      (1000) user      (1000)   115638 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecp.c
+-rw-rw-r--   0 user      (1000) user      (1000)   333782 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecp_curves.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11329 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecp_internal_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7587 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ecp_invasive.h
+-rw-rw-r--   0 user      (1000) user      (1000)    19866 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/entropy.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6550 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/entropy_poll.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2240 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/entropy_poll.h
+-rw-rw-r--   0 user      (1000) user      (1000)    36873 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/error.c
+-rw-rw-r--   0 user      (1000) user      (1000)    38451 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/gcm.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3615 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/hash_info.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3389 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/hash_info.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4504 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/hkdf.c
+-rw-rw-r--   0 user      (1000) user      (1000)    19508 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/hmac_drbg.c
+-rw-rw-r--   0 user      (1000) user      (1000)    29194 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/lmots.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14177 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/lmots.h
+-rw-rw-r--   0 user      (1000) user      (1000)    27425 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/lms.c
+-rw-rw-r--   0 user      (1000) user      (1000)    25821 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/md.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13041 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/md5.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2087 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/md_wrap.h
+-rw-rw-r--   0 user      (1000) user      (1000)    19132 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/memory_buffer_alloc.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7913 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/mps_common.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3762 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/mps_error.h
+-rw-rw-r--   0 user      (1000) user      (1000)    20021 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/mps_reader.c
+-rw-rw-r--   0 user      (1000) user      (1000)    17593 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/mps_reader.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2873 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/mps_trace.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6155 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/mps_trace.h
+-rw-rw-r--   0 user      (1000) user      (1000)    18604 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/net_sockets.c
+-rw-rw-r--   0 user      (1000) user      (1000)    22257 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/nist_kw.c
+-rw-rw-r--   0 user      (1000) user      (1000)    31108 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/oid.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4756 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/padlock.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3731 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/padlock.h
+-rw-rw-r--   0 user      (1000) user      (1000)    17200 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pem.c
+-rw-rw-r--   0 user      (1000) user      (1000)    29259 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pk.c
+-rw-rw-r--   0 user      (1000) user      (1000)    51344 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pk_wrap.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5875 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pk_wrap.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13523 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pkcs12.c
+-rw-rw-r--   0 user      (1000) user      (1000)    17486 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pkcs5.c
+-rw-rw-r--   0 user      (1000) user      (1000)    23260 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pkcs7.c
+-rw-rw-r--   0 user      (1000) user      (1000)    47236 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pkparse.c
+-rw-rw-r--   0 user      (1000) user      (1000)    17380 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pkwrite.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4071 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/pkwrite.h
+-rw-rw-r--   0 user      (1000) user      (1000)    11466 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/platform.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7785 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/platform_util.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14992 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/poly1305.c
+-rw-rw-r--   0 user      (1000) user      (1000)   273456 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto.c
+-rw-rw-r--   0 user      (1000) user      (1000)    23459 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_aead.c
+-rw-rw-r--   0 user      (1000) user      (1000)    24438 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_aead.h
+-rw-rw-r--   0 user      (1000) user      (1000)    19390 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_cipher.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15025 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_cipher.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2508 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)    37737 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_core.h
+-rw-rw-r--   0 user      (1000) user      (1000)   108384 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_driver_wrappers.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13370 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_driver_wrappers.h
+-rw-rw-r--   0 user      (1000) user      (1000)    19527 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_ecp.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13414 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_ecp.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12021 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_hash.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9681 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_hash.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3211 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_invasive.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7059 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_its.h
+-rw-rw-r--   0 user      (1000) user      (1000)    15539 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_mac.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12308 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_mac.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21066 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_pake.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7461 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_pake.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7066 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_random_impl.h
+-rw-rw-r--   0 user      (1000) user      (1000)    26674 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_rsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)    16515 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_rsa.h
+-rw-rw-r--   0 user      (1000) user      (1000)    12815 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_se.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6973 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_se.h
+-rw-rw-r--   0 user      (1000) user      (1000)    18745 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_slot_management.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8164 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_slot_management.h
+-rw-rw-r--   0 user      (1000) user      (1000)    16902 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_storage.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15709 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_crypto_storage.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8082 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_its_file.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5685 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/psa_util.c
+-rw-rw-r--   0 user      (1000) user      (1000)    16707 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ripemd160.c
+-rw-rw-r--   0 user      (1000) user      (1000)    76123 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/rsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14152 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/rsa_alt_helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8846 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/rsa_alt_helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)    14685 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/sha1.c
+-rw-rw-r--   0 user      (1000) user      (1000)    28678 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/sha256.c
+-rw-rw-r--   0 user      (1000) user      (1000)    37224 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/sha512.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11123 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_cache.c
+-rw-rw-r--   0 user      (1000) user      (1000)    92945 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_ciphersuites.c
+-rw-rw-r--   0 user      (1000) user      (1000)    33698 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)      986 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_client.h
+-rw-rw-r--   0 user      (1000) user      (1000)    11224 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_cookie.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3399 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_debug_helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)     9091 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_debug_helpers_generated.c
+-rw-rw-r--   0 user      (1000) user      (1000)   108105 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_misc.h
+-rw-rw-r--   0 user      (1000) user      (1000)   209289 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_msg.c
+-rw-rw-r--   0 user      (1000) user      (1000)    16792 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_ticket.c
+-rw-rw-r--   0 user      (1000) user      (1000)   319813 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls.c
+-rw-rw-r--   0 user      (1000) user      (1000)   130546 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls12_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)   154945 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls12_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)   103215 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls13_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)    58006 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls13_generic.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1156 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls13_invasive.h
+-rw-rw-r--   0 user      (1000) user      (1000)    67284 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls13_keys.c
+-rw-rw-r--   0 user      (1000) user      (1000)    29083 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls13_keys.h
+-rw-rw-r--   0 user      (1000) user      (1000)   107155 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/ssl_tls13_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6248 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/threading.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4515 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/timing.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1189 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/version.c
+-rw-rw-r--   0 user      (1000) user      (1000)    28505 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/version_features.c
+-rw-rw-r--   0 user      (1000) user      (1000)    50057 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12759 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509_create.c
+-rw-rw-r--   0 user      (1000) user      (1000)    21572 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509_crl.c
+-rw-rw-r--   0 user      (1000) user      (1000)    89493 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509_crt.c
+-rw-rw-r--   0 user      (1000) user      (1000)    17888 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509_csr.c
+-rw-rw-r--   0 user      (1000) user      (1000)    24629 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509write_crt.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14734 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/library/x509write_csr.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.312770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/
+-rw-rw-r--   0 user      (1000) user      (1000)    16988 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.312770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/aes/
+-rw-rw-r--   0 user      (1000) user      (1000)    18692 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/aes/crypt_and_hash.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.312770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/cipher/
+-rw-rw-r--   0 user      (1000) user      (1000)     9036 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/cipher/cipher_aead_demo.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.312770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/
+-rw-rw-r--   0 user      (1000) user      (1000)     1859 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     2475 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/common.c
+-rw-rw-r--   0 user      (1000) user      (1000)      749 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/common.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5577 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3561 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_dtlsclient.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5376 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_dtlsserver.c
+-rw-rw-r--   0 user      (1000) user      (1000)      339 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_pkcs7.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3012 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_privkey.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2460 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_pubkey.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6589 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)      660 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_x509crl.c
+-rw-rw-r--   0 user      (1000) user      (1000)      660 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_x509crt.c
+-rw-rw-r--   0 user      (1000) user      (1000)      660 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/fuzz_x509csr.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/fuzz/onefile.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.312770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/hash/
+-rw-rw-r--   0 user      (1000) user      (1000)     5691 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/hash/generic_sum.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1400 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/hash/hello.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5214 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/hash/md_hmac_demo.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/
+-rw-rw-r--   0 user      (1000) user      (1000)     8540 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/dh_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5183 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/dh_genprime.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9508 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/dh_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6007 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/ecdh_curve25519.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6726 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/ecdsa.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12891 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/gen_key.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11178 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/key_app.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13066 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/key_app_writer.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3394 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/mpi_demo.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4491 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/pk_decrypt.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4569 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/pk_encrypt.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4709 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/pk_sign.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3509 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/pk_verify.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5608 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_decrypt.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4774 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_encrypt.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5306 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_genkey.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5126 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_sign.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4951 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_sign_pss.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3918 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_verify.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3905 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/pkey/rsa_verify_pss.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/
+-rw-rw-r--   0 user      (1000) user      (1000)    10269 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/aead_demo.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12081 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/crypto_examples.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6225 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/hmac_demo.c
+-rw-rw-r--   0 user      (1000) user      (1000)    26589 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/key_ladder_demo.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10905 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/psa_constant_names.c
+-rw-rw-r--   0 user      (1000) user      (1000)    28073 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/psa/psa_constant_names_generated.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/random/
+-rw-rw-r--   0 user      (1000) user      (1000)     2422 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/random/gen_entropy.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3628 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/random/gen_random_ctr_drbg.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/
+-rw-rw-r--   0 user      (1000) user      (1000)    10129 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/dtls_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11939 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/dtls_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10160 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/mini_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8538 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_client1.c
+-rw-rw-r--   0 user      (1000) user      (1000)   122683 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_client2.c
+-rw-rw-r--   0 user      (1000) user      (1000)    31558 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_context_info.c
+-rw-rw-r--   0 user      (1000) user      (1000)    12103 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_fork_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)    25464 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_mail_client.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14924 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_pthread_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10791 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_server.c
+-rw-rw-r--   0 user      (1000) user      (1000)   162615 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_server2.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13047 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_test_common_source.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13346 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_test_lib.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10950 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/ssl/ssl_test_lib.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/
+-rw-rw-r--   0 user      (1000) user      (1000)    45755 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/benchmark.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/cmake_package/
+-rw-rw-r--   0 user      (1000) user      (1000)     1246 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/cmake_package/cmake_package.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/cmake_package_install/
+-rw-rw-r--   0 user      (1000) user      (1000)     1261 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/cmake_package_install/cmake_package_install.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/cmake_subproject/
+-rw-rw-r--   0 user      (1000) user      (1000)     1265 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/cmake_subproject/cmake_subproject.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3792 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/dlopen.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2489 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/query_compile_time_config.c
+-rw-rw-r--   0 user      (1000) user      (1000)   146981 2023-03-27 17:05:28.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/query_config.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1695 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/query_config.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1205 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/query_included_headers.c
+-rw-rw-r--   0 user      (1000) user      (1000)    17353 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/selftest.c
+-rw-rw-r--   0 user      (1000) user      (1000)    31749 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/udp_proxy.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2632 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/test/zeroize.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/util/
+-rw-rw-r--   0 user      (1000) user      (1000)     6122 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/util/pem2der.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1936 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/util/strerror.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1166 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/wince_main.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/
+-rw-rw-r--   0 user      (1000) user      (1000)    15129 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/cert_app.c
+-rw-rw-r--   0 user      (1000) user      (1000)    16769 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/cert_req.c
+-rw-rw-r--   0 user      (1000) user      (1000)    34441 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/cert_write.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3299 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/crl_app.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5479 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/load_roots.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3317 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/programs/x509/req_app.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.316770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/
+-rwxrwxr-x   0 user      (1000) user      (1000)    28050 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/abi_check.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    21450 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/assemble_changelog.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     8296 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/code_size_compare.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     8637 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/code_style.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    25317 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/config.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7446 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/ecp_comb_table.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     8163 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/generate_driver_wrappers.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    12545 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/generate_psa_constants.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    14498 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/generate_ssl_debug_helpers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/
+-rw-rw-r--   0 user      (1000) user      (1000)      146 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14170 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/asymmetric_key_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15089 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/bignum_common.py
+-rw-rw-r--   0 user      (1000) user      (1000)    35067 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/bignum_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7178 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/bignum_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4615 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/bignum_mod.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10161 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/bignum_mod_raw.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2320 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/build_tree.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6095 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/c_build_helper.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23272 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/crypto_knowledge.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13931 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/ecp.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23838 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/macro_collector.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8562 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/psa_storage.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3494 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/test_case.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9347 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/test_data_generation.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/mbedtls_dev/typing_util.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     5646 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/scripts/min_requirements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)    11927 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/configs/
+-rw-rw-r--   0 user      (1000) user      (1000)     1085 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/configs/config-wrapper-malloc-0-null.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/configs/tls13-only.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2123 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/configs/user-config-for-test.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/data_files/
+-rw-rw-r--   0 user      (1000) user      (1000)    85825 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/data_files/Makefile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/docker/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/docker/bionic/
+-rw-rw-r--   0 user      (1000) user      (1000)     5945 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/docker/bionic/Dockerfile
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/
+-rw-rw-r--   0 user      (1000) user      (1000)      970 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/aes_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      848 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/aria_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/camellia_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      841 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/ccm_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/chacha20_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      921 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/chachapoly_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      821 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/cmac_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      922 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/des_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      841 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/dhm_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      869 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/ecjpake_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1035 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/ecp_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      841 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/gcm_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      841 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/md5_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      845 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/nist_kw_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      891 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/platform_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      876 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/poly1305_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      883 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/ripemd160_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      841 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/rsa_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      848 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/sha1_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      862 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/sha256_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      862 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/sha512_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      882 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/threading_alt.h
+-rw-rw-r--   0 user      (1000) user      (1000)      925 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-dummy/timing_alt.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.288770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-extra/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-extra/psa/
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/alt-extra/psa/crypto.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/baremetal-override/
+-rw-rw-r--   0 user      (1000) user      (1000)      721 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/baremetal-override/time.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/spe/
+-rw-rw-r--   0 user      (1000) user      (1000)     5082 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/spe/crypto_spe.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/
+-rw-rw-r--   0 user      (1000) user      (1000)     2076 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/asn1_helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4695 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/bignum_helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)     9248 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/certs.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3025 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/constant_flow.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/
+-rw-rw-r--   0 user      (1000) user      (1000)     4758 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/aead.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3240 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/asymmetric_encryption.h
+-rw-rw-r--   0 user      (1000) user      (1000)     5293 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/cipher.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1822 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/config_test_driver.h
+-rw-rw-r--   0 user      (1000) user      (1000)     7212 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/crypto_config_test_driver_extension.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2658 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/hash.h
+-rw-rw-r--   0 user      (1000) user      (1000)     2476 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/key_agreement.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4927 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/key_management.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4433 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/mac.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3123 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/pake.h
+-rw-rw-r--   0 user      (1000) user      (1000)     4186 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/signature.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1440 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/drivers/test_driver.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1932 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/fake_external_rng_for_test.h
+-rw-rw-r--   0 user      (1000) user      (1000)    10104 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)    11015 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/macros.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13818 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/psa_crypto_helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)     8810 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/psa_exercise_key.h
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/psa_helpers.h
+-rw-rw-r--   0 user      (1000) user      (1000)     3295 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/random.h
+-rw-rw-r--   0 user      (1000) user      (1000)    21922 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/include/test/ssl_helpers.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.320770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/
+-rwxrwxr-x   0 user      (1000) user      (1000)     9765 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/analyze_outcomes.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    16356 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/check_files.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    36634 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/check_names.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     8737 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/check_test_cases.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    26778 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/depends.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7173 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/generate_bignum_tests.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1279 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/generate_ecp_tests.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7438 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/generate_pkcs7_tests.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    41950 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/generate_psa_tests.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    44695 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/generate_test_code.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    23779 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/generate_tls13_compat_tests.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1996 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/list_internal_identifiers.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     5748 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/psa_collect_statuses.py
+-rw-rw-r--   0 user      (1000) user      (1000)      932 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/scripts_path.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    11860 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/set_psa_test_dependencies.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7451 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/test_config_script.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    57951 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/test_generate_test_code.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     5700 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/test_psa_compliance.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     8117 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/test_psa_constant_names.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     6387 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/scripts/translate_ciphers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/
+-rw-rw-r--   0 user      (1000) user      (1000)     2230 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/asn1_helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4207 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/bignum_helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)   112089 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/certs.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/
+-rw-rw-r--   0 user      (1000) user      (1000)     7573 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/hash.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3387 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/platform_builtin_keys.c
+-rw-rw-r--   0 user      (1000) user      (1000)    18217 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_aead.c
+-rw-rw-r--   0 user      (1000) user      (1000)     6015 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_asymmetric_encryption.c
+-rw-rw-r--   0 user      (1000) user      (1000)    13891 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_cipher.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4072 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_key_agreement.c
+-rw-rw-r--   0 user      (1000) user      (1000)    28342 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_key_management.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14401 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_mac.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7585 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_pake.c
+-rw-rw-r--   0 user      (1000) user      (1000)    14141 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/drivers/test_driver_signature.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1719 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/fake_external_rng_for_test.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10280 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)     4322 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/psa_crypto_helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)    37165 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/psa_exercise_key.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3774 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/random.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/test_helpers/
+-rw-rw-r--   0 user      (1000) user      (1000)    76922 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/test_helpers/ssl_helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)     8275 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/mbedtls/tests/src/threading_helpers.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9900 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/ssh.c
+-rw-rw-r--   0 user      (1000) user      (1000)      523 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/lib/protocol/ssh/ssh.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/lib/transform/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:32.000000 red_team_language-0.2.0/rtl/lib/transform/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/lib/transform/xor/
+-rw-rw-r--   0 user      (1000) user      (1000)      598 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/lib/transform/xor/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      463 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/lib/transform/xor/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1297 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/lib/transform/xor/main.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1256 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/lib/transform/xor/xor.c
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/parser/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/parser/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      440 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/_with.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1180 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/credential.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3768 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/driver.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8534 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/executable.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1540 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      520 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/host.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2314 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/kvstore.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/parser/protocol/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/parser/protocol/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5094 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/protocol/shell.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6974 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/parser/protocol/ssh.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/parser/protocol/tcp.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-06 15:12:48.324770 red_team_language-0.2.0/rtl/parser/transform/
+-rw-rw-r--   0 user      (1000) user      (1000)       33 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/parser/transform/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1394 2023-08-03 00:48:54.000000 red_team_language-0.2.0/rtl/parser/transform/transform.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5790 2023-07-21 19:23:33.000000 red_team_language-0.2.0/rtl/parser/transform/xor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3964 2023-08-06 15:09:00.000000 red_team_language-0.2.0/rtl/rtl.py
+-rw-r--r--   0 user      (1000) user      (1000)     2000 2023-08-06 15:12:48.324770 red_team_language-0.2.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      180 2022-08-26 01:48:10.000000 red_team_language-0.2.0/setup.py
```

### Comparing `red_team_language-0.1.1/LICENSE` & `red_team_language-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/PKG-INFO` & `red_team_language-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red_team_language
-Version: 0.1.1
+Version: 0.2.0
 Summary: Red-Team-Language - something snazzy
 Home-page: https://github.com/ArchiMoebius/rtl
 Download-URL: https://github.com/ArchiMoebius/rtl
 Author: Archi Moebius
 Author-email: ArchiMoebius@dojobebo.com
 Maintainer: Archi Moebius
 Maintainer-email: ArchiMoebius@dojobebo.com
```

### Comparing `red_team_language-0.1.1/README.md` & `red_team_language-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/red_team_language.egg-info/PKG-INFO` & `red_team_language-0.2.0/red_team_language.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-team-language
-Version: 0.1.1
+Version: 0.2.0
 Summary: Red-Team-Language - something snazzy
 Home-page: https://github.com/ArchiMoebius/rtl
 Download-URL: https://github.com/ArchiMoebius/rtl
 Author: Archi Moebius
 Author-email: ArchiMoebius@dojobebo.com
 Maintainer: Archi Moebius
 Maintainer-email: ArchiMoebius@dojobebo.com
```

### Comparing `red_team_language-0.1.1/rtl/Dockerfile` & `red_team_language-0.2.0/rtl/Dockerfile`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/examples/shell/executable_binary.rtl` & `red_team_language-0.2.0/rtl/examples/shell/executable_binary.rtl`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/lib/protocol/shell/Makefile` & `red_team_language-0.2.0/rtl/lib/protocol/shell/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 CFLAGS=-O2 -D_FORTIFY_SOURCE=2 -fpie -pie -fstack-protector -flto -Wl,-z,now -Wl,-z,relro -Wformat -Wformat-security -Werror=format-security
 RTL_TARGET ?= x86_64-linux-musl
+INCLUDES=-I../common/
 
 all: shell
 	@echo
 
-shell:
-	@clang -S -emit-llvm -c -no-integrated-as shell.c -Wa,-aln=shell.ll
+rtl_common.o:
+	@make -C ../common/
+	@cp ../common/rtl_common.o ./
+
+shell: rtl_common.o
+	@clang -S -emit-llvm -c ${INCLUDES} -no-integrated-as shell.c -Wa,-aln=shell.ll
 	@# clang ${CFLAGS} -std=c11 -c -fPIC -Wall shell.c -o shell.o
 	@zig cc ${CFLAGS} -target ${RTL_TARGET} -c -fPIC -Wall shell.c -o shell.o
 
 
 main: shell
-	@# clang ${CFLAGS} -std=c11 -fPIC -Wall shell.o main.c -o main
-	@zig cc ${CFLAGS} -target ${RTL_TARGET} -fPIC -Wall shell.o main.c -o main -Wl,-s
+	@# clang ${INCLUDES} ${CFLAGS} -std=c11 -fPIC -Wall shell.o main.c -o main
+	@zig cc ${INCLUDES} ${CFLAGS} -target ${RTL_TARGET} -fPIC -Wall shell.o rtl_common.o main.c -o main -Wl,-s
 
 clean:
-	@rm shell.ll shell.o main &> /dev/null || echo
+	@rm -f shell.ll shell.o rtl_common.o main &> /dev/null || echo
+	@make -C ../common/ clean;
```

### Comparing `red_team_language-0.1.1/rtl/lib/protocol/shell/__init__.py` & `red_team_language-0.2.0/rtl/lib/protocol/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/lib/protocol/shell/main.c` & `red_team_language-0.2.0/rtl/lib/protocol/shell/main.c`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/lib/protocol/shell/shell.c` & `red_team_language-0.2.0/rtl/lib/protocol/shell/shell.c`

 * *Files 27% similar despite different names*

```diff
@@ -7,58 +7,22 @@
 #include <stdlib.h>
 #include <string.h>
 #include <sys/mman.h>
 #include <sys/wait.h>
 #include <unistd.h>
 
 #include "shell.h"
-
-unsigned char **parse_protocol_shell_argument_buffer(unsigned char *buf) {
-
-  uint16_t argc = 0;
-
-  if (buf != NULL) {
-    argc = (uint16_t) * (buf);
-  }
-
-  uint16_t offset = sizeof(uint16_t);
-
-  unsigned char **argv = calloc(argc + 1, sizeof(unsigned char *));
-
-  for (uint16_t i = 0; i < argc; i++) {
-    uint16_t arg_sz = (uint16_t) * (buf + offset);
-    offset += sizeof(uint16_t);
-
-    argv[i] = calloc(arg_sz + 1, sizeof(unsigned char));
-
-    memcpy(argv[i], buf + offset, arg_sz);
-
-    offset += arg_sz;
-  }
-
-  argv[argc] = NULL;
-
-#ifdef DEBUG
-  printf("Argument Buffer: \n");
-  int i = 0;
-  while (argv[i] != NULL) {
-    printf("\targ[%d] = |||%s|||\n", i, argv[i]);
-    i++;
-  }
-#endif
-
-  return argv;
-}
+#include "../common/rtl_common.h"
 
 extern int protocol_shell(uint32_t method, unsigned char *buf,
                           uint32_t buf_size, unsigned char *argv_buf,
                           unsigned char *envp_buf) {
 
-  unsigned char **argv = parse_protocol_shell_argument_buffer(argv_buf);
-  unsigned char **envp = parse_protocol_shell_argument_buffer(envp_buf);
+  unsigned char **argv = rtl_parse_protocol_argument_buffer(argv_buf);
+  unsigned char **envp = rtl_parse_protocol_argument_buffer(envp_buf);
 
   // function table, would be nice - prob. break things out and clean this up
   // at somepoint...
 
   if (method == RTL_PROTOCOL_SHELL_METHOD_MEMFD) {
     int a = memfd_create("", 0);
```

### Comparing `red_team_language-0.1.1/rtl/lib/transform/xor/Makefile` & `red_team_language-0.2.0/rtl/lib/transform/xor/Makefile`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/lib/transform/xor/main.c` & `red_team_language-0.2.0/rtl/lib/transform/xor/main.c`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/lib/transform/xor/xor.c` & `red_team_language-0.2.0/rtl/lib/transform/xor/xor.c`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/parser/driver.py` & `red_team_language-0.2.0/rtl/parser/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from rtl.parser.credential import Credential
 from rtl.parser.host import Host
 from rtl.parser.executable import Executable
 from rtl.parser._with import With
 
 
 class Driver:
-
     LINE_TRIGGER_MAP = {
         Credential.LINE_TRIGGER: Credential.parse,
         Host.LINE_TRIGGER: Host.parse,
         Executable.LINE_TRIGGER: Executable.parse,
         With.LINE_TRIGGER: With.parse,
     }
     LINE_TRIGGERS = LINE_TRIGGER_MAP.keys()
@@ -43,42 +42,37 @@
         self.script = []
         self.__llvm_module = ""
 
         self._parse()
         self._build()
 
     def _parse(self):
-
         with open(self.filepath, "r") as fh:
             line = True
 
             while line:
-
                 line = fh.readline()
 
                 tokens = line.strip().split(" ")
 
                 if tokens[0].startswith("#"):
                     continue
 
                 for trigger_key in self.LINE_TRIGGERS:
-
                     if trigger_key == tokens[0]:
                         self.script.append(self.LINE_TRIGGER_MAP[trigger_key](tokens, fh))
 
     def _build(self):
-
         function_type = llvmir.FunctionType(llvmir.IntType(32), [])
         function = llvmir.Function(self.module, function_type, name="main")
         block_main = function.append_basic_block("entry")
         irbuilder = llvmir.IRBuilder(block_main)
         irbuilder.position_at_end(block_main)
 
         for entry in self.script:
-
             if entry:
                 entry.IR(irbuilder)
 
         irbuilder.ret(llvmir.Constant(llvmir.IntType(32), 0))
 
         # LLVM-IR ==> in-memory representation
         self.__llvm_module = llvm.parse_assembly(str(self.module))
@@ -102,15 +96,14 @@
         else:
             filename = PosixPath(args.dst)
 
             if not filename.parent.exists():
                 filename.parent.mkdir(parents=True, exist_ok=True)
 
         if not args.ir:
-
             # tm = llvm.Target.from_default_triple().create_target_machine()
             tm = llvm.Target.from_triple(self.rtl_target).create_target_machine()
 
             # Compile the module to machine code using MCJIT
             with llvm.create_mcjit_compiler(self.__llvm_module, tm) as ee:
                 ee.finalize_object()
 
@@ -120,14 +113,13 @@
                 if args.obj:
                     with open(filename, "wb") as fh:
                         fh.write(tm.emit_object(self.__llvm_module))
 
                     ret = filename
 
         if not args.obj and args.dst is not None:
-
             with open(filename, "w") as fh:
                 fh.write(str(ret))
 
             ret = filename
 
         return ret
```

### Comparing `red_team_language-0.1.1/rtl/parser/executable.py` & `red_team_language-0.2.0/rtl/parser/executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class Executable:
     LINE_TRIGGER = "executable"
     EXECUTABLES = {}
     RTL_PROTOCOL_SHELL_BINARY_EXECUTION_METHODS = {"MEMFD": 0, "TEMPFS": 1}
 
     def __init__(self, id, content, transform, options):
-
         if self.EXECUTABLES.get(id, False):
             raise Exception(f"Multiple instances of {id} found - pick a different identifier...!")
 
         self.id = id
         self.content = content
         self.transform = transform
         self.options = options
@@ -85,15 +84,14 @@
         content = ""
         transform = SimpleNamespace(transforms=[])
 
         tokens = " ".join(tokens[2:]).split(":")
 
         c = 0
         for token in tokens:
-
             if "method" == token:
                 options.method = tokens[c + 1].strip()
 
             if "name" == token:
                 options.name = tokens[c + 1].strip()
 
             if "path" == token:
@@ -112,15 +110,14 @@
 
             if line == "" or line == "!!!":
                 break
 
             line_tokens = line.split(" ")
 
             if line_tokens[0] == "content":
-
                 while True:
                     line = fh.readline()
 
                     if len(line.strip()) > 0 and line.strip()[0] == "#":
                         continue
 
                     if line.strip() == "!!!":
@@ -174,29 +171,26 @@
             raise Exception(f"The option :path: option or content block is required - example :path:/bin/sh")
 
         executable_bytes = b""
 
         binary_path = PosixPath(filepath)
 
         if self.content != "":
-
             executable_bytes = bytes(self.content, "utf8") + b"\x00"
             shell = self.options.path
 
             if shell:
-
                 if "#!" not in shell:
                     shell = f"#!{shell}"
 
             else:
                 shell = "#!/bin/sh"
 
             executable_bytes = bytes(shell, "utf8") + b"\n" + executable_bytes
         else:
-
             if not binary_path.exists() or not binary_path.is_file():
                 raise Exception(f"binary does not exist at path : {binary_path}")
 
             with open(binary_path, "rb") as fh:
                 executable_bytes = fh.read()
 
         func_ty = ir.FunctionType(ir.PointerType(ir.IntType(8)), [])  # function returns a char*
@@ -222,15 +216,14 @@
         return f"{self.id}.argv.bytes"
 
     @property
     def argv_size(self):
         return f"{self.id}.argv.size"
 
     def IR_argv(self, builder):
-
         name = self.options.name
 
         if name == False:
             name = self.id
 
         # argv[0] is the binary name in the process list
         self.options.argv.insert(0, name)
```

### Comparing `red_team_language-0.1.1/rtl/parser/helpers.py` & `red_team_language-0.2.0/rtl/parser/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,25 @@
             ir.ArrayType(ir.IntType(8), data_len),
             [i for i in data],
         )
 
     return gv
 
 
+def helper_parse_options(tokens):
+    options = {}
+
+    for entry in tokens:
+        if ":" in entry and isinstance(entry, str):
+            kva = entry.split(":")
+            options[kva[0]] = kva[1]
+
+    return options
+
+
 def helper_create_global_int(module, symbol_name, value):
     gv = ir.GlobalVariable(
         module,
         ir.IntType(32),
         symbol_name,
     )
     gv.global_constant = False
```

### Comparing `red_team_language-0.1.1/rtl/parser/protocol/shell.py` & `red_team_language-0.2.0/rtl/parser/protocol/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import llvmlite.ir as ir
 import llvmlite.binding as llvm
 
-
+from rtl.lib.protocol.common import COMMON_LLVM_O
 from rtl.lib.protocol.shell import SHELL_LLVM_O, RTL_PROTOCOL_SHELL_EXECUTION_METHODS  # recompile things...every import...so dirty...
 from rtl.parser.executable import Executable
 from rtl.parser.helpers import helper_generate_id
 
+llvm.ObjectFileRef.from_path(COMMON_LLVM_O)
 llvm.ObjectFileRef.from_path(SHELL_LLVM_O)
 
 EXTERNAL_FUNCTION_TYPE = ir.FunctionType(
     ir.IntType(32),
     [
         ir.IntType(32),
         ir.PointerType(ir.IntType(8)),
```

### Comparing `red_team_language-0.1.1/rtl/parser/transform/transform.py` & `red_team_language-0.2.0/rtl/parser/transform/transform.py`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/parser/transform/xor.py` & `red_team_language-0.2.0/rtl/parser/transform/xor.py`

 * *Files identical despite different names*

### Comparing `red_team_language-0.1.1/rtl/rtl.py` & `red_team_language-0.2.0/rtl/rtl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import shlex
 
 from argparse import ArgumentParser
 from pathlib import PosixPath
 
 from rtl.parser.driver import Driver
 
+CURRENT_PATH = PosixPath(__file__).parent
+
 
 def main():
     parser = ArgumentParser(
         "rtl",
         None,
         "The Red-Team-Language compiler enables one to write scripts and deploy them as static executables - for the lolz of course!",
         add_help=True,
@@ -58,15 +60,14 @@
     )
 
     args = parser.parse_args()
 
     driver = Driver(args.src)
 
     if not args.build:
-
         if not args.ir and not args.asm and not args.obj:
             args.ir = True
 
         print(driver.emit(args))
     else:
         """
         The following is the silliest, shortsighted, sick, stultification of code ever seen; in short, stereoisomeric with shit...I'll fix it someday...
@@ -78,34 +79,63 @@
 
         fn = driver.emit(args)
 
         filename = f"{PosixPath('/tmp/').joinpath(PosixPath(f'{args.src}').stem)}.elf"
 
         import subprocess
 
+        from rtl.lib.protocol.common import COMMON_LLVM_O
         from rtl.lib.protocol.shell import SHELL_LLVM_O
+        from rtl.lib.protocol.ssh import SSH_LLVM_O
         from rtl.lib.transform.xor import XOR_LLVM_O
 
+        llvm_ir_contents = str(driver.module)
+
+        LLVM_O = f"{COMMON_LLVM_O}"
+        INCLUDES = ""
+        LIBRARY_PATHS = ""
         CFLAGS = "-fPIC"
-        args = shlex.split(f"zig cc -target {driver.rtl_target} {CFLAGS} {SHELL_LLVM_O} {XOR_LLVM_O} {fn} -o {filename}")
+
+        if ".shell" in llvm_ir_contents:
+            LLVM_O += f" {SHELL_LLVM_O}"
+
+        if ".ssh" in llvm_ir_contents:
+            LLVM_O += f" {SSH_LLVM_O}"
+            INCLUDES += f" -I{CURRENT_PATH}/lib/protocol/ssh/libssh2/include/"
+            LIBRARY_PATHS += f" -L{CURRENT_PATH}/lib/protocol/ssh/libssh2/build/src"
+            LIBRARY_PATHS += f" -L{CURRENT_PATH}/lib/protocol/ssh/mbedtls/build/library"
+            # CFLAGS += " -Wl,-s"
+            CFLAGS += " -lssh2"
+            CFLAGS += " -lmbedtls"
+            CFLAGS += " -lmbedcrypto"
+            CFLAGS += " -lmbedx509"
+
+        if ".xor" in llvm_ir_contents:
+            LLVM_O += f" {XOR_LLVM_O}"
+
+        print(LLVM_O)
+
+        args = shlex.split(
+            f"zig cc -g {INCLUDES} {LIBRARY_PATHS} -target {driver.rtl_target} {CFLAGS} {LLVM_O} {fn} -o {filename}"
+        )
 
         if (
             subprocess.call(
                 args,
                 cwd=f"{PosixPath(__file__).parent}",
             )
             != 0
         ):
             print(
                 "Failed to compile - is zig on PATH? build...is an experiment in how horrible one can write functional Python code xD"
             )
             exit(2)
         else:
-            subprocess.call(
-                shlex.split(f"strip -s {filename}"),
-                cwd=f"{PosixPath(__file__).parent}",
-            )
+            # subprocess.call(
+            #     shlex.split(f"strip -s {filename}"),
+            #     cwd=f"{PosixPath(__file__).parent}",
+            # )
             print(f"done building {filename}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `red_team_language-0.1.1/setup.cfg` & `red_team_language-0.2.0/setup.cfg`

 * *Files identical despite different names*

