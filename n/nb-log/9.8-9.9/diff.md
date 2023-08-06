# Comparing `tmp/nb_log-9.8.tar.gz` & `tmp/nb_log-9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_log-9.8.tar", last modified: Fri Jul 21 14:26:59 2023, max compression
+gzip compressed data, was "nb_log-9.9.tar", last modified: Fri Jul 28 15:15:08 2023, max compression
```

## Comparing `nb_log-9.8.tar` & `nb_log-9.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 14:26:59.102989 nb_log-9.8/
--rw-rw-rw-   0        0        0    30393 2023-07-21 14:26:59.099990 nb_log-9.8/PKG-INFO
--rw-rw-rw-   0        0        0    29460 2023-07-03 13:46:53.000000 nb_log-9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 14:26:59.073990 nb_log-9.8/nb_log/
--rw-rw-rw-   0        0        0     3192 2023-07-02 07:24:38.000000 nb_log-9.8/nb_log/__init__.py
--rw-rw-rw-   0        0        0     3423 2023-07-06 13:56:36.000000 nb_log-9.8/nb_log/file_write.py
--rw-rw-rw-   0        0        0    51517 2023-07-09 11:39:13.000000 nb_log-9.8/nb_log/handlers.py
--rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.8/nb_log/handlers0000.py
--rw-rw-rw-   0        0        0    31273 2023-07-09 05:58:10.000000 nb_log-9.8/nb_log/log_manager.py
--rw-rw-rw-   0        0        0     6841 2023-07-21 14:24:52.000000 nb_log-9.8/nb_log/monkey_print.py
--rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.8/nb_log/monkey_std_filter_words.py
--rw-rw-rw-   0        0        0     2420 2023-07-21 14:24:52.000000 nb_log-9.8/nb_log/monkey_sys_std.py
--rw-rw-rw-   0        0        0    10921 2023-07-14 15:43:54.000000 nb_log-9.8/nb_log/nb_log_config_default.py
--rw-rw-rw-   0        0        0     5127 2023-07-06 13:55:43.000000 nb_log-9.8/nb_log/nb_logger.py
--rw-rw-rw-   0        0        0     6283 2023-07-09 13:55:16.000000 nb_log-9.8/nb_log/rotate_file_writter.py
--rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.8/nb_log/set_nb_log_config.py
--rw-rw-rw-   0        0        0     2067 2023-07-09 04:17:03.000000 nb_log-9.8/nb_log/simple_print.py
-drwxrwxrwx   0        0        0        0 2023-07-21 14:26:59.094987 nb_log-9.8/nb_log.egg-info/
--rw-rw-rw-   0        0        0    30393 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 14:26:58.000000 nb_log-9.8/nb_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 14:26:59.102989 nb_log-9.8/setup.cfg
--rw-rw-rw-   0        0        0     2376 2023-07-21 14:26:19.000000 nb_log-9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:15:08.286917 nb_log-9.9/
+-rw-rw-rw-   0        0        0    33588 2023-07-28 15:15:08.284922 nb_log-9.9/PKG-INFO
+-rw-rw-rw-   0        0        0    32655 2023-07-28 15:14:50.000000 nb_log-9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 15:15:08.254917 nb_log-9.9/nb_log/
+-rw-rw-rw-   0        0        0     3256 2023-07-28 14:00:29.000000 nb_log-9.9/nb_log/__init__.py
+-rw-rw-rw-   0        0        0     5145 2023-07-28 13:33:38.000000 nb_log-9.9/nb_log/compatible_logger.py
+-rw-rw-rw-   0        0        0     2961 2023-07-28 14:25:01.000000 nb_log-9.9/nb_log/direct_logger.py
+-rw-rw-rw-   0        0        0     3423 2023-07-06 13:56:36.000000 nb_log-9.9/nb_log/file_write.py
+-rw-rw-rw-   0        0        0    51517 2023-07-09 11:39:13.000000 nb_log-9.9/nb_log/handlers.py
+-rw-rw-rw-   0        0        0    49868 2022-09-12 12:13:59.000000 nb_log-9.9/nb_log/handlers0000.py
+-rw-rw-rw-   0        0        0    31331 2023-07-28 13:37:38.000000 nb_log-9.9/nb_log/log_manager.py
+-rw-rw-rw-   0        0        0     6841 2023-07-21 14:24:52.000000 nb_log-9.9/nb_log/monkey_print.py
+-rw-rw-rw-   0        0        0      853 2023-07-01 05:26:36.000000 nb_log-9.9/nb_log/monkey_std_filter_words.py
+-rw-rw-rw-   0        0        0     2420 2023-07-21 14:24:52.000000 nb_log-9.9/nb_log/monkey_sys_std.py
+-rw-rw-rw-   0        0        0    10958 2023-07-28 13:25:05.000000 nb_log-9.9/nb_log/nb_log_config_default.py
+-rw-rw-rw-   0        0        0     6283 2023-07-09 13:55:16.000000 nb_log-9.9/nb_log/rotate_file_writter.py
+-rw-rw-rw-   0        0        0     6066 2023-07-03 14:08:57.000000 nb_log-9.9/nb_log/set_nb_log_config.py
+-rw-rw-rw-   0        0        0     2067 2023-07-09 04:17:03.000000 nb_log-9.9/nb_log/simple_print.py
+drwxrwxrwx   0        0        0        0 2023-07-28 15:15:08.278917 nb_log-9.9/nb_log.egg-info/
+-rw-rw-rw-   0        0        0    33588 2023-07-28 15:15:07.000000 nb_log-9.9/nb_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-07-28 15:15:08.000000 nb_log-9.9/nb_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 15:15:07.000000 nb_log-9.9/nb_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-07-28 15:15:07.000000 nb_log-9.9/nb_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 15:15:07.000000 nb_log-9.9/nb_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 15:15:08.287917 nb_log-9.9/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2023-07-28 15:14:50.000000 nb_log-9.9/setup.py
```

### Comparing `nb_log-9.8/PKG-INFO` & `nb_log-9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_log
-Version: 9.8
+Version: 9.9
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -479,14 +479,62 @@
 defaul_logger.info("hello")
 
 但这样有个弊端，用户想使用什么日志模板，用户希望日志记录到 控制台 文件 钉钉 es中的哪几个地方没法定义。
 用户如果想屏蔽a函数里面的日志，但想放开b函数里面的日志，这种不传参/不设置日志命名空间的日志就无能为力做到了。
 所以nb_log推荐用户调用get_logger函数来自定义日志，而不是直接import defaul_logger然后所有地方都使用这个 defaul_logger来记录日志。
 ```
 
+### 1.8.4 nb_log的使用可以比loguru更简单
+
+loguru:
+```
+from loguru import logger
+logger.add("./log_files/loguru-test1.log",  rotation="100000 KB")
+logger.info("hello")
+```
+
+nb_log ,你想简单不想get_loger,你想粗暴的导入就能记录日志到控制台和文件，代码如下：
+```
+import nb_log
+
+nb_log.debug('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用debug函数，那就满足这种人')
+nb_log.info('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用info函数，那就满足这种人')
+nb_log.warning('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用warning函数，那就满足这种人')
+nb_log.error('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用error函数，那就满足这种人')
+nb_log.critical('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用critical函数，那就满足这种人')
+
+```
+[![pPSClpF.png](https://s1.ax1x.com/2023/07/28/pPSClpF.png)](https://imgse.com/i/pPSClpF)
+
+```
+有的笨瓜总是不能理解 logging.getLogger第一个入参name的作用和巨大好处，老是觉得需要实例化生成 logger 对象觉得麻烦，想开箱即用，那就满足这种人。
+用from loguru import logger 这种日志，先不同模块或功能的日志设置不同级别，不同的模块写入不同的文件，非常麻烦不优雅。
+但有的人完全不理解 日志命名空间的作用，只会抱怨nb_log的例子要他实例化不同name的logger麻烦，那就满足这种人，不用他手动实例化生成不同命名空间的logger。
+
+import nb_log
+
+nb_log.debug('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用debug函数，那就满足这种人')
+nb_log.info('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用info函数，那就满足这种人')
+nb_log.warning('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用warning函数，那就满足这种人')
+nb_log.error('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用error函数，那就满足这种人')
+nb_log.critical('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用critical函数，那就满足这种人')
+
+
+loguru的用法是：
+from loguru import logger
+logger.debug(msg)
+
+nb_log的用法是：
+import nb_log
+nb_log.debug(msg)
+
+nb_log比loguru少了 from import那不是更简洁了吗？满足这种只知道追求简单的笨瓜。
+```
+
+
 
 综上所述 nb_log既使用简单，又兼容性高。
 
 ## 1.9 内置logging包的日志命名空间是什么
 
 ```python
 import logging
