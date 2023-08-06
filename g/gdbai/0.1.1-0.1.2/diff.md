# Comparing `tmp/gdbai-0.1.1.tar.gz` & `tmp/gdbai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdbai-0.1.1.tar", max compression
+gzip compressed data, was "gdbai-0.1.2.tar", max compression
```

## Comparing `gdbai-0.1.1.tar` & `gdbai-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     5641 2023-08-06 11:22:20.195651 gdbai-0.1.1/README.md
--rw-r--r--   0        0        0     7515 2023-08-06 11:22:20.195651 gdbai-0.1.1/gdbai.py
--rw-r--r--   0        0        0      314 2023-08-06 11:22:20.195651 gdbai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6196 1970-01-01 00:00:00.000000 gdbai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-06 11:59:10.398990 gdbai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5716 2023-08-06 11:59:10.398990 gdbai-0.1.2/README.md
+-rw-r--r--   0        0        0     7515 2023-08-06 11:59:10.398990 gdbai-0.1.2/gdbai.py
+-rw-r--r--   0        0        0      362 2023-08-06 11:59:10.398990 gdbai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6373 1970-01-01 00:00:00.000000 gdbai-0.1.2/PKG-INFO
```

### Comparing `gdbai-0.1.1/README.md` & `gdbai-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 ## 命令
 - ai - 根据当前堆栈信息回答问题
 - chat - 和GPT聊天
 - trans - 将自然语言翻译称一条GDB命令
 - explain - 解释GDB命令的含义
 
 ## load
-`(gdb) source /path/to/gdbai/gdbai.py ` every time or add it to `.gdbinit`
+`(gdb) source /path/to/gdbai/gdbai.py ` every time 
+
+or add it to `.gdbinit`
+
+`echo "source $(python -m site --user-site)/gdbai.py" > $HOME/.gdbinit`
 
 ```
 (gdb) source /path/to/gdbai/gdbai.py 
 usage:
         ai
         ai Explain what the root cause of this error is.Give me Suggestions
         ai 用中文回答无效指针是哪个
```

### Comparing `gdbai-0.1.1/gdbai.py` & `gdbai-0.1.2/gdbai.py`

 * *Files identical despite different names*

### Comparing `gdbai-0.1.1/PKG-INFO` & `gdbai-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: gdbai
-Version: 0.1.1
+Version: 0.1.2
 Summary: gdb AI assistant
+Home-page: https://github.com/airob0t/gdbai
 License: GPLv3
 Author: airobot
 Author-email: airobot@airobot.link
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.8,<0.28.0)
+Project-URL: Repository, https://github.com/airob0t/gdbai
 Description-Content-Type: text/markdown
 
 # GDBAI
 GDB AI assistant plugin. Debug with GPT.
 
 GDB AI助手插件,和GPT一起debug.
 
@@ -45,15 +47,19 @@
 ## 命令
 - ai - 根据当前堆栈信息回答问题
 - chat - 和GPT聊天
 - trans - 将自然语言翻译称一条GDB命令
 - explain - 解释GDB命令的含义
 
 ## load
-`(gdb) source /path/to/gdbai/gdbai.py ` every time or add it to `.gdbinit`
+`(gdb) source /path/to/gdbai/gdbai.py ` every time 
+
+or add it to `.gdbinit`
+
+`echo "source $(python -m site --user-site)/gdbai.py" > $HOME/.gdbinit`
 
 ```
 (gdb) source /path/to/gdbai/gdbai.py 
 usage:
         ai
         ai Explain what the root cause of this error is.Give me Suggestions
         ai 用中文回答无效指针是哪个
```