```

### Comparing `nb_log-9.8/README.md` & `nb_log-9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -457,14 +457,62 @@
 defaul_logger.info("hello")
 
 但这样有个弊端，用户想使用什么日志模板，用户希望日志记录到 控制台 文件 钉钉 es中的哪几个地方没法定义。
 用户如果想屏蔽a函数里面的日志，但想放开b函数里面的日志，这种不传参/不设置日志命名空间的日志就无能为力做到了。
 所以nb_log推荐用户调用get_logger函数来自定义日志，而不是直接import defaul_logger然后所有地方都使用这个 defaul_logger来记录日志。
 ```
 
+### 1.8.4 nb_log的使用可以比loguru更简单
+
+loguru:
+```
+from loguru import logger
+logger.add("./log_files/loguru-test1.log",  rotation="100000 KB")
+logger.info("hello")
+```
+
+nb_log ,你想简单不想get_loger,你想粗暴的导入就能记录日志到控制台和文件，代码如下：
+```
+import nb_log
+
+nb_log.debug('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用debug函数，那就满足这种人')
+nb_log.info('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用info函数，那就满足这种人')
+nb_log.warning('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用warning函数，那就满足这种人')
+nb_log.error('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用error函数，那就满足这种人')
+nb_log.critical('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用critical函数，那就满足这种人')
+
+```
+[![pPSClpF.png](https://s1.ax1x.com/2023/07/28/pPSClpF.png)](https://imgse.com/i/pPSClpF)
+
+```
+有的笨瓜总是不能理解 logging.getLogger第一个入参name的作用和巨大好处，老是觉得需要实例化生成 logger 对象觉得麻烦，想开箱即用，那就满足这种人。
+用from loguru import logger 这种日志，先不同模块或功能的日志设置不同级别，不同的模块写入不同的文件，非常麻烦不优雅。
+但有的人完全不理解 日志命名空间的作用，只会抱怨nb_log的例子要他实例化不同name的logger麻烦，那就满足这种人，不用他手动实例化生成不同命名空间的logger。
+
+import nb_log
+
+nb_log.debug('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用debug函数，那就满足这种人')
+nb_log.info('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用info函数，那就满足这种人')
+nb_log.warning('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用warning函数，那就满足这种人')
+nb_log.error('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用error函数，那就满足这种人')
+nb_log.critical('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用critical函数，那就满足这种人')
+
+
+loguru的用法是：
+from loguru import logger
+logger.debug(msg)
+
+nb_log的用法是：
+import nb_log
+nb_log.debug(msg)
+
+nb_log比loguru少了 from import那不是更简洁了吗？满足这种只知道追求简单的笨瓜。
+```
+
+
 
 综上所述 nb_log既使用简单，又兼容性高。
 
 ## 1.9 内置logging包的日志命名空间是什么
 
 ```python
 import logging
```

### Comparing `nb_log-9.8/nb_log/__init__.py` & `nb_log-9.9/nb_log/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,25 @@
 
 
 
 from nb_log import handlers
 from nb_log.log_manager import LogManager, LoggerLevelSetterMixin, LoggerMixin, LoggerMixinDefaultWithFileHandler, get_logger, get_logger_with_filehanlder
 
 
-simple_logger = LogManager('simple').get_logger_and_add_handlers()
+simple_logger = get_logger('simple')
 defaul_logger = LogManager('defaul').get_logger_and_add_handlers(do_not_use_color_handler=True, formatter_template=7)
 default_file_logger = LogManager('default_file_logger').get_logger_and_add_handlers(log_filename='default_file_logger.log')
 
 logger_dingtalk_common = LogManager('钉钉通用报警提示').get_logger_and_add_handlers(
     ding_talk_token=nb_log_config_default.DING_TALK_TOKEN,
     log_filename='dingding_common.log')
 
+
+from nb_log.direct_logger import debug,info,warning,error,exception,critical
+
 only_print_on_main_process('\033[0m' + r"""
 
 .__   __. .______           __        ______     _______ 
 |  \ |  | |   _  \         |  |      /  __  \   /  _____|
 |   \|  | |  |_)  |  ______|  |     |  |  |  | |  |  __  
 |  . `  | |   _  <  |______|  |     |  |  |  | |  | |_ | 
 |  |\   | |  |_)  |        |  `----.|  `--'  | |  |__| | 
@@ -55,7 +58,13 @@
 
         nb_log文档 https://nb-log-doc.readthedocs.io/zh_CN/latest/
 
         为什么要设置pycharm终端颜色，解释为什么\\033不能决定最终颜色 https://nb-log-doc.readthedocs.io/zh_CN/latest/articles/c1.html#c
         \033[0m
 
         """)
+
+
+
+
+
+
```

### Comparing `nb_log-9.8/nb_log/file_write.py` & `nb_log-9.9/nb_log/file_write.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/handlers.py` & `nb_log-9.9/nb_log/handlers.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/handlers0000.py` & `nb_log-9.9/nb_log/handlers0000.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/log_manager.py` & `nb_log-9.9/nb_log/log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 """
 import logging
 import multiprocessing
 import typing
 from functools import lru_cache
 from logging import FileHandler, _checkLevel  # noqa
-from nb_log import nb_log_config_default, nb_logger  # noqa
+from nb_log import nb_log_config_default, compatible_logger  # noqa
+from nb_log.compatible_logger import CompatibleLogger
 from nb_log.handlers import *
 import deprecated
 
 
 # noinspection DuplicatedCode
 def revision_call_handlers(self, record):  # 对logging标准模块打猴子补丁。主要是使父命名空间的handler不重复记录当前命名空间日志已有种类的handler。
     """
@@ -209,26 +210,26 @@
     一个日志管理类，用于创建logger和添加handler，支持将日志打印到控制台打印和写入日志文件和mongodb和邮件。
     """
     logger_name_list = []
     logger_list = []
     preset_name__level_map = dict()
 
     # logger_cls = logging.Logger
-    logger_cls = nb_logger.NbLogger
+    logger_cls = CompatibleLogger
 
     def __init__(self, logger_name: typing.Union[str, None] = 'nb_log_default_namespace'):
         """
         :param logger_name: 日志名称，当为None时候创建root命名空间的日志，一般情况下千万不要传None，除非你确定需要这么做和是在做什么.这个命名空间是双刃剑
         """
         if logger_name in (None, '',) and multiprocessing.process.current_process().name == 'MainProcess':
             very_nb_print('logger_name 设置为None和空字符串都是一个意义，在操作根日志命名空间，任何其他日志的行为将会发生变化，'
                           '一定要弄清楚原生logging包的日志name的意思。这个命名空间是双刃剑')
         self._logger_name = logger_name
-        if self.logger_cls == nb_logger.NbLogger:
-            self.logger = nb_logger.NbLogger(logger_name)
+        if self.logger_cls == CompatibleLogger:
+            self.logger = CompatibleLogger(logger_name)
         else:
             self.logger = logging.getLogger(logger_name)
 
     def preset_log_level(self, log_level_int=20):
         """
         提前设置锁定日志级别，当之后再设置该命名空间日志的级别的时候，按照提前预设的级别，无视之后设定的级别。
         主要是针对动态初始化的日志，在生成日志之后再去设置日志级别不方便。
@@ -302,15 +303,15 @@
         # else:
         #     self._logger_level = self._logger_level
         self._is_add_stream_handler = is_add_stream_handler
         self._do_not_use_color_handler = do_not_use_color_handler
         self._log_path = log_path
         self._log_filename = log_filename
         self._log_file_size = log_file_size
-        if log_file_handler_type not in (None, 1, 2, 3, 4, 5,6):
+        if log_file_handler_type not in (None, 1, 2, 3, 4, 5, 6):
             raise ValueError("log_file_handler_type的值必须设置为 1 2 3 4 5 6 这几个数字")
         self._log_file_handler_type = log_file_handler_type or nb_log_config_default.LOG_FILE_HANDLER_TYPE
         self._mongo_url = mongo_url
         self._is_add_elastic_handler = is_add_elastic_handler
         self._is_add_kafka_handler = is_add_kafka_handler
         self._ding_talk_token = ding_talk_token
         self._ding_talk_time_interval = ding_talk_time_interval
```

### Comparing `nb_log-9.8/nb_log/monkey_print.py` & `nb_log-9.9/nb_log/monkey_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/monkey_std_filter_words.py` & `nb_log-9.9/nb_log/monkey_std_filter_words.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/monkey_sys_std.py` & `nb_log-9.9/nb_log/monkey_sys_std.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/nb_log_config_default.py` & `nb_log-9.9/nb_log/nb_log_config_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf8
 """
-此文件nb_log_config.py是自动生成到python项目的根目录的。
+此文件nb_log_config.py是自动生成到python项目的根目录的,因为是自动生成到 sys.path[1]。
 在这里面写的变量会覆盖此文件nb_log_config_default中的值。对nb_log包进行默认的配置。用户是无需修改nb_log安装包位置里面的配置文件的。
 
 但最终配置方式是由get_logger_and_add_handlers方法的各种传参决定，如果方法相应的传参为None则使用这里面的配置。
 """
 
 """
 如果反对日志有各种彩色，可以设置 DEFAULUT_USE_COLOR_HANDLER = False
```

### Comparing `nb_log-9.8/nb_log/nb_logger.py` & `nb_log-9.9/nb_log/compatible_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 '''
 
 '''
 有的人手痒，非要封装nb_log,那么封装时候调用原生日志的 info() 务必要传入  extra={'sys_getframe_n': 3}
 如果你不传递 extra={'sys_getframe_n': 3} ，那么 废物日志类().info('啊啊啊啊') ，显示是第 x2 行打印的日志，而不是第 y行打印的日志。
 '''
 
-class NbLogger(logging.Logger):
+
+class CompatibleLogger(logging.Logger):
 
     """
-    写 NbLogger 实在python3.7测试的，python3.9以后官方已经加了stacklevel入参。
+    写 CompatibleLogger 是在python3.7测试的，python3.9以后官方已经加了stacklevel入参。
     20230705 现在经过github cpython的源码核实，在python3.9版本中
     def _log(self, level, msg, args, exc_info=None, extra=None, stack_info=False,
              stacklevel=1):
 
     def findCaller(self, stack_info=False, stacklevel=1):
 
     用户可以传递 stacklevel 了，本NbLogger是适配python3.6 3.7 3.8版本, Nblogger 的 sys_getframe_n 入参就是 stacklevel的意义。
```

### Comparing `nb_log-9.8/nb_log/rotate_file_writter.py` & `nb_log-9.9/nb_log/rotate_file_writter.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/set_nb_log_config.py` & `nb_log-9.9/nb_log/set_nb_log_config.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log/simple_print.py` & `nb_log-9.9/nb_log/simple_print.py`

 * *Files identical despite different names*

### Comparing `nb_log-9.8/nb_log.egg-info/PKG-INFO` & `nb_log-9.9/nb_log.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-log
-Version: 9.8
+Version: 9.9
 Summary: very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on 
 Home-page: https://github.com/ydf0509/nb_log
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -479,14 +479,62 @@
 defaul_logger.info("hello")
 
 但这样有个弊端，用户想使用什么日志模板，用户希望日志记录到 控制台 文件 钉钉 es中的哪几个地方没法定义。
 用户如果想屏蔽a函数里面的日志，但想放开b函数里面的日志，这种不传参/不设置日志命名空间的日志就无能为力做到了。
 所以nb_log推荐用户调用get_logger函数来自定义日志，而不是直接import defaul_logger然后所有地方都使用这个 defaul_logger来记录日志。
 ```
 
+### 1.8.4 nb_log的使用可以比loguru更简单
+
+loguru:
+```
+from loguru import logger
+logger.add("./log_files/loguru-test1.log",  rotation="100000 KB")
+logger.info("hello")
+```
+
+nb_log ,你想简单不想get_loger,你想粗暴的导入就能记录日志到控制台和文件，代码如下：
+```
+import nb_log
+
+nb_log.debug('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用debug函数，那就满足这种人')
+nb_log.info('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用info函数，那就满足这种人')
+nb_log.warning('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用warning函数，那就满足这种人')
+nb_log.error('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用error函数，那就满足这种人')
+nb_log.critical('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用critical函数，那就满足这种人')
+
+```
+[![pPSClpF.png](https://s1.ax1x.com/2023/07/28/pPSClpF.png)](https://imgse.com/i/pPSClpF)
+
+```
+有的笨瓜总是不能理解 logging.getLogger第一个入参name的作用和巨大好处，老是觉得需要实例化生成 logger 对象觉得麻烦，想开箱即用，那就满足这种人。
+用from loguru import logger 这种日志，先不同模块或功能的日志设置不同级别，不同的模块写入不同的文件，非常麻烦不优雅。
+但有的人完全不理解 日志命名空间的作用，只会抱怨nb_log的例子要他实例化不同name的logger麻烦，那就满足这种人，不用他手动实例化生成不同命名空间的logger。
+
+import nb_log
+
+nb_log.debug('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用debug函数，那就满足这种人')
+nb_log.info('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用info函数，那就满足这种人')
+nb_log.warning('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用warning函数，那就满足这种人')
+nb_log.error('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用error函数，那就满足这种人')
+nb_log.critical('笨瓜不想实例化多个不同name的logger,不理解logging.getLogger第一个入参name的作用和好处，想直接粗暴的调用critical函数，那就满足这种人')
+
+
+loguru的用法是：
+from loguru import logger
+logger.debug(msg)
+
+nb_log的用法是：
+import nb_log
+nb_log.debug(msg)
+
+nb_log比loguru少了 from import那不是更简洁了吗？满足这种只知道追求简单的笨瓜。
+```
+
+
 
 综上所述 nb_log既使用简单，又兼容性高。
 
 ## 1.9 内置logging包的日志命名空间是什么
 
 ```python
 import logging
```

### Comparing `nb_log-9.8/setup.py` & `nb_log-9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 if os.name == 'nt':
     install_requires.append('pywin32')
 
 setup(
     name='nb_log',  #
-    version="9.8",
+    version="9.9",
     description=(
         'very sharp color display,monkey patch bulitin print  and high-performance multiprocess safe roating file handler,other handlers includeing dintalk ,email,kafka,elastic and so on '
     ),
     keywords=["logging", "logger", "multiprocess file handler", "color handler"],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -63,14 +63,14 @@
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
 
 python setup.py sdist & twine upload dist/nb_log-6.0.tar.gz
-python setup.py sdist & python -m  twine upload dist/nb_log-9.8.tar.gz
+python setup.py sdist & python -m  twine upload dist/nb_log-9.9.tar.gz
 
 twine upload dist/*
 
 
 python -m pip install nb_log --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

